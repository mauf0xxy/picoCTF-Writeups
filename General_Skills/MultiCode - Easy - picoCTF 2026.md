# MultiCode - Easy - picoCTF 2026

```bash
┌──(kali㉿kali)-[~]
└─$ cat message.txt 
NjM3NjcwNjI1MDQ3NTMyNTM3NDI2MTcyNjY2NzcyNzE1ZjcyNjE3MDMwNzE3NjYxNzQ1ZjM2MzY2ZjM1MzQzMjM1MzcyNTM3NDQ=
```

```bash
┌──(kali㉿kali)-[~]
└─$ echo "NjM3NjcwNjI1MDQ3NTMyNTM3NDI2MTcyNjY2NzcyNzE1ZjcyNjE3MDMwNzE3NjYxNzQ1ZjM2MzY2ZjM1MzQzMjM1MzcyNTM3NDQ=" | base64 -d
637670625047532537426172666772715f72617030717661745f36366f3534323537253744

┌──(kali㉿kali)-[~]
└─$ mauf0xxy-academy@webshell:~$ echo "637670625047532537426172666772715f72617030717661745f36366f3534323537253744" | xxd -r -p
cvpbPGS%7Barfgrq_rap0qvat_66o54257%7D

┌──(kali㉿kali)-[~]
└─$ php -r "echo urldecode('cvpbPGS%7Barfgrq_rap0qvat_66o54257%7D');"
cvpbPGS{arfgrq_rap0qvat_66o54257}

┌──(kali㉿kali)-[~]
└─$ echo "cvpbPGS{arfgrq_rap0qvat_66o54257}" | tr 'A-Za-z' 'N-ZA-Mn-za-m'
```

---

`picoCTF{nested_enc0ding_[REDACTED]}`