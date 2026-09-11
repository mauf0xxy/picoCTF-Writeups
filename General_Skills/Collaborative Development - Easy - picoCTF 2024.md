# Collaborative Development - Easy - picoCTF 2024

```markdown
mauf0xxy-academy@webshell:~/drop-in$ git log
commit 2258a0f267d57e8b6025e2a020b77fac7a553c92 (main)
Author: picoCTF <ops@picoctf.com>
Date:   Tue Mar 12 00:07:54 2024 +0000

    init flag printer
    
mauf0xxy-academy@webshell:~/drop-in$ git branch -a  
  feature/part-1
  feature/part-2
  feature/part-3
* main

mauf0xxy-academy@webshell:~/drop-in$ git checkout feature/part-1
Switched to branch 'feature/part-1'

mauf0xxy-academy@webshell:~/drop-in$ ls -la
total 4
drwxr-xr-x 3 mauf0xxy-academy mauf0xxy-academy  33 Jul 17 12:29 .
drwxr-xr-x 5 mauf0xxy-academy mauf0xxy-academy 192 Jul 17 12:26 ..
drwxr-xr-x 8 mauf0xxy-academy mauf0xxy-academy 166 Jul 17 12:29 .git
-rw-rw-r-- 1 mauf0xxy-academy mauf0xxy-academy  64 Jul 17 12:29 flag.py

mauf0xxy-academy@webshell:~/drop-in$ python3 flag.py 
Printing the flag...
picoCTF{t3@mw0rk_

mauf0xxy-academy@webshell:~/drop-in$ git checkout feature/part-2
Switched to branch 'feature/part-2'

mauf0xxy-academy@webshell:~/drop-in$ python3 flag.py 
Printing the flag...
m@k3s_th3_dr3@m_

mauf0xxy-academy@webshell:~/drop-in$ git checkout feature/part-3
Switched to branch 'feature/part-3'

mauf0xxy-academy@webshell:~/drop-in$ python3 flag.py 
Printing the flag...
w0rk_[REDACTED]}
```

---

`picoCTF{t3@mw0rk_m@k3s_th3_dr3@m_w0rk_[REDACTED]}`