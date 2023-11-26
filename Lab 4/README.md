# Lab 4

### 1. List the user commands and redirect the output to /tmp/commands.list
ls /usr/bin/ > /tmp/commands.list
### 2. Count the number of user commands
wc -w /tmp/commands.list
### 3. Get all the users names whose first character in their login is ‘g’.
cat /tmp/commands.list | grep ^g
### 4. Get the logins name and full names (comment) of logins starts with “g”.
cut -f1,5 -d: /etc/passwd | grep ^g
### 5. Save the output of the last command sorted by their full names in a file.
cut -f1,5 -d: /etc/passwd | grep ^g | sort -t : -k2 -o sorted_users
### 6. Write two commands: first: to search for all files on the system that named .bash_profile. Second: sorts the output of ls command on / recursively, Saving their output and error in 2 different files and sending them to the background.
find / -name .bash_profile\
ls -R / > output 2> errors
### 7. Display the number of users who is logged now to the system.
who | wc -l
### 8. Display lines 7 to line 10 of /etc/passwd file
head /etc/passwd | tail -4
### 9. What happens if you execute:
#### a. cat filename1 | cat filename2
only second file is printed
#### b. ls | rm
rm: missing operand
#### c. ls /etc/passwd | wc –l
wc: –l: No such file or directory
### 10.Issue the command sleep 100.
sleep 100
### 11.Stop the last command.
kill -STOP %1
### 12. Resume the last command in the background
bg %1
### 13. Issue the jobs command and see its output.
jobs
### 14. Send the sleep command to the foreground and send it again to the background.
fg %1 (then ctrl+z)
### 15. Kill the sleep command.
kill %1
### 16. Display your processes only
ps -u
### 17. Display all processes except yours
ps -U user -N
### 18. Use the pgrep command to list your processes only
pgrep -lu username
### 19. Kill your processes only.
pkill -U uid

## Screenshots
![Screenshot from 2023-11-25 13-51-22](https://github.com/stevenadel/Red-Hat-Sysadmin-ITI-44/assets/111876286/f2e6f078-23c8-439d-ab05-4294473341fe)
![Screenshot from 2023-11-25 13-52-49](https://github.com/stevenadel/Red-Hat-Sysadmin-ITI-44/assets/111876286/81dd4279-9f4f-4bd8-97ec-6a235e8a2a8a)
![Screenshot from 2023-11-25 23-57-22](https://github.com/stevenadel/Red-Hat-Sysadmin-ITI-44/assets/111876286/fdd7b307-1ace-4f88-bce2-0dcc1d339727)
![Screenshot from 2023-11-26 00-04-47](https://github.com/stevenadel/Red-Hat-Sysadmin-ITI-44/assets/111876286/44e70c5d-3c88-44fd-ad1f-1c4465c6295d)
![Screenshot from 2023-11-26 06-52-21](https://github.com/stevenadel/Red-Hat-Sysadmin-ITI-44/assets/111876286/e7498cbf-ff18-4522-a02d-b026c3e3f3ba)
![Screenshot from 2023-11-26 06-56-59](https://github.com/stevenadel/Red-Hat-Sysadmin-ITI-44/assets/111876286/bd0ad11e-873b-4448-b0d4-cff665f2a4f4)
![Screenshot from 2023-11-26 07-04-15](https://github.com/stevenadel/Red-Hat-Sysadmin-ITI-44/assets/111876286/96496456-6ce1-4973-8190-aac7f36af7d4)
![Screenshot from 2023-11-26 07-10-28](https://github.com/stevenadel/Red-Hat-Sysadmin-ITI-44/assets/111876286/8d0d7521-e619-4a60-b325-fc70129212ec)
![Screenshot from 2023-11-26 07-06-48](https://github.com/stevenadel/Red-Hat-Sysadmin-ITI-44/assets/111876286/a17771e6-4894-42aa-9323-c31a16c1c951)
