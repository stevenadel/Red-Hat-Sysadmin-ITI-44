# Lab 3

### 1. Using vi write your CV in the file mycv. Your CV should include your name, age, school, college, experience,...
vi mycv
### 2. Open mycv file using vi command then: Without using arrows state how to:
#### a. Move the cursor down one line at time.
Press j (in Command Mode)
#### b. Move the cursor up one line at time.
Press k (in Command Mode)
#### c. Search for word age
/age (Execute Mode)
#### d. Step to line 5 (assuming that you are in line 1 and file is more than 5 lines).
:5 (Execute Mode)
#### e. Delete the line you are on and line 5.
To delete only the line you are on -> dd\
to delete from your line (for example 3) to line 5 -> :3,5d
#### f. How to step to the end of line and change to writing mode in one-step.
Press A (in Command Mode)
### 3. List the available shells in your system.
cat /etc/shells\
(sh, bash and zsh)
### 4. List the environment variables in your current shell.
printenv
### 5. List all of the environment variables for the bash shell.
set (also includes local variables in shell)
### 6. What are the commands that list the value of a specific variable?
echo $VARIABLE_NAME
### 7. Display your current shell name.
echo $SHELL
### 8. State the initialization files of: sh, ksh, bash.
For Bash:
/etc/profile, /etc/bashrc (global)\
~/.profile, ~/.bash_profile
### 9. Edit in your profile to display date at login and change your prompt permanently.
in ~/.profile: PS1="\D{%d-%m-%Y} >>"
### 10.Execute the following command :
#### echo \ then press enter
echo \
#### What is the purpose of \ ?
enters second prompt
#### Notice the prompt ”>” what is that? and how can you change it from “>” to “:”
PS2=":"
### 11.Create a Bash shell alias named ls for the “ls –l” command
alias ls="ls -l"

## Screenshots
![Screenshot from 2023-11-23 04-23-06](https://github.com/stevenadel/red-hat-sysadmin-iti-44/assets/111876286/3ccd81bf-152e-4ecf-b786-b03bc0ffe629)
![Screenshot from 2023-11-23 04-22-08](https://github.com/stevenadel/red-hat-sysadmin-iti-44/assets/111876286/11e5666e-e7db-4c8b-82a2-2da81a888147)
![Screenshot from 2023-11-23 04-18-38](https://github.com/stevenadel/red-hat-sysadmin-iti-44/assets/111876286/2fd48b22-a6e1-4530-81eb-ea5f17fa9bee)
![Screenshot from 2023-11-23 04-06-17](https://github.com/stevenadel/red-hat-sysadmin-iti-44/assets/111876286/14b52db6-9d05-4967-87da-bfcb4a8951b4)
![Screenshot from 2023-11-23 04-00-10](https://github.com/stevenadel/red-hat-sysadmin-iti-44/assets/111876286/cf4e43b3-0726-417c-9285-11335574aa0c)
![Screenshot from 2023-11-23 03-57-48](https://github.com/stevenadel/red-hat-sysadmin-iti-44/assets/111876286/59ae530c-2a41-4d27-bff2-fdeb204cba44)
![Screenshot from 2023-11-23 03-57-00](https://github.com/stevenadel/red-hat-sysadmin-iti-44/assets/111876286/516b3938-eb2d-4760-bf64-d6456212d807)
![Screenshot from 2023-11-23 03-56-54](https://github.com/stevenadel/red-hat-sysadmin-iti-44/assets/111876286/7a23514e-0214-4cd4-a63a-3fa94670529d)
![Screenshot from 2023-11-23 03-41-39](https://github.com/stevenadel/red-hat-sysadmin-iti-44/assets/111876286/d764d46b-91ac-4832-bd2a-4097a4525ad8)



