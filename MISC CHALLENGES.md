# PHASE-2-CHALLENGES
This repository describes how I completed my tasks for phase 2, my approach and my final answer.
+ Challenge 1:
  <br>
![image](https://github.com/bhavisan/PHASE-2-CHALLENGES/assets/155368794/574e91d7-34b3-4ec7-b785-3e7635cb6f7a)
</br>
<br>
I used Linux terminal to extract the strings from the strings file after making it executable. The command I used is 'strings'. The above image displays the base64 encoded message at the very bottom. I was able to identify the base64 because of the '=' sign at the end. I used Notepad++ to decrypt my base64 message which revealed a link to a Github site to me. The link to the site is attached below.
</br>
https://gist.github.com/rSrikesh/ccbccc6222e857e426e53b2c7956be0a

I have attached the picture of the github repo below:
![image](https://github.com/bhavisan/PHASE-2-CHALLENGES/assets/155368794/813c6ed0-e8c0-4597-b50c-3cca3395e5f0)

Unfortunately, that's as far as I could go with this challenge. I wasn't able to decode then numbers and obtain the flag for this challenge.

- Challenge 2:
  I tried opening 'script' in linux terminal and realised that the game is supposed to be played with the help of pwn tools and a python code and not manually. Basically, I figured out what exactly the challenge meant when they said you will be doomed without pwntools. Then I studied about pwntools and started creating my python code in Notepad++. I used simple pwntools to create my python code. I have uploaded my python code below.

  ![image](https://github.com/bhavisan/PHASE-2-CHALLENGES/assets/155368794/df0c5577-6579-4d13-8a36-afe117c007c1)
![image](https://github.com/bhavisan/PHASE-2-CHALLENGES/assets/155368794/6e42a31c-0612-4ce3-bcee-072ca85f8cdd)
![image](https://github.com/bhavisan/PHASE-2-CHALLENGES/assets/155368794/cf1aa72b-ac00-407c-9927-f7df2b38ca91)
![image](https://github.com/bhavisan/PHASE-2-CHALLENGES/assets/155368794/27ba9a68-c19b-4f40-ac25-bb9460e048d5)

<br>
I ran python3 test.py in my linux terminal and obtained my flag. Here's the ss of my output:
</br>

![image](https://github.com/bhavisan/PHASE-2-CHALLENGES/assets/155368794/b6d3bec1-edf8-45ad-9e1d-f6c6dc9c8fcf).
![image](https://github.com/bhavisan/PHASE-2-CHALLENGES/assets/155368794/c1d573ca-18ee-49ce-ba73-36a1ecece0b2)
![image](https://github.com/bhavisan/PHASE-2-CHALLENGES/assets/155368794/b90f931d-e18f-465c-a89a-a72fc414e614)
![image](https://github.com/bhavisan/PHASE-2-CHALLENGES/assets/155368794/52847b02-b5f8-41a2-9dec-3692f3555181)

flag{y0u_4r3_g0d_5cr1pt3r_4f7f4a}

- Challenge 3:
  For the third challenge, after searching around a bit, I figured out that the symbols meant Wingding font. Then I decrypted the Wingding to obtain my flag.

  flag{72123dcea19936533e4525a2e15bad5c}

- Challenge 4:
  <br>
  The first thing I did was check if the encrypted text was in base64 by going to the end of file to look for a '='. Turns out, it was indeed encoded in base64. Then I simply opened the file in Notepad++ and decoded it around 25-30 times. I could see the number of lines reducing each time I decoded, sometimes rapidly and sometimes slowly. In the last decode, I got a python code.
  </br>

  ![image](https://github.com/bhavisan/PHASE-2-CHALLENGES/assets/155368794/487c74fd-b4ca-404a-88a7-64dd93027820)

<br>
I ran the above code in python and hence obtained my flag. 
</br>

flag{bd03dfff3f126aba0ae3756b464d106c}

- Challenge 5:
  As given in the hint, I checked the file type:
  ![image](https://github.com/bhavisan/PHASE-2-CHALLENGES/assets/155368794/304fa229-8125-447e-a1fe-bffcb901ee4f)
The file type said ASCII text with no line terminators, but I had it converted to simple ASCII text. Next, I used Notepad++ to convert the hex to ascii. This is what I obtained:
![image](https://github.com/bhavisan/PHASE-2-CHALLENGES/assets/155368794/e55b0d34-beba-45e0-a114-9f7fb6dfa81a)
I had no way to know if this was the flag, since the challenge mentioned I had to enclose the text I got in flag{}. I couldn't convert the text into anything meaningful either. Since there wasn't anything mentioned in the challenge or hint on the image of the flag,  I figured I got my answer. I understood as "special keyboard" mentioned in the chall desciption as a keyboard that converts whatever you type into hex format.



