# Glitch Cat
Tags: General Skills, nc, shell, Python   
Author: LT 'syreal' Jones
## Description
Our flag printing service has started glitching!  
`$ nc saturn.picoctf.net 50562`
## Hints
1. ASCII is one of the most common encodings used in programming
1. We know that the glitch output is valid Python, somehow!
1. Press Ctrl and c on your keyboard to close your connection and return to the command prompt.
## Approach
If we open Terminal and connect with `nc saturn.picoctf.net 50562` (input that line) then we get an output:
```
'picoCTF{gl17ch_m3_n07_' + chr(0x38) + chr(0x39) + chr(0x38) + chr(0x61) + chr(0x33) + chr(0x66) + chr(0x61) + chr(0x36) + '}'
```
In [Python, `chr` is a command](https://docs.python.org/3/library/functions.html#chr) that turns numbers into characters. [ASCII](https://en.wikipedia.org/wiki/ASCII) is a type of number to character and character to number encoding. If we run
```python
print('picoCTF{gl17ch_m3_n07_' + chr(0x38) + chr(0x39) + chr(0x38) + chr(0x61) + chr(0x33) + chr(0x66) + chr(0x61) + chr(0x36) + '}')
```
in the Python shell or as a new Python file and it should output the flag.
## Flag
picoCTF{gl17ch_m3_n07_898a3fa6}