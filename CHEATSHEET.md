# 🐧 Linux Commands Cheatsheet — Beginner Friendly

This cheatsheet includes simple Linux commands with clear explanations and clean, copy-friendly examples.

---

# 📍 1. BASIC COMMANDS

## 📌 `pwd` — Show current directory
```
$ pwd
/home/user
```

## 📌 `ls` — List files
```
$ ls
file.txt  downloads  pictures
```

## 📌 `ls -la` — Show hidden files
```
$ ls -la
drwxr-xr-x  3 user user 4096 Jan 10 .
drwxr-xr-x 25 user user 4096 Jan 10 ..
-rw-r--r--  1 user user  220 Jan 10 .bashrc
```

## 📌 `cd` — Change directory
```
$ cd Downloads
```

---

# 📁 2. FILE & FOLDER COMMANDS

## Create file
```
$ touch file.txt
```

## Create folder
```
$ mkdir project
```

## Copy file
```
$ cp file.txt backup.txt
```

## Move / Rename
```
$ mv file.txt notes.txt
```

## Delete file
```
$ rm notes.txt
```

---

# 👤 3. USER INFORMATION COMMANDS

## who
```
$ who
user :0 2025-03-21 10:32 (:0)
```

## whoami
```
$ whoami
user
```

## id
```
$ id
uid=1000(user) gid=1000(user) groups=1000(user),27(sudo)
```

## groups
```
$ groups
user : user sudo
```

## grep user
```
$ grep -i user /etc/passwd
user:x:1000:1000::/home/user:/bin/bash
```

---

# 🌐 4. NETWORK COMMANDS

## Ping
```
$ ping -c 2 google.com
```

## Show IP
```
$ ip a
```

## Curl headers
```
$ curl -I https://example.com
```

---

# ⚙️ 5. PROCESS COMMANDS

## Show live processes
```
$ top
```

## Show running processes
```
$ ps aux
```

---

# 🔐 6. PERMISSIONS

## Make script executable
```
$ chmod +x script.sh
```

## Change file owner
```
$ sudo chown user:user file.txt
```

---

# 📦 7. ARCHIVE COMMANDS

## Create tar.gz
```
$ tar -czvf backup.tar.gz project/
```

## Extract tar.gz
```
$ tar -xzvf backup.tar.gz
```

---

# ⌨️ 8. SHORTCUTS

- Ctrl + C → stop command  
- Ctrl + R → search history  
- !! → repeat last command  
- Tab → autocomplete  
