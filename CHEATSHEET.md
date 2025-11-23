```md
# 🐧 Linux Commands Cheatsheet — Human Friendly (With Parrot OS Output)

---

# 📍 1. BASIC COMMANDS

## ➤ pwd
```
┌─(sambath@parrot)-[~]
└─$ pwd
/home/sambath
```

## ➤ ls
```
┌─(sambath@parrot)-[~]
└─$ ls
notes.txt  pictures  downloads
```

## ➤ ls -la
```
┌─(sambath@parrot)-[~]
└─$ ls -la
drwxr-xr-x  3 sambath sambath 4096 Jan 10 .
drwxr-xr-x 25 sambath sambath 4096 Jan 10 ..
-rw-r--r--  1 sambath sambath  220 Jan 10 .bashrc
```

## ➤ cd
```
┌─(sambath@parrot)-[~]
└─$ cd Downloads
```
```
┌─(sambath@parrot)-[~/Downloads]
└─$ pwd
/home/sambath/Downloads
```

---

# 📁 2. FILE & FOLDER COMMANDS

## touch
```
┌─(sambath@parrot)-[~]
└─$ touch file.txt
```

## mkdir
```
┌─(sambath@parrot)-[~]
└─$ mkdir projects
```

## cp
```
┌─(sambath@parrot)-[~]
└─$ cp file.txt copy.txt
```

## mv
```
┌─(sambath@parrot)-[~]
└─$ mv file.txt notes.txt
```

## rm
```
┌─(sambath@parrot)-[~]
└─$ rm notes.txt
```

---

# 🧑‍💻 3. USER INFORMATION COMMANDS

## who
```
┌─(sambath@parrot)-[~]
└─$ who
sambath :0 2025-03-21 10:32 (:0)
```

## whoami
```
┌─(sambath@parrot)-[~]
└─$ whoami
sambath
```

## id
```
┌─(sambath@parrot)-[~]
└─$ id
uid=1000(sambath) gid=1000(sambath) groups=1000(sambath),27(sudo)
```

## groups
```
┌─(sambath@parrot)-[~]
└─$ groups
sambath : sambath sudo
```

## grep user
```
┌─(sambath@parrot)-[~]
└─$ grep -i sambath /etc/passwd
sambath:x:1000:1000::/home/sambath:/bin/bash
```

---

# 🌐 4. NETWORK COMMANDS

## ping
```
┌─(sambath@parrot)-[~]
└─$ ping -c 2 google.com
64 bytes from 142.250.xx.xx: icmp_seq=1 ttl=118 time=23 ms
```

## ip a
```
┌─(sambath@parrot)-[~]
└─$ ip a
3: wlp3s0: <UP,RUNNING>
    inet 192.168.1.12/24
```

## curl -I
```
┌─(sambath@parrot)-[~]
└─$ curl -I https://example.com
HTTP/1.1 200 OK
```

---

# ⚙️ 5. PROCESSES

## top
```
┌─(sambath@parrot)-[~]
└─$ top
```

## ps aux | head
```
┌─(sambath@parrot)-[~]
└─$ ps aux | head
root 1 0.0 0.1 168376 ? Ss init
```

---

# 🔐 6. PERMISSIONS

## chmod
```
┌─(sambath@parrot)-[~]
└─$ chmod +x script.sh
```

## chown
```
┌─(sambath@parrot)-[~]
└─$ sudo chown sambath:sambath file.txt
```

---

# 🗃️ 7. ARCHIVE

## tar create
```
┌─(sambath@parrot)-[~]
└─$ tar -czvf backup.tar.gz projects/
```

## tar extract
```
┌─(sambath@parrot)-[~]
└─$ tar -xzvf backup.tar.gz
```

```
```

