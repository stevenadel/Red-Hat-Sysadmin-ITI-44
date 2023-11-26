# Lab 5

### 1. Compress a file by compress, gzip, zip commands and decompress it again. State the differences between compress and gzip commands.
compress -v file\
uncompress file.Z\
gzip file\
gunzip file.gz\
zip file.zip file\
unzip file.zip
### 2. What is the command used to view the content of a compressed file.
zcat file.zip
### 3. Backup /etc directory using tar utility.
tar cvf etc.tar /etc
### 4. Starting from your home directory, find all files that were modified in the last two day.
find ~ -mtime -2
### 5. Starting from /etc, find files owned by root user.
find /etc -user root
### 6. Find all directories in your home directory.
find ~ -type d
### 7. Write a command to search for all files on the system that, its name is “.profile”.
locate .profile
### 8. Identify the file types of the following: /etc/passwd, /dev/pts/0, /etc, /dev/sda
file /etc/passwd\
file /dev/pts/0\
file /etc\
file /dev/sda
### 9. List the inode numbers of /, /etc, /etc/hosts.
ls -id /\
ls -id /etc\
ls -id /etc/hosts
### 10. Copy /etc/passwd to your home directory, use the commands diff and cmp, and Edit in the file you copied, and then use these commands again, and check the output.
cp /etc/passwd ~\
diff passwd /etc/passwd\
cmp passwd /etc/passwd
### 11. Create a symbolic link of /etc/passwd in /boot.
cd /boot\
sudo ln -s /etc/passwd
### 12. Create a hard link of /etc/passwd in /boot. Could you? Why?
cd /boot\
sudo ln /etc/passwd\
(ln: failed to create hard link './passwd' => '/etc/passwd': Invalid cross-device link)

## Screenshots
![Screenshot from 2023-11-26 15-19-45](https://github.com/stevenadel/Red-Hat-Sysadmin-ITI-44/assets/111876286/1989cd1a-18f1-4cc6-bd9b-3f6ac335dd8b)
![Screenshot from 2023-11-26 15-16-24](https://github.com/stevenadel/Red-Hat-Sysadmin-ITI-44/assets/111876286/72fe807a-e6a4-41f4-8f29-72c60b92acce)
![Screenshot from 2023-11-26 15-15-27](https://github.com/stevenadel/Red-Hat-Sysadmin-ITI-44/assets/111876286/d83dde9c-6ba7-45cc-9086-8975da823d7a)
![Screenshot from 2023-11-26 15-09-11](https://github.com/stevenadel/Red-Hat-Sysadmin-ITI-44/assets/111876286/9317a622-ce23-49b7-bb26-c62fa739f855)
![Screenshot from 2023-11-26 15-06-36](https://github.com/stevenadel/Red-Hat-Sysadmin-ITI-44/assets/111876286/d411e323-c889-4f3b-8bdf-9cd41dd31848)
![Screenshot from 2023-11-26 15-03-08](https://github.com/stevenadel/Red-Hat-Sysadmin-ITI-44/assets/111876286/719f3808-8c71-449d-88e1-a14f232bd8c5)
![Screenshot from 2023-11-26 14-34-38](https://github.com/stevenadel/Red-Hat-Sysadmin-ITI-44/assets/111876286/5cf06bbf-a733-4ca1-bde2-a1d0aee6bc7b)
![Screenshot from 2023-11-26 14-23-30](https://github.com/stevenadel/Red-Hat-Sysadmin-ITI-44/assets/111876286/fb329587-d3b2-45ec-9332-dc573aecfd51)
![Screenshot from 2023-11-26 14-23-09](https://github.com/stevenadel/Red-Hat-Sysadmin-ITI-44/assets/111876286/4a5b90a3-325a-4ea7-ab1d-ee5c4dd025a6)
![Screenshot from 2023-11-26 14-02-01](https://github.com/stevenadel/Red-Hat-Sysadmin-ITI-44/assets/111876286/b7840b2b-807e-4f97-af50-e7130e6e3457)
![Screenshot from 2023-11-26 13-54-21](https://github.com/stevenadel/Red-Hat-Sysadmin-ITI-44/assets/111876286/3ff14af5-d43a-4b04-afbe-f41b000415f2)
![Screenshot from 2023-11-26 13-52-09](https://github.com/stevenadel/Red-Hat-Sysadmin-ITI-44/assets/111876286/c4424f10-470d-4363-a449-c3509b71494f)
