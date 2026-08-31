# Static ain't always noise - Easy - picoCTF 2021

```bash
mauf0xxy-academy@webshell:~$ chmod +x ltdis.sh

mauf0xxy-academy@webshell:~$ ./ltdis.sh 
Attempting disassembly of  ...
objdump: 'a.out': No such file
objdump: section '.text' mentioned in a -j option, but not found in any input file
Disassembly failed!
Usage: ltdis.sh <program-file>
Bye!

mauf0xxy-academy@webshell:~$ ./ltdis.sh static 
Attempting disassembly of static ...
Disassembly successful! Available at: static.ltdis.x86_64.txt
Ripping strings from binary with file offsets...
Any strings found in static have been written to static.ltdis.strings.txt with file offset

mauf0xxy-academy@webshell:~$ cat static
static                    static.ltdis.strings.txt  static.ltdis.x86_64.txt   
mauf0xxy-academy@webshell:~$ cat static.ltdis.strings.txt | grep "pico"
   3020 picoCTF{d15a5m_t34s3r_[REDACTED]}
```

---

`picoCTF{d15a5m_t34s3r_[REDACTED]}`