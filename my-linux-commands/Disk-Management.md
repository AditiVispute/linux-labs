# Linux Disk Management Commands

## 1. df
Shows disk space usage.

df
df -h

---

## 2. du
Shows file and directory size.

du -h
du -sh foldername

---

## 3. lsblk
Displays block devices (disks and partitions).

lsblk

---

## 4. fdisk
Used for disk partitioning.

sudo fdisk -l

---

## 5. mount
Mounts a filesystem.

sudo mount /dev/sdb1 /mnt

---

## 6. umount
Unmounts a filesystem.

sudo umount /mnt

---

## 7. mkfs
Formats a disk partition.

sudo mkfs.ext4 /dev/sdb1

---

## 8. blkid
Displays UUID of disks.

blkid

---

## 9. df -i
Shows inode usage.

df -i

---

# Practical Lab

1. Check disk space:
   df -h

2. Check directory size:
   du -sh .

3. List disks:
   lsblk

4. Create mount directory:
   sudo mkdir /mnt/data

5. Mount disk:
   sudo mount /dev/sdb1 /mnt/data

6. Verify mount:
   df -h
