# Mastering Linux Fundamentals – TryHackMe Notes  
This document contains detailed explanations, real command examples, and practical breakdowns of Mastering Linux Fundamentals Part 1–3 from TryHackMe.

📌PART 1 — Introduction to Linux & Basic Commands

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



