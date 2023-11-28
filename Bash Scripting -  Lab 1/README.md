# Bash Lab 1
### Using sed utility
### 1- Display the lines that contain the word “lp” in /etc/passwd file.
sed -n '/lp/p' /etc/passwd

![1](https://github.com/stevenadel/Red-Hat-Sysadmin-ITI-44/assets/111876286/affc4a5f-3ebd-4815-9cbd-6b501724862b)

### 2- Display /etc/passwd file except the third line.
sed '3d' /etc/passwd

![2](https://github.com/stevenadel/Red-Hat-Sysadmin-ITI-44/assets/111876286/75235534-1839-4aea-b624-8ffc5b07a19d)

### 3- Display /etc/passwd file except the last line.
sed ‘$d’ myfile

![3](https://github.com/stevenadel/Red-Hat-Sysadmin-ITI-44/assets/111876286/60975b62-bef4-4e96-a291-3e2c34ec984a)

### 4- Display /etc/passwd file except the lines that contain the word “lp”.
sed '/lp/d' /etc/passwd

![4](https://github.com/stevenadel/Red-Hat-Sysadmin-ITI-44/assets/111876286/f29f1ced-7109-40a1-aed4-c0245dd260e2)

### 5- Substitute all the words that contain “lp” with “mylp” in /etc/passwd file.
sed 's/lp/mylp/g' /etc/passwd

![5](https://github.com/stevenadel/Red-Hat-Sysadmin-ITI-44/assets/111876286/ce9d2e10-a02f-486d-8570-2a2e12f6fb4b)

---------------------------------------------------------------------------------------

### Using awk utility
### 1- Print full name (comment) of all users in the system.
### 2- Print login, full name (comment) and home directory of all users.( Print each line preceded by a line number)
### 3- Print login, uid and full name (comment) of those uid is greater than 500
### 4- Print login, uid and full name (comment) of those uid is exactly 500
### 5- Print line from 5 to 15 from /etc/passwd
### 6- Change lp to mylp
### 7- Print all information about greatest uid.
### 8- Get the sum of all accounts id’s.


---------------------------------------------------------------------------------------

### Bonus
### 1. Get the sum of accounts id’s that has the same group.
### 2. Make the report:

