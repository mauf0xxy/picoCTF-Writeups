# Undo - Easy - picoCTF 2026

```
mauf0xxy-picoctf@webshell:~$ nc foggy-cliff.picoctf.net 53390
===Welcome to the Text Transformations Challenge!===

Your goal: step by step, recover the original flag.
At each step, you'll see the transformed flag and a hint.
Enter the correct Linux command to reverse the last transformation.

--- Step 1 ---
Current flag: KXA2OTgxcHBxLWZhMDFnQHplMHNmYTRlRy1nazNnLXRhMWZlcmlyRShTR1BicHZj
Hint: Base64 encoded the string.
Enter the Linux command to reverse it: base64 -d
Correct!
--- Step 2 ---
Current flag: )p6981ppq-fa01g@ze0sfa4eG-gk3g-ta1ferirE(SGPbpvc
Hint: Reversed the text.
Enter the Linux command to reverse it: rev
Correct!
--- Step 3 ---
Current flag: cvpbPGS(Eriref1at-g3kg-Ge4afs0ez@g10af-qpp1896p)
Hint: Replaced underscores with dashes.
Enter the Linux command to reverse it: tr '-' '_'
Correct!
--- Step 4 ---
Current flag: cvpbPGS(Eriref1at_g3kg_Ge4afs0ez@g10af_qpp1896p)
Hint: Replaced curly braces with parentheses.
Enter the Linux command to reverse it: tr '()' '{}'
Correct!
--- Step 5 ---
Current flag: cvpbPGS{Eriref1at_g3kg_Ge4afs0ez@g10af_qpp1896p}
Hint: Applied ROT13 to letters.

Enter the Linux command to reverse it: tr 'n-za-mN-ZA-M' 'a-zA-Z'
Correct!

Congratulations! You've recovered the original flag:
```

---

`picoCTF{Revers1ng_t3xt_Tr4nsf0rm@t10ns_[REDACTED]}`