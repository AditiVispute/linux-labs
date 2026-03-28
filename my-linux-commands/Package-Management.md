# Linux Package Management Commands

## For Ubuntu / Debian (APT)

## 1. Update package list
sudo apt update

---

## 2. Upgrade installed packages
sudo apt upgrade

---

## 3. Install a package
sudo apt install nginx

---

## 4. Remove a package
sudo apt remove nginx

---

## 5. Remove package with configuration
sudo apt purge nginx

---

## 6. Search for a package
apt search nginx

---

## 7. Show package details
apt show nginx

---

## 8. List installed packages
apt list --installed

---

## For RedHat / CentOS (YUM)

## 1. Install a package
sudo yum install nginx

---

## 2. Remove a package
sudo yum remove nginx

---

## 3. Update packages
sudo yum update

---

## 4. List installed packages
yum list installed

---

# Practical Lab

1. Update system:
   sudo apt update

2. Install nginx:
   sudo apt install nginx

3. Check service status:
   sudo systemctl status nginx

4. Stop service:
   sudo systemctl stop nginx

5. Remove package:
   sudo apt remove nginx
