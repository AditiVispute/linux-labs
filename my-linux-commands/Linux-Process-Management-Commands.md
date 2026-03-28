# Linux Process Management Commands

## 1. ps
Displays running processes.

ps
ps -ef
ps aux

---

## 2. top
Shows real-time system processes.

top

Press q to exit.

---

## 3. htop
Interactive process viewer (if installed).

htop

---

## 4. kill
Terminates a process using PID.

kill PID

Force kill:
kill -9 PID

---

## 5. pkill
Kills process using name.

pkill processname

Example:
pkill nginx

---

## 6. bg
Resumes a suspended job in background.

bg

---

## 7. fg
Brings background job to foreground.

fg

---

## 8. jobs
Displays background jobs.

jobs

---

## 9. nice
Starts a process with priority.

nice -n 10 command

---

## 10. systemctl
Manages system services.

Start service:
sudo systemctl start nginx

Stop service:
sudo systemctl stop nginx

Restart service:
sudo systemctl restart nginx

Check status:
sudo systemctl status nginx

Enable at boot:
sudo systemctl enable nginx

---

# Practical Lab

1. Run a background process:
   sleep 300 &

2. Check running processes:
   ps aux | grep sleep

3. Find process ID:
   pgrep sleep

4. Kill process:
   kill -9 $(pgrep sleep)

5. Check jobs:
   jobs
