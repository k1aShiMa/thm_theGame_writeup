# thm_theGame_writeup
I've made my first writeup of my CTF journey. This CTF ain't that hard, you can do it in like 3 steps.

* **Where to find the room?:**
  * https://tryhackme.com/room/hfb1thegame

**The 3 steps you need:**
1. Initial Analysis
2. Static Analysis of Binary
3. Extracting the Flag

---

## Initial Analysis

* First things first I've downloaded the game file to crack it and unzipped it

![alt text](image.png)


## Static Analysis of Binary

* I've tried to list the strings in the "Tetrix.exe" file. Since the environment is Linux-based, I used native tools to analyze the Windows binary.

 ![alt text](image-1.png)

* As you can see there're strings in this file.

* **Commands:** *strings Tetrix.exe*

---

## Extracting the Flag

* Basically I just tried to filter the findings to strings that has "THM{" . If you ran everything right, the flag'll pop up like a cop on the highway
![alt text](image-2.png)

* **Commands:** *strings Tetrix.exe | grep -a "THM{"*

---

### Happy hacking folks!

#### Gabor "k1aShiMa" Sill
---
