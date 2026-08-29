# Wave a flag - Easy - picoCTF 2021

> Can you invoke help flags for a tool or binary? This program has extraordinarily helpful information...
> 

---

```
mauf0xxy-picoctf@webshell:~$ wget https://challenge-files.picoctf.net/c_wily_courier/89a0e56b3f2697fe5d597b2805202b86693dcb0e04aec062e11fe66edbbd04aa/warm
--2026-04-11 15:04:55--  https://challenge-files.picoctf.net/c_wily_courier/89a0e56b3f2697fe5d597b2805202b86693dcb0e04aec062e11fe66edbbd04aa/warm
Resolving challenge-files.picoctf.net (challenge-files.picoctf.net)... 3.160.5.40, 3.160.5.95, 3.160.5.18, ...
Connecting to challenge-files.picoctf.net (challenge-files.picoctf.net)|3.160.5.40|:443... connected.
HTTP request sent, awaiting response... 200 OK
Length: 19312 (19K) [application/octet-stream]
Saving to: 'warm'

warm                  100%[=======================>]  18.86K  --.-KB/s    in 0.005s

2026-04-11 15:04:55 (3.37 MB/s) - 'warm' saved [19312/19312]

maufoxy-picoctf@webshell:~$ chmod 777 warm
maufoxy-picoctf@webshell:~$ ./warm
Hello user! Pass me a -h to learn what I can do!
maufoxy-picoctf@webshell:~$ ./warm -h
Oh, help? I actually don't do much, but I do have this flag here:
```

---

`picoCTF{b1scu1ts_4nd_gr4vy_[REDACTED]}`