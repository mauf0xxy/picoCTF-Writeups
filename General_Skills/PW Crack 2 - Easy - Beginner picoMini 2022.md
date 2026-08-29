# PW Crack 2 - Easy - Beginner picoMini 2022

```python
mauf0xxy-picoctf@webshell:~$ cat level2.py

###THIS FUNCTION WILL NOT HELP YOU FIND THE FLAG --LT

def str_xor(secret, key):
#extend key to secret length
new_key = key
i = 0
while len(new_key) < len(secret):
new_key = new_key + key[i]
i = (i + 1) % len(key)

return "".join([chr(ord(secret_c) ^ ord(new_key_c)) for (secret_c,new_key_c) in zip(secret,new_key)])
###############################################################################

flag_enc = open('level2.flag.txt.enc', 'rb').read()

def level_2_pw_check():
user_pw = input("Please enter correct password for flag: ")
if( user_pw == chr(0x64) + chr(0x65) + chr(0x37) + chr(0x36) ):
print("Welcome back... your flag, user:")
decryption = str_xor(flag_enc.decode(), user_pw)
print(decryption)
return
print("That password is incorrect")

level_2_pw_check()
```

```
mauf0xxy-picoctf@webshell:~$ python
Python 3.10.12 (main, Mar  3 2026, 11:56:32) [GCC 11.4.0] on linux
Type "help", "copyright", "credits" or "license" for more information.
>>> print(chr(0x64) + chr(0x65) + chr(0x37) + chr(0x36))

mauf0xxy-picoctf@webshell:~$ python level2.py
Please enter correct password for flag: de76
Welcome back... your flag, user:
```

---

`picoCTF{tr45h_51ng1ng_[REDACTED]}`