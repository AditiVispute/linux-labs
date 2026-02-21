# Linux File Permission Commands (Practical)

This section includes basic commands used to manage file and directory permissions in Linux.

---

## chmod

 Use:
  The chmod command is used to change the permission settings of a file or directory.

 Command:
  ```bash
  chmod 777 file1.txt

 Sample Output:
  Permissions changed successfully

 This gives read, write and execute permissions to all users.

## Types of Permissions 

  r → Read permission

  w → Write permission

  x → Execute permission

Numeric Representation:
  Number	Permission
  4	Read
  2	Write
  1	Execute

Example:
 Command:
  chmod 755 test.sh

Explanation:

  Owner has read, write and execute permission.

  Group has read and execute permission.

  Others have read and execute permission.

## chown
Use:
  The chown command is used to change the ownership of a file or directory.

Command:
  chown user file1.txt

Sample Output:
  Ownership changed successfully

Used to assign ownership of files to a specific user.
