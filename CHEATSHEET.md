```md
# 🐧 Linux Commands Cheatsheet — Beginner Friendly

This cheatsheet gives you clean Linux commands with simple explanations and real sample outputs.

---

# 📍 1. BASIC COMMANDS

## pwd — show current directory
```
┌─(sambath@linux)-[~]
└─$ pwd
/home/sambath
```

## ls — list files
```
┌─(sambath@linux)-[~]
└─$ ls
notes.txt  pictures  downloads
```

## ls -la — show hidden files
```
┌─(sambath@linux)-[~]
└─$ ls -la
drwxr-xr-x  3 sambath sambath 4096 Jan 10 .
drwxr-xr-x 25 sambath sambath 4096 Jan 10 ..
-rw-r--r--  1 sambath sambath  220 Jan 10 .bashrc
```

## cd — change directory
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

## touch — create file
```
┌─(sambath@linux)-[~]
└─$ touch file.txt
```

## mkdir — create folder
```
┌─(sambath@linux)-[~]
└─$ mkdir projects
```

## cp — copy file
```
┌─(sambath@linux)-[~]
└─$ cp file.txt backup.txt
```

## mv — rename / move
```
┌─(sambath@linux)-[~]
└─$ mv file.txt notes.txt
```

## rm — delete file
```
┌─(sambath@linux)-[~]
└─$ rm notes.txt
```

---

# 🧑‍💻 3. USER INFORMATION COMMANDS

## who
```
┌─(sambath@linux)-[~]
└─$ who
sambath :0 2025-03-21 10:32 (:0)
```

## whoami
```
┌─(sambath@linux)-[~]
└─$ whoami
sambath
```

## id
```
┌─(sambath@linux)-[~]
└─$ id
uid=1000(sambath) gid=1000(sambath) groups=1000(sambath),27(sudo)
```

## groups
```
┌─(sambath@linux)-[~]
└─$ groups
sambath : sambath sudo
```

## grep user
```
┌─(sambath@linux)-[~]
└─$ grep -i sambath /etc/passwd
sambath:x:1000:1000::/home/sambath:/bin/bash
```

---

# 🌐 4. NETWORK COMMANDS

## ping
```
┌─(sambath@linux)-[~]
└─$ ping -c 2 google.com
64 bytes from 142.250.xx.xx: icmp_seq=1 ttl=118 time=23 ms
```

## ip a — show IP info
```
┌─(sambath@linux)-[~]
└─$ ip a
3: wlp3s0: <UP,RUNNING>
    inet 192.168.1.12/24
```

## curl — check server
```
┌─(sambath@linux)-[~]
└─$ curl -I https://example.com
HTTP/1.1 200 OK
```

---

# ⚙️ 5. PROCESS COMMANDS

## top — live monitoring
```
┌─(sambath@linux)-[~]
└─$ top
```

## ps aux — show processes
```
┌─(sambath@linux)-[~]
└─$ ps aux | head
root 1 0.0 0.1 168376 ? Ss init
```

---

# 🔐 6. PERMISSIONS

## chmod — give execute permission
```
┌─(sambath@linux)-[~]
└─$ chmod +x script.sh
```

## chown — change ownership
```
┌─(sambath@linux)-[~]
└─$ sudo chown sambath:sambath file.txt
```

---

# 🗃️ 7. ARCHIVE COMMANDS

## Create tar.gz
```
┌─(sambath@linux)-[~]
└─$ tar -czvf backup.tar.gz projects/
```

## Extract tar.gz
```
┌─(sambath@linux)-[~]
└─$ tar -xzvf backup.tar.gz
```

---

# ⌨️ SHORTCUTS

- Ctrl + C — stop  
- Ctrl + R — search history  
- !! — repeat last command  
- Tab — autocomplete  

```
