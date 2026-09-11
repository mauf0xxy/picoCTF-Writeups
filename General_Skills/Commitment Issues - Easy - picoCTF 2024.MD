# Commitment Issues - Easy - picoCTF 2024

```markdown
mauf0xxy-academy@webshell:~/drop-in$ git log
commit a6dca68e4310585eac3b5c9caf0f75967dfe972c (HEAD -> master)
Author: picoCTF <ops@picoctf.com>
Date:   Sat Mar 9 21:10:06 2024 +0000

    remove sensitive info

commit e720dc26a1a55405fbdf4d338d465335c439fb3e
Author: picoCTF <ops@picoctf.com>
Date:   Sat Mar 9 21:10:06 2024 +0000

    create flag

commit e720dc26a1a55405fbdf4d338d465335c439fb3e
Author: picoCTF <ops@picoctf.com>
Date:   Sat Mar 9 21:10:06 2024 +0000

    create flag
    
mauf0xxy-academy@webshell:~/drop-in$ git show e720dc26a1a55405fbdf4d338d465335c439fb3e
diff --git a/message.txt b/message.txt
new file mode 100644
index 0000000..d263841
--- /dev/null
+++ b/message.txt
@@ -0,0 +1 @@
+picoCTF{s@n1t1z3_[REDACTED]}
```

---

`picoCTF{s@n1t1z3_[REDACTED]}`