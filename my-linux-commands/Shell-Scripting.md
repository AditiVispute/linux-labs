# Linux Shell Scripting

## 1. What is Shell Scripting?

Shell scripting is used to automate tasks in Linux using a sequence of commands written in a file.

---

## 2. Basic Script Structure

Create a script file:

touch script.sh

Add this:

#!/bin/bash
echo "Hello Cloud Engineer"

Make it executable:

chmod +x script.sh

Run script:

./script.sh

---

## 3. Variables

#!/bin/bash
name="Aditi"
echo "Hello $name"

---

## 4. User Input

#!/bin/bash
echo "Enter your name:"
read name
echo "Welcome $name"

---

## 5. If-Else Condition

#!/bin/bash
echo "Enter a number:"
read num

if [ $num -gt 10 ]
then
  echo "Number is greater than 10"
else
  echo "Number is 10 or less"
fi

---

## 6. For Loop

#!/bin/bash

for i in 1 2 3 4 5
do
  echo "Number: $i"
done

---

## 7. While Loop

#!/bin/bash

count=1

while [ $count -le 5 ]
do
  echo "Count: $count"
  ((count++))
done

---

## 8. Simple Automation Script (User Creation)

#!/bin/bash

echo "Enter username:"
read username

sudo useradd $username
echo "User $username created successfully"

---

## 9. Backup Script Example

#!/bin/bash

source_dir="/home/user"
backup_dir="/home/user/backup"

mkdir -p $backup_dir
cp -r $source_dir/* $backup_dir/

echo "Backup completed"

---

# Practical Lab

1. Create script:
   nano test.sh

2. Add code:
   #!/bin/bash
   echo "Linux Practice"

3. Make executable:
   chmod +x test.sh

4. Run script:
   ./test.sh
