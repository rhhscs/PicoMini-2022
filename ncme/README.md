# ncme
Tags: General Skills, nc  
Author: LT 'syreal' Jones
## Description
Connect to a remote computer using `nc` and get the flag.  
`$ nc saturn.picoctf.net 65317`
## Hints
1. If you don't know what netcat (nc) is, use the webshell to complete this problem. (It has `nc` installed already!)
1. Don't put the `$` in your command to connect to remote computer! That is meant to show that the command goes in the command prompt on the webshell.
1. Press Ctrl and c on your keyboard to close your connection and return to the command prompt.
## Approach
### Method 1: Using Pico Webshell
Open Pico's webshell
![webshell](./webshell.png), log in and input `nc saturn.picoctf.net 65317`
### Method 2: Mac/Linux
Open [Terminal](https://en.wikipedia.org/wiki/Terminal_(macOS)) and input `nc saturn.picoctf.net 65317`
### Method 3: Windows
Install [WSL](https://en.wikipedia.org/wiki/Windows_Subsystem_for_Linux) and any Linux flavor, (some tutorials can be found on [YouTube](https://www.youtube.com/watch?v=X-DHaQLrBi8)). Once installed, open WSL in a Linux tab and input `nc saturn.picoctf.net 65317`
## Flag
picoCTF{s4n1ty_c4t}