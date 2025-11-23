# 🐧 Linux Commands Cheatsheet — Beginner Friendly

This cheatsheet contains the essential Linux commands you will use daily.  
Each command includes a simple explanation and real example output.

---

# 📍 1. BASIC COMMANDS

## 📌 `pwd` — Show current directory
```
┌─(sambath@linux)-[~]
└─$ pwd
/home/sambath
```

## 📌 `ls` — List files
```
┌─(sambath@linux)-[~]
└─$ ls
notes.txt  pictures  downloads
```

## 📌 `ls -la` — Show hidden files
```
┌─(sambath@linux)-[~]
└─$ ls -la
drwxr-xr-x  3 sambath sambath 4096 Jan 10 .
drwxr-xr-x 25 sambath sambath 4096 Jan 10 ..
-rw-r--r--  1 sambath sambath 220 Jan 10 .bashrc
```

## 📌 `cd` — Change directory
```
┌─(sambath@linux)-[~]
└─$ cd Downloads
```

```
┌─(sambath@linux)-[~/Downloads]
└─$ pwd
/home/sambath/Downloads
```

---

# 📁 2. FILE & FOLDER COMMANDS

## 📌 Create file
```
┌─(sambath@linux)-[~]
└─$ touch file.txt
```

## 📌 Create folder
```
┌─(sambath@linux)-[~]
└─$ mkdir projects
```

## 📌 Copy file
```
┌─(sambath@linux)-[~]
└─$ cp file.txt backup.txt
```

## 📌 Rename / Move file
```
┌─(sambath@linux)-[~]
└─$ mv file.txt notes.txt
```

## 📌 Delete file
```
┌─(sambath@linux)-[~]
└─$ rm notes.txt
```

---

# 🧑‍💻 3. USER INFORMATION COMMANDS

## 📌 `who`
```
┌─(sambath@linux)-[~]
└─$ who
sambath :0 2025-03-21 10:32 (:0)
```

## 📌 `whoami`
```
┌─(sambath@linux)-[~]
└─$ whoami
sambath
```

## 📌 `id`
```
┌─(sambath@linux)-[~]
└─$ id
uid=1000(sambath) gid=1000(sambath) groups=1000(sambath),27(sudo)
```

## 📌 `groups`
```
┌─(sambath@linux)-[~]
└─$ groups
sambath : sambath sudo
```

## 📌 `grep user`
```
┌─(sambath@linux)-[~]
└─$ grep -i sambath /etc/passwd
sambath:x:1000:1000::/home/sambath:/bin/bash
```

---

# 🌐 4. NETWORK COMMANDS

## 📌 Ping
```
┌─(sambath@linux)-[~]
└─$ ping -c 2 google.com
64 bytes from 142.250.xx.xx: icmp_seq=1 ttl=118 time=23 ms
```

## 📌 Show IP
```
┌─(sambath@linux)-[~]
└─$ ip a
3: wlp3s0: <UP,RUNNING>
    inet 192.168.1.12/24
```

## 📌 Curl headers
```
┌─(sambath@linux)-[~]
└─$ curl -I https://example.com
HTTP/1.1 200 OK
```

---

# ⚙️ 5. PROCESS COMMANDS

## 📌 top — Live processes
```
┌─(sambath@linux)-[~]
└─$ top
```

## 📌 ps aux
```
┌─(sambath@linux)-[~]
└─$ ps aux | head
root 1 0.0 0.1 168376 ? Ss init
```

---

# 🔐 6. PERMISSIONS

## 📌 chmod
```
┌─(sambath@linux)-[~]
└─$ chmod +x script.sh
```

## 📌 chown
```
┌─(sambath@linux)-[~]
└─$ sudo chown
