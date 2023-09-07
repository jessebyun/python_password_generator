<p align="center">
  <img src="https://i.imgur.com/HDtcLAz.png" alt="header_image"/>
</p>

<h2>Password Generator</h2>

This password generator will ask the user specifically the number of letters, number of symbols, and the number of numbers as the input for a random password. 

<h3>Code structure</h3>

I created 3 lists where the program can randomly choose characters from according to user input:
>letters = ['a', 'b', 'c', 'd', 'e', 'f', 'g', 'h', 'i', 'j', 'k', 'l', 'm', 'n', 'o', 'p', 'q', 'r', 's', 't', 'u', 'v', 'w', 'x', 'y', 'z', 'A', 'B', 'C', 'D', 'E', 'F', 'G', 'H', 'I', 'J', 'K', 'L', 'M', 'N', 'O', 'P', 'Q', 'R', 'S', 'T', 'U', 'V', 'W', 'X', 'Y', 'Z'] </br>
>numbers = ['0', '1', '2', '3', '4', '5', '6', '7', '8', '9']</br>
>symbols = ['!', '@', '#', '$', '%', '^', '&', '(', ')', '*', '+']</br>

First I created a function to get user input on the number of characters user wants to use for the password. This function serves to catch invalid user inputs. I would ask the user series of 3 questions on the number of characters from each category: letters, symbols, and numbers. With each question it would call up the said function to get that user input. If input is valid, it passes that value into a variable which will later be used in a range function. If input is invalid such as a negative number or something other than a number, it would loop the question until a valid input is entered. 

Next, I used a for-loop with a range function with variable from user input as the parameter (number of characters), and with each iteration of the loop, the computer would choose a random character from the list until it met user requirements on the length (range). Each time the computer chose a random character, it was added to a running list (password list). This loop was used for each question, for the number of letters, symbols, and numbers. Once computer randomly chose all the characters for the password then the list was complete.

Next, I used the shuffle function to scramble the password list. Generally, on a list each item is separated by commas, and for this list each character is its' own item . To combine all the characters of the password list into a single string, I used another for-loop to pass each character from the list onto a string variable. Finally, I displayed the string (password) onto the consol for the user to view.  
