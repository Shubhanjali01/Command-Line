<h1>CMD + PowerShell + VS Code</h1>


---

# 🚀 **VS CODE TERMINAL COMMANDS**

(These work *inside* VS Code terminal)

### **VS Code editor commands**

```
code .                     → Open current folder in VS Code
code <filename>            → Open specific file in VS Code
code ..                    → Open parent directory in VS Code
code --version
code --help
```

### **VS Code specific shortcuts (terminal related)**

```
Ctrl + `                   → Toggle terminal
Ctrl + Shift + `           → New terminal
Ctrl + Shift + C           → Copy path
Ctrl + Shift + P           → Command palette
```

---

# 🪟 **WINDOWS CMD — FULL COMMAND LIST (Developer Relevant)**

### 🔹 **File & Directory**

```
dir
dir /a
cd <folder>
cd ..
cd \
mkdir <folder>
rmdir <folder>
del <file>
copy <src> <dest>
move <src> <dest>
ren <old> <new>
type <file>
tree
cls
```

### 🔹 **System Info**

```
systeminfo
ipconfig
ipconfig /all
hostname
whoami
tasklist
taskkill /PID <id> /F
```

### 🔹 **Network**

```
ping <url>
tracert <url>
netstat -a
netstat -ano
curl <url>
```

### 🔹 **Utilities**

```
echo hello
echo %PATH%
set
setx
path
where <program>
color 0a
```

### 🔹 **Archive**

```
tar -xf file.tar
tar -xzf file.tar.gz
```

---

# ⚡ **POWERSHELL — FULL PROFESSIONAL COMMAND LIST**

### 🔹 **File & Directory**

```
Get-ChildItem            (ls)
Set-Location             (cd)
Get-Location             (pwd)
New-Item                 (create file)
New-Item -ItemType Directory
Remove-Item              (rm)
Copy-Item                (cp)
Move-Item                (mv)
Rename-Item              (ren)
Clear-Host               (clear)
```

### 🔹 **System**

```
Get-Process
Stop-Process -Id <pid>
Get-Service
Start-Service <name>
Restart-Service <name>
Get-History
Clear-History
```

### 🔹 **Network**

```
Test-Connection google.com   (like ping)
Invoke-WebRequest <url>      (curl)
Resolve-DnsName google.com   (nslookup)
Get-NetIPAddress
```

### 🔹 **Security**

```
Get-ExecutionPolicy
Set-ExecutionPolicy RemoteSigned
```

### 🔹 **Variables & Output**

```
$var = "hello"
Write-Output $var
Get-Content file.txt
Set-Content file.txt
Add-Content file.txt
```

### 🔹 **Package Manager (PowerShell 7+ / Win10+)**

```
winget search <app>
winget install <app>
winget upgrade
```

---


