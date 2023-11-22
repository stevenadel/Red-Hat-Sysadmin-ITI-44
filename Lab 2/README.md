# Lab 2
Users & groups

### 1. sudo useradd islam -c "Islam Askar"; sudo passwd islam
### 2. sudo useradd baduser -c "Bad User"; sudo passwd baduser
### 3. sudo groupadd pgroup -g 30000
### 4. sudo groupadd badgroup
### 5. sudo usermod islam -G pgroup -a
### 6. sudo passwd islam
### 7. sudo chage -E $(date -d +30days +%Y-%m-%d) islam
### 8. sudo usermod islam -L
### 9. sudo userdel -r baduser
### 10. sudo groupdel badgroup

## Screenshots
![Screenshot1](https://github.com/stevenadel/red-hat-sysadmin-iti-44/assets/111876286/ae97cb3f-6ea5-4796-b634-bf7fcd40a97d)
![Screenshot2](https://github.com/stevenadel/red-hat-sysadmin-iti-44/assets/111876286/2402d20e-d9cb-404e-b7c9-a9048f056486)

-------------------------------------------------------------------------------------------------------------------

# Lab 3

### 13. Create a folder called myteam in your home directory and change its permissions to read only for the owner.

### 14. Log out and log in by another user

### 15. Try to access (by cd command) the folder (myteam)

### 16. Using the command Line
#### a. Change the permissions of oldpasswd file to give owner read and write
#### b. permissions and for group write and execute and execute only for the others (using chmod in 2 different ways)
#### c. Change your default permissions to be as above.
#### d. What is the maximum permission a file can have, by default when it is just created? And what is that for directory.
#### e. Change your default permissions to be no permission to everyone then create a directory and a file to verify.

### 17. What are the minimum permission needed for:
#### a. Copy a directory (permission for source directory and permissions for target parent directory)
#### b. Copy a file (permission for source file and and permission for target parent directory)
#### c. Delete a file
#### d. Change to a directory
#### e. List a directory content (ls command)
#### f. View a file content (more/cat command)
#### g. Modify a file content

### 18. Create a file with permission 444. Try to edit in it and to remove it? Note what happened.

### 19. What is the difference between the “x” permission for a file and for a directory?
