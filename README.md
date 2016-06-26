# Codebreaker #

##Introduction
Welcome to Codebreaker! This project was completed as part of a basic C++ programming course.

![alt text](http://i.imgur.com/9WxVzoD.jpg)

##Instructions
The object of this game is to guess the *secret* code in the **fewest** guesses possible. The secret code is randomly generated by the RNG in the program. (insert link to line of code that has random number generator) By default, the secret code is four digits long and the range of digits allowed is 0 through 6. Both of these variables can be changed in the main file. A larger number of digits or a wider range of digits increases difficulty. (move this?)

![alt text](http://i.imgur.com/AJRivym.jpg)

The player's input shows to the right of the "Enter Code:" text. After the user makes a guess, the computer displays the guess in the "YOUR GUESSES" collumn. The collumn under "CORRECT" displays the number of digits that are correct **AND** in their correct spots. The collumn under "MISPLACED" shows the number of digits that are correct but are **NOT** in their correct positions.

##Gameplay

![alt text](http://i.imgur.com/zm1LqLd.jpg)

In this example, the player's first guess is "1234". This yields 0 correct and 2 misplaced. This means that two of the digits from the input are in the secret code, but are not in the correct position. 

![alt text](http://i.imgur.com/sIfAFtM.jpg)

The player swaps the 1 for a 2 and guesses "2234". This yields 1 correct and 0 misplaced. The only digit that was changed was the first one, so having 1 more correct digit means that the changed digit is the correct one. The player can safely assume that the first digit is a "2".

Furthermore, having 0 misplaced after this guess means that the player can also assume that "1" is in the secret code. If "1" was not in the secret code, the number of misplaced would have instead gone from 2 to 1 because the "2" was put in its correct position. "1" was the only digit that was changed.
