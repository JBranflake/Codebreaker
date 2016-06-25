# Codebreaker #

##Introduction
Welcome to Codebreaker! This project was completed as part of a basic C++ programming course.

![alt text](http://i.imgur.com/9WxVzoD.jpg)

##Instructions
The object of this game is to guess the *secret* code in the **fewest** guesses possible. The secret code is randomly generated by the RNG in the program. (insert link to line of code that has random number generator) By default, the secret code is four digits long and the range of digits allowed is 0 through 6. Both of these variables can be changed in the main file. A longer span of digits or a wider range of digits increases difficulty. (move this?)

![alt text](http://i.imgur.com/AJRivym.jpg)

The player's input shows to the right of the "Enter Code:" text. After the user makes a first guess, the computer displays the guesses under the "YOUR GUESSES" text. Under "CORRECT", the computer displays the number of digits that are the correct digit **AND** are in the correct spots. Below "MISPLACED", the computer shows the number of digits that are the correct digits but are **NOT** in the correct positions.

![alt text](http://i.imgur.com/zm1LqLd.jpg)

In this example, the input "1234" yields 0 correct and 2 misplaced. This means that two of the digits from the input are in the secret code, but not in the right position. 
