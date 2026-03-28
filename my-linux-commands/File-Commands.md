# Linux File & Directory Commands

## 1. ls
List files and directories.

ls
ls -l
ls -a

---

## 2. pwd
Print current working directory.

pwd

---

## 3. cd
Change directory.

cd /home
cd ..
cd ~

---

## 4. mkdir
Create a new directory.

mkdir mydir

Create multiple directories:
mkdir dir1 dir2 dir3

---

## 5. rmdir
Remove empty directory.

rmdir mydir

---

## 6. touch
Create empty file.

touch file.txt

Create multiple files:
touch file1.txt file2.txt

---

## 7. cp
Copy files and directories.

cp file1.txt file2.txt

Copy directory:
cp -r dir1 dir2

---

## 8. mv
Move or rename files.

Rename file:
mv old.txt new.txt

Move file:
mv file.txt /home/user/

---

## 9. rm
Remove files and directories.

Delete file:
rm file.txt

Delete directory:
rm -r dir1

Force delete:
rm -rf dir1

---

## 10. find
Search for files and directories.

find . -name "file.txt"

---

## 11. locate
Find files quickly (if installed).

locate file.txt

---

## 12. cat
Display file content.

cat file.txt

---

## 13. less
View file content page by page.

less file.txt

---

## 14. head
Show first lines of file.

head file.txt

---

## 15. tail
Show last lines of file.

tail file.txt

---

# Practical Lab

1. Create directory:
   mkdir practice

2. Go inside:
   cd practice

3. Create files:
   touch file1.txt file2.txt

4. Copy file:
   cp file1.txt copy.txt

5. Rename file:
   mv copy.txt newfile.txt

6. List files:
   ls -l

7. Delete file:
   rm newfile.txt

8. Go back:
   cd ..
