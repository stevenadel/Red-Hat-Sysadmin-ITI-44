# Lab 6
### 1.	Use systemctl to view the status of all the system services.
```bash
systemctl status
```
![Screenshot from 2023-12-05 13-34-16](https://github.com/stevenadel/Red-Hat-Sysadmin-ITI-44/assets/111876286/0abda6fb-8038-4f06-8824-33b667b9b783)
### 2.	Change the default run level back to multi-user.target and reboot.
```bash

```
### 3.	Send mail to the root user.
```bash

```
### 4.	Verify that you have received this mail.
```bash

```
### 5.	Use  systemctl utility to stop postfix service
```bash

```
### 6.	Send mail again to the root user.
```bash

```
### 7.	Verify that you have received this mail.
```bash

```
### 8.	Use systemctl utility to start postfix service
```bash

```
### 9.	Verify that you have received this mail.
```bash

```
### 10.	Edit in the GRUB2 configuration file and change the timeout variable equal 20 seconds.
```bash

```
### 11.	 Edit in the GRUB2 configuration file and change your default operating system
```bash

```
### 12.	You want to know some information about the status of the system every ten minutes today between the hours of  8:00 AM and 5:00 PM. to help investigate some performance issues you have been having. You suspect it might be memory related and want to keep an eye on those resources.
```bash

```
### 13.	Use mail as the root user to check for e-mail from the cron jobs you have scheduled.
```bash

```
### 14.	How could you send the output from these cron jobs to another e-mail address (the manager user)?
```bash

```
### 15.	Use mail as the manager user to check for e-mail from the cron jobs you have scheduled.
```bash

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
17. Attempt to run the command gnuplot. You should find that it is not installed.
```bash

```
18. Search for the plotting packages.
```bash

```
19. Find out more information about the gunuplot package.
```bash

```
20. Install the gnuplot package.
```bash

```
21. Attempt to remove the gnuplot package, but say no. How many packages would be removed?
```bash

```
21. Attempt to remove the gunplot-common package but say no. How many packages would be removed?
```bash

```
## Using rpm
22. List all installed packages in your system.
```bash

```
23. View the files in the initscripts package
```bash

```
24. Get general information about bash rpm.
```bash

```
25. Have the files from the pam package changed since it was installed.
```bash

```
26. Which installed packages have gnome in their names?
```bash

```
27. Install any uninstalled package from RH Enterprise Linux cds
```bash

```
28. Search for software resemble the Photoshop software other than Gimp and install it.
```bash

```
30. Create the file /etc/yum.repos.d/cdrom.repo to enable install from
the iso from the iso of Red Hat.
31. Try to install any package from the new repository
