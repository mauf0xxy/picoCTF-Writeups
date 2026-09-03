# Piece by Piece - Easy - picoCTF 2026

```bash
ctf-player@pico-chall$ cat part_* > flag.zip
ctf-player@pico-chall$ cat instructions.txt 
Hint:

- The flag is split into multiple parts as a zipped file.
- Use Linux commands to combine the parts into one file.
- The zip file is password protected. Use this "supersecret" password to extract the zip file.
- After unzipping, check the extracted text file for the flag.

ctf-player@pico-chall$ unzip flag.zip 
Archive:  flag.zip
[flag.zip] flag.txt password: 
 extracting: flag.txt
                 
ctf-player@pico-chall$ cat 
.cache/           flag.zip          part_ab           part_ae
.profile          instructions.txt  part_ac           
flag.txt          part_aa           part_ad           

ctf-player@pico-chall$ cat 
.cache/           flag.zip          part_ab           part_ae
.profile          instructions.txt  part_ac           
flag.txt          part_aa           part_ad           

ctf-player@pico-chall$ cat flag.txt
```

---

`picoCTF{z1p_and_spl1t_f1l3s_4r3_fun_[REDACTED]}`