# Linux Core Concepts

- Take me to the [Video Tutorial](https://kodekloud.com/topic/linux-kernel/)

In this section, we will take a look at the core concepts of a linux operating system.
- We will start with introduction to the linux kernel.
- We will then learn about the kernel space and user space.

## Linux Kernel

#### If you have worked with any operating system, you have run into the term kernel. 

- The Linux kernel is monolithic, this means that the kernel carrries out CPU scheduling, memory management and several operations by itselfs. 
- The Linux Kernel is also modular, which means it can extends its capabilities through the use of dynamically loaded kernel modules

 <img width="779" height="403" alt="k1" src="https://github.com/user-attachments/assets/bd0e6c23-2901-4001-aad3-1cc1b5f48846" />


#### To understand a kernel in simple terms, let us use an analogy of a **`College Library`**. Here the librarian is equal to Linux Kernel.

<img width="787" height="417" alt="k2" src="https://github.com/user-attachments/assets/3c46261c-2a09-4440-99ec-8f5e9663e947" />


#### The Kernel is responsible for 4 major tasks

1. Memory Management
1. Process Management
1. Device Drivers
1. System calls and Security

## Linux Kernel Versions

#### let us know identify the ways to identify linux kernel versions

Use **`uname`** command to get the information about the kernel (by itself it doesn't provide much information except that the system uses the **`Linux`** Kernel.
```
$ uname
```

Use the **`uname -r`** or **`uname`** comamnd and option to print the kernel version
```
$ uname -r
$ uname -a
```
<img width="918" height="452" alt="k3" src="https://github.com/user-attachments/assets/a8f5601b-83f6-4351-aefc-e8609d4de641" />


## Kernel and User Space

#### One of the important functions of the linux kernel is the **`Memory Management`** . We will now see how memory is seperated within the linux kernel

Memory is divded into two areas.
1. Kernel Space
   1. Kernel Code
   1. kernel Extensions
   1. Device Drivers
1. User Space
   1. C
   1. Java
   1. Python
   1. Ruby e.t.c
   1. Docker Containers
   <img width="710" height="476" alt="k4" src="https://github.com/user-attachments/assets/397b0303-fe25-4571-ab1e-978aea9e9ec9" />


#### Let us know see how programs running in the `User Space` work

All user programs function by manipulating data that is stored in memory and on disk. User programs get access to data by making special request to the kernel called **`System Calls`**
- Examples include, allocating memory by using variables or opening a file.

<img width="987" height="453" alt="k5" src="https://github.com/user-attachments/assets/55fc164b-cf6b-465b-9b9f-4b4d11b666d1" />


- For example, opening a file such as the **`/etc/os-release`** to see the operating system installed, results in a **`system call`**

  ![user-space1](../../images/user-space1.PNG)
