# Linux Networking Commands

## 1. ping
Checks connectivity to a host.

ping google.com

Send limited packets:
ping -c 4 google.com

---

## 2. ip
Displays IP address and network details.

ip a
ip route

---

## 3. ifconfig
Shows network configuration (older command).

ifconfig

---

## 4. netstat
Displays network connections.

netstat -tulnp

---

## 5. ss
Modern replacement for netstat.

ss -tulnp

---

## 6. curl
Transfers data from server.

curl http://example.com

---

## 7. wget
Downloads files from internet.

wget http://example.com/file.zip

---

## 8. traceroute
Shows path taken by packets.

traceroute google.com

---

## 9. hostname
Displays system hostname.

hostname

---

## 10. nslookup
Finds DNS records.

nslookup google.com

---

## 11. dig
Detailed DNS lookup.

dig google.com

---

# Important Ports

22   - SSH  
80   - HTTP  
443  - HTTPS  
21   - FTP  
25   - SMTP  
3306 - MySQL  
8080 - Application Server  

---

# Practical Lab

1. Check IP address:
   ip a

2. Test internet connection:
   ping -c 4 google.com

3. Check open ports:
   ss -tulnp

4. Test website:
   curl http://example.com

5. Perform DNS lookup:
   nslookup google.com
