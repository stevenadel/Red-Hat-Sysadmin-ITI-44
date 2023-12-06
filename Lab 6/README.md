# Lab 6
### 1.	Use systemctl to view the status of all the system services.
```bash
systemctl status
```
![Screenshot from 2023-12-05 13-34-16](https://github.com/stevenadel/Red-Hat-Sysadmin-ITI-44/assets/111876286/0abda6fb-8038-4f06-8824-33b667b9b783)
### 2.	Change the default run level back to multi-user.target and reboot.
```bash
systemctl set-default multi-user.target
sudo shutdown -r 0
```
![Screenshot from 2023-12-05 13-34-51](https://github.com/stevenadel/Red-Hat-Sysadmin-ITI-44/assets/111876286/c7d83cfc-9830-404a-bda7-b8b55a99f682)
![Screenshot from 2023-12-05 13-36-21](https://github.com/stevenadel/Red-Hat-Sysadmin-ITI-44/assets/111876286/54ec3151-e371-4a7a-9070-9669a4261ac6)
### 3.	Send mail to the root user.
```bash
mail root
```
![Screenshot from 2023-12-05 14-11-02](https://github.com/stevenadel/Red-Hat-Sysadmin-ITI-44/assets/111876286/51a56cad-6e68-47a1-b1af-7185468adb25)
### 4.	Verify that you have received this mail.
```bash
su -
mail
```
![Screenshot from 2023-12-05 14-13-03](https://github.com/stevenadel/Red-Hat-Sysadmin-ITI-44/assets/111876286/bde9571f-5e64-4f48-9d22-33d1bd112efe)
### 5.	Use  systemctl utility to stop postfix service
```bash
systemctl stop postfix
```
![Screenshot from 2023-12-05 14-17-12](https://github.com/stevenadel/Red-Hat-Sysadmin-ITI-44/assets/111876286/e4d340ec-871e-49a9-b7ae-820905a5afda)
### 6.	Send mail again to the root user.
```bash
mail root
```
![Screenshot from 2023-12-05 14-22-31](https://github.com/stevenadel/Red-Hat-Sysadmin-ITI-44/assets/111876286/45c58270-4c30-4212-bab9-6d13e37a31a0)
### 7.	Verify that you have received this mail.
```bash
su -
mail
# second mail not received
```
![Screenshot from 2023-12-05 14-23-56](https://github.com/stevenadel/Red-Hat-Sysadmin-ITI-44/assets/111876286/b7ddff91-4c86-412d-80e7-279b772bbba5)
### 8.	Use systemctl utility to start postfix service
```bash
systemctl start postfix
```
![Screenshot from 2023-12-05 14-31-06](https://github.com/stevenadel/Red-Hat-Sysadmin-ITI-44/assets/111876286/a4d12eaf-bd32-433a-9625-fffeee7ced25)
### 9.	Verify that you have received this mail.
```bash
su -
mail
```
![Screenshot from 2023-12-05 14-33-04](https://github.com/stevenadel/Red-Hat-Sysadmin-ITI-44/assets/111876286/830d91d5-448b-4863-90a6-ecd813fe55d7)
### 10.	Edit in the GRUB2 configuration file and change the timeout variable equal 20 seconds.
```bash
sudo vim /etc/default/grub
sudo grub2-mkconfig
```
![Screenshot from 2023-12-05 14-37-50](https://github.com/stevenadel/Red-Hat-Sysadmin-ITI-44/assets/111876286/fc203bce-0619-41ea-b2cf-b285c716ba7c)
### 11.	 Edit in the GRUB2 configuration file and change your default operating system
```bash
sudo vim /etc/default/grub
cat /etc/default/grub    # changed to Windows, but don't worry won't leave it like this for long ;)
sudo grub2-mkconfig
```
![Screenshot from 2023-12-05 14-45-40](https://github.com/stevenadel/Red-Hat-Sysadmin-ITI-44/assets/111876286/f1b75f58-1046-4b01-a0a0-46638e433f66)
### 12.	You want to know some information about the status of the system every ten minutes today between the hours of  8:00 AM and 5:00 PM. to help investigate some performance issues you have been having. You suspect it might be memory related and want to keep an eye on those resources.
```bash
crontab -e
```
![Screenshot from 2023-12-05 15-16-17](https://github.com/stevenadel/Red-Hat-Sysadmin-ITI-44/assets/111876286/4b16e4e9-66d5-4b36-b164-27ed7676b735)
### 13.	Use mail as the root user to check for e-mail from the cron jobs you have scheduled.
```bash
su -
mail
```
![Screenshot from 2023-12-05 19-23-25](https://github.com/stevenadel/Red-Hat-Sysadmin-ITI-44/assets/111876286/28a61a16-6ca1-4671-bbfb-d0150b92d44c)
### 14.	How could you send the output from these cron jobs to another e-mail address (the manager user)?
```bash
crontab -e
#inside crontab -e add MAILTO=manager
```
![Screenshot from 2023-12-05 19-25-10](https://github.com/stevenadel/Red-Hat-Sysadmin-ITI-44/assets/111876286/f5522f3c-f992-425b-a295-57d5816de150)
### 15.	Use mail as the manager user to check for e-mail from the cron jobs you have scheduled.
```bash
su - manager
mail
```
### 16.	Bonus
```
Your boss thinks it’s a great idea to have one central logging server. Satisfy his requirements
Hint:
Set up rsyslogd on the "logging server" machine to accept logging messages from other machines.
On the your "workstation", set up rsyslogd to send messages to the "logging server
Test the new setup by using the logger command on the "workstation" to generate a log message
Does the message appear in the "logging server's" /var/log/messages file?
Why does this message also appear in the "workstation's" /var/log/messages file?
How could you have the message only appear in the "logging server's" files?
```
```bash

```
## Using yum
### 17. Attempt to run the command gnuplot. You should find that it is not installed.
```bash
gnuplot
```
![Screenshot from 2023-12-06 10-51-34](https://github.com/stevenadel/Red-Hat-Sysadmin-ITI-44/assets/111876286/d21ff1bd-59c9-4424-b61e-46b9cedcad98)
### 18. Search for the plotting packages.
```bash
yum search plot
```
![Screenshot from 2023-12-06 10-52-58](https://github.com/stevenadel/Red-Hat-Sysadmin-ITI-44/assets/111876286/8f1efad1-767f-4abf-a8c4-b56a89fe6ef2)
### 19. Find out more information about the gunuplot package.
```bash
yum info gnuplot
```
![Screenshot from 2023-12-06 11-07-32](https://github.com/stevenadel/Red-Hat-Sysadmin-ITI-44/assets/111876286/eed2a371-1239-4cce-9adc-854a0fe2b782)
### 20. Install the gnuplot package.
```bash
sudo yum install gnuplot
```
![Screenshot from 2023-12-06 11-09-20](https://github.com/stevenadel/Red-Hat-Sysadmin-ITI-44/assets/111876286/f41e026d-1bb9-45f7-8c0e-8cd4d60852ec)
### 21. Attempt to remove the gnuplot package, but say no. How many packages would be removed?
```bash
sudo yum remove gnuplot
# 4 packages to be removed
```
![Screenshot from 2023-12-06 09-11-29](https://github.com/stevenadel/Red-Hat-Sysadmin-ITI-44/assets/111876286/60be2932-6c37-4cf9-bb67-a2837bfd23d2)
### 21. Attempt to remove the gunplot-common package but say no. How many packages would be removed?
```bash
sudo yum remove gnuplot-common
# 4 packages to be removed
```
![Screenshot from 2023-12-06 09-13-03](https://github.com/stevenadel/Red-Hat-Sysadmin-ITI-44/assets/111876286/ad9a3b71-62aa-4de5-941e-9f08a561e408)

## Using rpm
### 22. List all installed packages in your system.
```bash
rpm -qa
```
![Screenshot from 2023-12-06 09-14-13](https://github.com/stevenadel/Red-Hat-Sysadmin-ITI-44/assets/111876286/d839dca7-09a1-4e3c-bcca-e1c44da30f70)
### 23. View the files in the initscripts package
```bash
rpm -ql initscripts
```
![Screenshot from 2023-12-06 09-19-55](https://github.com/stevenadel/Red-Hat-Sysadmin-ITI-44/assets/111876286/e3fd06f1-3cef-49e5-8cf4-2e4fb15a29db)
### 24. Get general information about bash rpm.
```bash
rpm -qi bash
```
![Screenshot from 2023-12-06 09-23-52](https://github.com/stevenadel/Red-Hat-Sysadmin-ITI-44/assets/111876286/419f1aa0-cad6-4e94-bbaf-4a38d23721a9)
### 25. Have the files from the pam package changed since it was installed.
```bash
rpm -V pam
```
![Screenshot from 2023-12-06 09-30-51](https://github.com/stevenadel/Red-Hat-Sysadmin-ITI-44/assets/111876286/6643aed7-d8a2-4889-a75d-f31b45e93170)
### 26. Which installed packages have gnome in their names?
```bash
rpm -qa | grep gnome
```
![Screenshot from 2023-12-06 09-39-36](https://github.com/stevenadel/Red-Hat-Sysadmin-ITI-44/assets/111876286/7e4293d6-99e2-4064-920a-568247a33adb)
