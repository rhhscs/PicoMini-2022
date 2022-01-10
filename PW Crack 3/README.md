# PW Crack 3
Tags: General Skills, password_cracking, hashing  
Author: LT 'syreal' Jones
## Description
Can you crack the password to get the flag?  
Download the password checker [here](./level3.py) and you'll need the encrypted [flag](./level3.flag.txt.enc) and the [hash](./level3.hash.bin) in the same directory too.  
There are 7 potential passwords with 1 being correct. You can find these by examining the password checker script.
## Hints
1. To view the level3.hash.bin file in the webshell, do: `$ bvi level3.hash.bin`
1. To exit `bvi` type `:q` and press enter.
1. The `str_xor` function does not need to be reverse engineered for this challenge.
## Approach
There's not really any way to reverse a hash so our best option is actually to just run the file with each of the passwords on line 44 until we get the flag from one of them.
## Flag
picoCTF{m45h_fl1ng1ng_64840799}