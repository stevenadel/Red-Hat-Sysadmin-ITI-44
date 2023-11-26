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
