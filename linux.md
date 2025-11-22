<h1> Linux Commands </h1>

# 🟢 **1. File & Directory Commands**

```
ls                # List files and folders
ls -l             # Detailed list
ls -a             # Show hidden files
pwd               # Show current directory
cd <folder>       # Change directory
cd ..             # Move one level up
cd ~              # Go to home directory
mkdir <name>      # Create folder
rmdir <name>      # Remove empty folder
rm <file>         # Delete file
rm -r <folder>    # Delete folder and contents
cp file1 file2    # Copy file
cp -r dir1 dir2   # Copy folder
mv old new        # Move/rename file or folder
touch file.txt    # Create empty file
cat file.txt      # Show file content
nano file.txt     # Edit file in terminal
```

---

# 🔵 **2. System Information**

```
uname -a          # Kernel and system info
hostname          # Show device name
whoami            # Current user
top               # Show running processes (like Task Manager)
htop              # Better process viewer (if installed)
df -h             # Disk usage
du -sh *          # Size of each file/folder
free -h           # RAM usage
uptime            # System uptime
```

---

# 🟣 **3. Package Management (Ubuntu/Debian)**

```
sudo apt update           # Refresh package list
sudo apt upgrade          # Update installed packages
sudo apt install <pkg>    # Install package
sudo apt remove <pkg>     # Remove package
sudo apt purge <pkg>      # Remove fully
```

---

# 🔶 **4. Permissions**

```
chmod 755 file           # Change file permission
chmod +x file            # Make file executable
chown user:group file    # Change owner
sudo su                  # Switch to root user
```

---

# 🔷 **5. Networking Commands**

```
ifconfig                 # Show network settings
ip a                     # Show IP addresses
ping google.com          # Check connection
curl <url>               # Make HTTP request
wget <url>               # Download file
ssh user@ip              # Connect to remote system
scp file user@ip:/path   # Copy file over SSH
```

---

# 🟡 **6. Searching & Finding**

```
find /path -name "file"   # Search by name
grep "text" file          # Search inside file
grep -r "text" folder     # Recursive search
```

---

# 🔘 **7. Archive & Compression**

```
tar -cvf file.tar folder      # Create tar
tar -xvf file.tar             # Extract tar
zip file.zip file             # Zip
unzip file.zip                # Unzip
```

---

# ⚫ **8. Process & Services**

```
ps aux                        # List processes
kill <pid>                    # Kill process
kill -9 <pid>                 # Force kill
systemctl status <service>    # Service status
systemctl start <service>
systemctl stop <service>
journalctl -xe                # System logs
```

---

# 🟤 **9. Git Shortcut (Linux)**

```
git init
git add .
git commit -m "msg"
git push
git pull
```

---

# 🟣 **10. Others**

```
history            # Show commands used
clear              # Clear terminal
alias ll="ls -l"   # Create shortcut
```

