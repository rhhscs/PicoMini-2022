# HashingJobApp
Tags: General Skills, hashing, nc, shell, python  
Author: LT 'syreal' Jones
## Description
If you want to hash with the best, beat this test!  
`nc saturn.picoctf.net 64710`
## Hints
1. You can use a commandline tool or web app to hash text
1. Press Ctrl and c on your keyboard to close your connection and return to the command prompt.
## Approach
Open terminal and connect to the server with `nc saturn.picoctf.net 64710`  
[MD5 hashing](https://en.wikipedia.org/wiki/MD5) is a method of generating a 32 character long sequence of hexadecimal characters based on some math. We don't care too much about the details and there are already [online hash generating tools](https://www.md5hashgenerator.com/)
```
Please md5 hash the text between quotes, excluding the quotes: 'hair transplants'
Answer:
5b416c0db26c7e0478766fc51931a3ab
5b416c0db26c7e0478766fc51931a3ab
Correct.
Please md5 hash the text between quotes, excluding the quotes: 'bad dogs'
Answer:
60cc96ffdc458c98395d6e7b6878a6e9
60cc96ffdc458c98395d6e7b6878a6e9
Correct.
Please md5 hash the text between quotes, excluding the quotes: 'Japanese'
Answer:
f32ced6a9ba164c4b3c047fd1d7c882e
f32ced6a9ba164c4b3c047fd1d7c882e
Correct.
picoCTF{4ppl1c4710n_r3c31v3d_91ab255f}
```
## Flag
picoCTF{4ppl1c4710n_r3c31v3d_91ab255f}