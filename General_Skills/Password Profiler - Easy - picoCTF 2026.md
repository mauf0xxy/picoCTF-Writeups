# Password Profiler - Easy - picoCTF 2026

>[GitHub - Mebus/cupp: Common User Passwords Profiler (CUPP)](https://app.notion.com/p/Password-Profiler-Easy-picoCTF-2026-395955efbada802b9900fd4c8596c6de?source=copy_link#395955efbada80f395efe7a81a791bf7)

---

```bash
┌──(kali㉿kali)-[~/cylab]
└─$ ls 
check_password.py  hash.txt  passwords.txt  userinfo.txt

┌──(kali㉿kali)-[~/cylab]
└─$ cat userinfo.txt 
First Name: Alice
Surname: Johnson
Nickname: AJ
Birthdate: 15-07-1990
Partner's Name: Bob
Child's Name: Charlie

┌──(kali㉿kali)-[~/cylab]
└─$ cupp.py -i

┌──(kali㉿kali)-[~/cylab]
└─$ python3 check_password.py                          
Password found:
```

---

`picoCTF{Aj_[REDACTED]}`