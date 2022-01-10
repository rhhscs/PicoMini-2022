# PW Crack 1
Tags: General Skills, password_cracking  
Author: LT 'syreal' Jones
## Description
Can you crack the password to get the flag?  
Download the password checker [here](./level1.py) and you'll need the encrypted [flag](./level1.flag.txt.enc) in the same directory too.
## Hints
1. To view the file in the webshell, do: `$ nano level1.py`
1. To exit `nano`, press Ctrl and x and follow the on-screen prompts.
1. The `str_xor` function does not need to be reverse engineered for this challenge.
## Approach
If we take a look at the code, we'll notice [line 19](https://github.com/vivian-dai/PicoMini-2022/blob/main/PW%20Crack%201/level1.py#L19) is `if( user_pw == "17ac"):` which is checking to see if the password you inputted is "17ac". If the password you give is "17ac" then it outputs the flag.
```
Please enter correct password for flag: 17ac
Welcome back... your flag, user:
picoCTF{545h_r1ng1ng_7719ae74}
```
## Flag
picoCTF{545h_r1ng1ng_7719ae74}