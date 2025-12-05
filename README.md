# Mastering Linux Fundamentals – TryHackMe Notes  
This document contains detailed explanations, real command examples, and practical breakdowns of Mastering Linux Fundamentals Part 1–3 from TryHackMe.

📌**PART 1 — Introduction to Linux & Basic Commands**

 1. What is Linux?
Linux is an open-source operating system widely used in servers, cybersecurity, development, embedded systems, and cloud environments.
It is known for security, stability, and flexibility.

It includes:
- **Kernel** – controls memory, CPU, processes.
- **Shell** – interprets commands (`bash`, `sh`, `zsh`).
- **Filesystem** – structured directory system starting at `/`.


2. Filesystem Structure with Examples

| Directory | Meaning | Example Usage |
|----------|---------|----------------|
| `/home` | Stores user folders | `/home/annon/docs` |
| `/etc` | Configuration files | `/etc/passwd` |
| `/var/log` | System logs | `/var/log/auth.log` |
| `/bin` | Basic commands | `/bin/ls` |
| `/root` | Root user home | `sudo su` → `cd /root` |


3. Basic Linux Commands
a) **pwd**
   Viewing your current directory

b) **ls**
    List files
    
 **ls -la**
 show all files with permissions

c) **cd**
  Changing directory e:g ( cd /home/user)
  **cd ..**     # go up one level
  **cd ~**       # go to home

d) **mkdir**
   creating directories
   **rmdir**
   removing directories

e) **touch**
   creating files (.txt)

f) **cat, less, head, tail**
    viewing file content

g) **nano**
   editing files with nano (nano script.sh)
   **CTRL + O** → Save
   **CTRL + X** → Exit

h) **find**
   Searching for files 

I) **uname -a, whoami, id, hostname**
   Getting System information



📌 **PART 2 — Permissions, Users, Groups & Processes**

1. File Permissions
 
Permission Breakdown

  **r** = read
  **w** = write
  **x** = execute

  a)**ls -l**
     View permissions

     **e:g**
     -rwxr-x---  1 annon admins 4096 script.sh
  
  b)**chmod**
     Change permissions

  c)**chown**
     Change Ownership
 

2. Managing Users & Groups

  a)  **sudo useradd john**\ Add a new user
      **sudo passwd john**/

  b) **sudo groupadd developers**
      Create a group

  c)**sudo usermod -aG developers john**
      Add user to group



3. Managing Processes
   a) **ps aux, top**
        View running processes

  b)**kill**
      Kill a process

 c) **env, echo, export**
      Environment Variables




📌 **PART 3 — File Operations, Networking, Services & Scripting**

1. File Manipulation
   
   a)**cp** 
        Copy file
   
   b)**mv**
       move file
   
   c)**rm** 
       remove file

   d)**tar**
      Archieve a file

   e)**gzip**
       compress a file



2. Networking in Linux
   
   a)**ip a**
      View IP address

   b)**ping 8.8.8.8**
     Test Connectivity

   c)**ss -tulnp**
     Check open ports

   d)**wget, curl**
     download files (e:g- wget http://example.com/file.txt, curl http://example.com)



4. Managing Services with Systemctl

   a) **Start / Stop / Restart / Enable**
      sudo systemctl start apache2
      sudo systemctl stop ssh
      sudo systemctl restart apache2
      sudo systemctl enable apache2
      sudo systemctl status ssh

   b)**Package Management**
      sudo apt update
      sudo apt install nmap
      sudo apt remove apache2



5. Cron Scheduling

   a)**crontab -e**
      Edit the cron table

   b) **Run a job every minute**
       * * * * echo "Hello World" >> /tmp/test.log
       



   
Summary Covered

✅ Linux navigation
✅ File creation, editing, and management
✅ Permissions, users, and groups
✅ Processes & system monitoring
✅ Network commands
✅ Services management
✅ Package installation
✅ Automation with cron



