# Run Levels

- Take me to the [Video Tutorial](https://kodekloud.com/topic/runlevels/)

## Systemd Targets (Run Levels)

We can setup the server to boot either into graphical mode or non-graphical mode. Linux can run in multiple modes and these modes are set by something called **`runlevel`**
- The operation mode which provide a graphical interface is called **`runlevel 5`**
- The operation mode which provide a non-graphical mode is called **`runlevel 3`**
<img width="945" height="469" alt="r1" src="https://github.com/user-attachments/assets/79555d25-c99c-4d08-8a3c-b15051215c04" />


To see the operation mode run in the system. Run the command **`runlevel`** from the terminal
```
$ runlevel
```

During boot, the **`init`** process checks the **`runlevel`**, it make sure that all programs need to get the system operation in that mode are started.
  - For example: The **`Graphical User`** mode requires a **`display manager`** service to run for the GUI to work, however this service is not required for the **`non-graphical mode`**
<img width="1239" height="601" alt="r2" src="https://github.com/user-attachments/assets/c384c8c2-6c06-41d8-acde-d6825f1209b6" />


In the boot process section, we saw that the **`systemd`** is used as the **`init`** process in most new linux distributions suchs as **`Ubuntu 18.04`**.
- In **`systemd`**, runlevels are called as **`targets`**.
  - The RunLevel 5 is called as the **`graphical target`** 
  - The Runlevel 3 is called as the **`multiuser target`**
  <img width="1231" height="560" alt="r3" src="https://github.com/user-attachments/assets/f321c50d-1ec0-414b-8c83-ffc52b06a834" />


#### Now that we are familiar with runlevels in systemd target unit. Lets now take a look at how we change these values from a shell.

To see the default target, run the command **`systemctl get-default`**. This command looks at the file located at **`/etc/systemd/system/default.target`** 
```
$ systemctl get-default
```

To change the default target, we can make use of **`systemctl set-target <desired target name goes here as an argument>`**
```
$ systemctl set-default multi-user.target 
```

