# bytemancy 0 - Easy - picoCTF 2026

```python
mauf0xxy-picoctf@webshell:~$ cat app.py
while(True):
try:
print('⊹──────[ BYTEMANCY-0 ]──────⊹')
print("☍⟐☉⟊☽☈⟁⧋⟡☍⟐☉⟊☽☈⟁⧋⟡☍⟐☉⟊☽☈⟁⧋⟡☍⟐")
print()
print('Send me ASCII DECIMAL 101, 101, 101, side-by-side, no space.')
print()
print("☍⟐☉⟊☽☈⟁⧋⟡☍⟐☉⟊☽☈⟁⧋⟡☍⟐☉⟊☽☈⟁⧋⟡☍⟐")
print('⊹─────────────⟡─────────────⊹')
user_input = input('==> ')
if user_input == "\x65\x65\x65":
print(open("./flag.txt", "r").read())
break
else:
print("That wasn't it. I got: " + str(user_input))
print()
print()
print()
except Exception as e:
print(e)
break

mauf0xxy-picoctf@webshell:~$ python app.py
⊹──────[ BYTEMANCY-0 ]──────⊹
☍⟐☉⟊☽☈⟁⧋⟡☍⟐☉⟊☽☈⟁⧋⟡☍⟐☉⟊☽☈⟁⧋⟡☍⟐

Send me ASCII DECIMAL 101, 101, 101, side-by-side, no space.

☍⟐☉⟊☽☈⟁⧋⟡☍⟐☉⟊☽☈⟁⧋⟡☍⟐☉⟊☽☈⟁⧋⟡☍⟐
⊹─────────────⟡─────────────⊹
==> eee
```

---

`picoCTF{pr1n74813_ch4r5_[REDACTED]}`