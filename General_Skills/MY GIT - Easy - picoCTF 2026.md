# MY GIT - Easy - picoCTF 2026

```
┌──(kali㉿kali)-[~/cylab]
└─$ git clone ssh://git@foggy-cliff.picoctf.net:63899/git/challenge.git
Cloning into 'challenge'...
The authenticity of host '[foggy-cliff.picoctf.net]:63899 ([3.15.249.208]:63899)' can't be established.
ED25519 key fingerprint is: SHA256:Grm7IvZgdCDbXv3DtQ70/6WKHA2q3XhT+sfva8nLT38
This host key is known by the following other names/addresses:
    ~/.ssh/known_hosts:14: [hashed name]
Are you sure you want to continue connecting (yes/no/[fingerprint])? yes
Warning: Permanently added '[foggy-cliff.picoctf.net]:63899' (ED25519) to the list of known hosts.
** WARNING: connection is not using a post-quantum key exchange algorithm.
** This session may be vulnerable to "store now, decrypt later" attacks.
** The server may need to be upgraded. See https://openssh.com/pq.html
git@foggy-cliff.picoctf.net's password: 
remote: Enumerating objects: 3, done.
remote: Counting objects: 100% (3/3), done.
remote: Compressing objects: 100% (2/2), done.
remote: Total 3 (delta 0), reused 0 (delta 0)
Receiving objects: 100% (3/3), done.

┌──(kali㉿kali)-[~/cylab]
└─$ cd challenge
                                                                              
┌──(kali㉿kali)-[~/cylab/challenge]
└─$ git config --global user.name "root"                               
                                                                              
┌──(kali㉿kali)-[~/cylab/challenge]
└─$ git config --global user.email "root@picoctf"                                                                            
                                                                                                                                                                                                                                                                                               
┌──(kali㉿kali)-[~/cylab/challenge]
└─$ git config list
user.name=root
user.email=root@picoctf
core.repositoryformatversion=0
core.filemode=true
core.bare=false
core.logallrefupdates=true
remote.origin.url=ssh://git@foggy-cliff.picoctf.net:63899/git/challenge.git
remote.origin.fetch=+refs/heads/*:refs/remotes/origin/*
branch.master.remote=origin
branch.master.merge=refs/heads/master
                                                                              
┌──(kali㉿kali)-[~/cylab/challenge]
└─$ echo "request flag" > flag.txt   
                                                                              
┌──(kali㉿kali)-[~/cylab/challenge]
└─$ git add flag.txt                 
                                                                              
┌──(kali㉿kali)-[~/cylab/challenge]
└─$ git commit -m "push flag as root"
[master 13545f0] push flag as root
 1 file changed, 1 insertion(+)
 create mode 100644 flag.txt
                                                                              
┌──(kali㉿kali)-[~/cylab/challenge]
└─$ git branch                       
* master
                                                                              
┌──(kali㉿kali)-[~/cylab/challenge]
└─$ git push origin master
** WARNING: connection is not using a post-quantum key exchange algorithm.
** This session may be vulnerable to "store now, decrypt later" attacks.
** The server may need to be upgraded. See https://openssh.com/pq.html
git@foggy-cliff.picoctf.net's password: 
Enumerating objects: 4, done.
Counting objects: 100% (4/4), done.
Delta compression using up to 8 threads
Compressing objects: 100% (2/2), done.
Writing objects: 100% (3/3), 280 bytes | 280.00 KiB/s, done.
Total 3 (delta 0), reused 0 (delta 0), pack-reused 0 (from 0)
remote: Author matched and flag.txt found in commit...
remote: Congratulations! You have successfully impersonated the root user
remote: Here's your flag: picoCTF{1mp3rs0n4t4_g17_345y_[REDACTED]}
To ssh://foggy-cliff.picoctf.net:63899/git/challenge.git
   088b58f..13545f0  master -> master
```

---

`picoCTF{1mp3rs0n4t4_g17_345y_[REDACTED]}`