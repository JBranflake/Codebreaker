![alt text](http://i.imgur.com/b6TzVuR.jpg)
___

##Introduction
Welcome to Codebreaker! The code for this project was written for a C++ programming course.

![alt text](http://i.imgur.com/9WxVzoD.jpg)

___

##Installation
Click [here](https://github.com/JBranflake/Codebreaker/archive/master.zip) to download the zip folder that contains the program files (if that does not work, click the "Clone or download" button and select the option "Download Zip"). Next, find the zip folder in your downloads folder. Unzip the folder to a convenient location. Finally, open the "main" file in a C++ IDE.

___

##Instructions
The object of this game is to guess the *secret* code in the **fewest** guesses possible. The secret code is generated by running a [random number generator](https://github.com/JBranflake/Codebreaker/blob/master/main.cpp#L151) through a [code generator](https://github.com/JBranflake/Codebreaker/blob/master/main.cpp#L139) function. By default, the secret code is four digits long and the range of digits allowed in the code are 0 through 6. 

![alt text](http://i.imgur.com/AJRivym.jpg)

The player's input shows to the right of the "Enter Code:" text. After the user makes a guess, the computer displays the guess in the "YOUR GUESSES" column. The column under "CORRECT" displays the number of digits that are correct **AND** in their correct spots. The column under "MISPLACED" shows the number of digits that are correct but are **NOT** in their correct positions.

___

##Example Gameplay

![alt text](http://i.imgur.com/zm1LqLd.jpg)

In this example, the player's first guess is "1234". This yields 0 correct and 2 misplaced. This means that two of the digits from the input are in the secret code, but are not in the correct position. 

![alt text](http://i.imgur.com/sIfAFtM.jpg)

The player swaps the 1 for a 2 and guesses "2234". This yields 1 correct and 0 misplaced. The only digit that was changed was the first one, so having 1 more correct digit means that the changed digit is the correct one. The player can safely assume that the first digit is a "2".

Furthermore, the player can assume that "1" is in the secret code because there are 0 misplaced digits. If "1" was not in the secret code, the number of misplaced would have instead gone from 2 to 1 because the "2" was put in its correct position.

![alt text](http://i.imgur.com/qrvRhZD.jpg?1)

The player guesses "2314" and confirms that the first digit is a "2". There is now 1 misplaced, so the "1" is not in the correct position. The "1" should either be in the second or fourth digit's place.

![alt text](http://i.imgur.com/xsgRKsO.jpg?1)

A guess of "2134" yields two correct! The player now knows that the second digit of the secret code is a "1". Since there are 0 misplaced digits, there is not a "3" or a "4" in the secret code.

![alt text](http://i.imgur.com/PrkpfRn.jpg)

How lucky! The player guesses "2165", which results in 2 misplaced. This means that the last two digits of the secret code are "5" and "6". The player simply has to swap the "6" and the "5".

![alt text](http://i.imgur.com/nO3Un6i.jpg)

Victory! The secret code was "2156".  The computer displays a congratulatory message and the number of guesses. The player is prompted to enter "Y" or "N" for playing another game. 

Note: *Most* games require more than 5 guesses.

___

##Customizations

The length and span of digits of the secret code can be changed in the ["main" file.] (https://github.com/JBranflake/Codebreaker/blob/master/main.cpp#L9) An increase in either of these adds difficulty. Here is a chart displaying various settings and their corresponding difficulties.

| Code Span | Code Length | Difficulty|
|-----------|------------|------------
| 4 digits  | 3 digits   | Easy       |
| 6 digits  | 4 digits   | Medium     |
| 8 digits  | 5 digits   | Hard       |
| 9 digits  | 6 digits   | EXTREME    |

___

##Acknowledgements

The professor of my C++ course provided the random number generator and player input functions for this assignment. I wrote the game logic, secret code generator, and header file. The title was made using a text-to-ASCII art generator found on  [this](http://patorjk.com/software/taag/#p=display&f=ANSI%20Shadow&t=Type%20Something%20) website.
