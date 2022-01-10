# PW Crack 2
Tags: General Skills, password_cracking  
Author: LT 'syreal' Jones
## Description
Can you crack the password to get the flag?  
Download the password checker [here](./level2.py) and you'll need the encrypted [flag](./level2.flag.txt.enc) in the same directory too.
## Hints
1. Does that encoding look familiar?
1. The `str_xor` function does not need to be reverse engineered for this challenge.
## Approach
When we look at [line 18](https://github.com/vivian-dai/PicoMini-2022/blob/main/PW%20Crack%202/level2.py#L18), we see `if( user_pw == chr(0x35) + chr(0x39) + chr(0x30) + chr(0x39) ):` and upon looking at hint 1, we can realize it should be the exact same encoding as the previous question, [Glitch Cat](../Glitch%20Cat/) We can now run
```python
print(chr(0x35) + chr(0x39) + chr(0x30) + chr(0x39))
```
in either the Python shell or a new Python file and this outputs "5909".  
The rest we can approach the same way as [PW Crack 1](../PW%20Crack%201/), make sure the files are in the same directory and run it, then input the password.
```
Please enter correct password for flag: 5909
Welcome back... your flag, user:
picoCTF{tr45h_51ng1ng_b0539d96}
```
## Flag
picoCTF{tr45h_51ng1ng_b0539d96}