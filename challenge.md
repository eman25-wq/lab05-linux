LAB 05 - LINUX SECURITY DETECTIVE CHALLENGE

Q1. What is your username and home directory?
Command: whoami
Command: echo ~
Answer: My username is eman25-wq.
My home directory is /home/eman25-wq.

Q2. What is your hostname and Ubuntu version?
Command: hostname
Command: cat /etc/os-release | head -2
Answer: My hostname is ubuntu.
My Ubuntu version is Ubuntu 26.04.1 LTS.

Q3. How much RAM and free disk space does your VM have?
Command: free -h
Command: df -h /
Answer: My VM has approximately 5.2 GiB RAM.
The available disk space was approximately 3.5 GB.

Q4. Which users have /bin/bash as their login shell?
Command: grep '/bin/bash$' /etc/passwd
Answer: This command lists users whose login shell is /bin/bash.

Q5. How many processes are running?
Command: ps aux | wc -l
Answer: The command returned 243 lines, including the header.
The process count can change over time.

Q6. How can you find when lab5user was created or deleted?
Command: sudo journalctl | grep lab5user
Answer: The system journal can show log entries related to
the creation, activity, and deletion of lab5user.
