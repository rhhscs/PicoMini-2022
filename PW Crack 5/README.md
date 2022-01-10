# PW Crack 5
Tags: General Skills, password_cracking, hashing  
Author: LT 'syreal' Jones
## Description
Can you crack the password to get the flag?  
Download the password checker [here](./level5.py) and you'll need the encrypted [flag](./level5.flag.txt.enc) and the [hash](./level5.hash.bin) in the same directory too. Here's a [dictionary](./dictionary.txt) with all possible passwords based on the password conventions we've seen so far.
## Hints
1. Opening a file in Python is crucial to using the provided dictionary.
1. You may need to trim the whitespace from the dictionary word before hashing. Look up the Python string function, `strip`
1. The `str_xor` function does not need to be reverse engineered for this challenge.
## Approach
This is pretty similar to [PW Crack 4](../PW%20Crack%204/)
```python
import hashlib
def hash_pw(pw_str):
    pw_bytes = bytearray()
    pw_bytes.extend(pw_str.encode())
    m = hashlib.md5()
    m.update(pw_bytes)
    return m.digest()
correct_pw_hash = open('level5.hash.bin', 'rb').read()

dictionary = open("dictionary.txt", "r").readlines()
for word in dictionary:
    word = word.strip()
    if hash_pw(word) == correct_pw_hash:
        print(word)
```
The first bit is the same, just change "level4.hash.bin" to "level5.hash.bin".  
The next bit reads the entire dictionary's lines, then loops through each word in the dictionary. There might be [trailing whitespaces](https://stackoverflow.com/questions/21410075/what-is-trailing-whitespace-and-how-can-i-handle-this) which is bad because the whitespace would be hashed too so to deal with this, we'll strip the word of whitespaces. [`strip`](https://docs.python.org/3/library/stdtypes.html#str.strip) removes trailing whitespaces. Then we just check to see if the hashed word is the same as the correct hashed password and if so, print the word.  
Run [`level5.py`](./level5.py) with the password obtained from the script.
## Flag
picoCTF{h45h_sl1ng1ng_36e992a6}