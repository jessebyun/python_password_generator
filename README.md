<p align="center">
  <img src="https://i.imgur.com/HDtcLAz.png" alt="header_image"/>
</p>

<h2>Password Generator</h2>

This password generator will create a random password using letters (upper and lower case), symbols, and numbers. The program will specifically ask the user the length of characters that the user wishes to use from each of the 3 categories.

<h3>Code structure</h3>

I created 3 lists where the program can randomly choose characters from:
>letters = ['a', 'b', 'c', 'd', 'e', 'f', 'g', 'h', 'i', 'j', 'k', 'l', 'm', 'n', 'o', 'p', 'q', 'r', 's', 't', 'u', 'v', 'w', 'x', 'y', 'z', 'A', 'B', 'C', 'D', 'E', 'F', 'G', 'H', 'I', 'J', 'K', 'L', 'M', 'N', 'O', 'P', 'Q', 'R', 'S', 'T', 'U', 'V', 'W', 'X', 'Y', 'Z'] </br>
>numbers = ['0', '1', '2', '3', '4', '5', '6', '7', '8', '9']</br>
>symbols = ['!', '@', '#', '$', '%', '^', '&', '(', ')', '*', '+']</br>

Next, I created a function which is called upon when asking the user the length of characters user wants from letters, from symbols, and finally from numbers. This function also serves to catch invalid inputs until a valid input is made. This input is passed into a variable which will later be used in a range function.

Next, I used a for-loop with a range function with the parameter from the user input variable (number of characters). With each iteration of the loop (each number in the range), the computer would choose a random character from the respective lists until it met user requirements on the length (range). Each time the computer chose a random character, it was added to a running list (password list). This loop was used for each question: the length of letters, length of symbols, and the length of numbers. Once computer randomly chose all the characters for the password, then the running lis was complete.

Next, I used the shuffle function to scramble the password list. On a list, each item is separated by commas. Therefore, in this list each character is its' own item . To combine all the characters of the password list into a single string, I used another for-loop to pass each character from the list onto a string variable. Finally, I displayed the string (password) onto the consol for the user to view.  
