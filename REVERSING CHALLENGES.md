- Challenge 1:
  Challenge description:
  <br>
  Finding out the hidden flag within the file
  </br>
  My Approach:
  <br>
  I extracted all the strings from tryme file using the 'strings' command. That's where I ran into this:
  ![image](https://github.com/bhavisan/PHASE-2-CHALLENGES/assets/155368794/6d832ce4-7a76-4ded-adb9-55cc30e127b9)
  This is what I found when I ran the executable file:
  ![image](https://github.com/bhavisan/PHASE-2-CHALLENGES/assets/155368794/956e9056-92dc-4320-bd9e-07d7cca07b88)

I figured the sup3r_s3cr3t_k3y_1337 had something to do with finding the flag. However:
![image](https://github.com/bhavisan/PHASE-2-CHALLENGES/assets/155368794/7645d629-9536-4a15-b80d-00b115d140c5)
what I got wasn't the correct flag. Hence I decided to go straight to the source code. For this, I used GHYDRA. Here is the code I obtained:
![image](https://github.com/bhavisan/PHASE-2-CHALLENGES/assets/155368794/cffb777d-6a95-4e47-876d-c5d934b67bf6)
Analysing the code made me realise that the code intended the user to first subtract 34 from the char of the letters in sup3r_s3cr3t_k3y_1337. Then we find the XOR of the result with the following values:
![image](https://github.com/bhavisan/PHASE-2-CHALLENGES/assets/155368794/3bd0c423-2311-4dfb-a8f3-e04d242514b6)
(I have converted the first two into decimal in the image)

Here's an excel sheet of all the above operations:
![image](https://github.com/bhavisan/PHASE-2-CHALLENGES/assets/155368794/c6578c6e-9791-459e-8e30-25bcd538a59d)
![image](https://github.com/bhavisan/PHASE-2-CHALLENGES/assets/155368794/af6611bc-e933-4740-8ea4-059482710bdc)
This led me to my flag.
![image](https://github.com/bhavisan/PHASE-2-CHALLENGES/assets/155368794/d58aa93d-9730-4397-83f0-ad71acf2a52f)

FLAG: _y0u_f0und_key_

- Challenge 2:
  <br>
  Challenge description: To figure out what's within the PYC file and find the flag.
  </br>

  My Approach:
  <br>
  A PYC file is basically compiled python code into bytecode.

- Challenge 3:
  <br>
  Challenge Description: to find the password
  </br>

  My Approach:
  ![image](https://github.com/bhavisan/PHASE-2-CHALLENGES/assets/155368794/c3a4988c-064d-43b1-8881-ae527facdbb7)
In this task as well, I used GHYDRA to decompile the given file and obtain the source code.
![image](https://github.com/bhavisan/PHASE-2-CHALLENGES/assets/155368794/81e298a4-ee5d-40bc-a15d-85118338feb0)
Analyzing the code gave me the flag:
![image](https://github.com/bhavisan/PHASE-2-CHALLENGES/assets/155368794/5b9f3784-af50-42a9-8012-ecb0c282521e)

FLAG: at_least_this_cafe_wont_leak_your_credit_card_numbers

- Challenge 4:
   <br>
   Challenge Description: to find the password
  </br>

  My Approach:
  ![image](https://github.com/bhavisan/PHASE-2-CHALLENGES/assets/155368794/f81b6567-cebd-4942-86c4-297f3e52fea2)
 This was yet another task that asked for password, so I did the usual and looked for the source code using GHIDRA.
![image](https://github.com/bhavisan/PHASE-2-CHALLENGES/assets/155368794/9b9788dd-ce3a-4695-8083-0ee5a0dc7c9a)

Analysing the source code, I was able to figure out the flag.
![image](https://github.com/bhavisan/PHASE-2-CHALLENGES/assets/155368794/d6ce3c21-56b8-40be-8c95-f10483f5ff41)

FLAG: pass@words (any 10 letter word as long as the 4th index is @)

for instance:
![image](https://github.com/bhavisan/PHASE-2-CHALLENGES/assets/155368794/93a77b87-444a-4279-b642-1fe2de4ade70)

