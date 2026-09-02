# Printer Shares - Easy - picoCTF 2026

```
mauf0xxy-picoctf@webshell:~$ nc -vz mysterious-sea.picoctf.net 64218
Connection to mysterious-sea.picoctf.net (3.130.79.223) 64218 port [tcp/*] succeeded!

mauf0xxy-picoctf@webshell:~$ smbclient //3.130.79.223/shares -p 64218 -N
Try "help" to get a list of possible commands.
smb: \> ls
.                                   D        0  Fri Mar  6 20:25:44 2026
..                                  D        0  Fri Mar  6 20:25:44 2026
dummy.txt                           N     1142  Wed Feb  4 21:22:17 2026
flag.txt                            N       37  Fri Mar  6 20:25:44 2026
65536 blocks of size 1024. 60156 blocks available

smb: \> more flag.txt
```

---

`picoCTF{5mb_pr1nter_5h4re5_[REDACTED]}`