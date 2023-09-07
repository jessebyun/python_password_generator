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

Created an empty new list where I can append/ add the characters that the computer randomly chose into a running list. I used a for-loop with a range function with user input as the parameter (for the number of characters to choose), and ran it through each of the 3 lists. Everytime the computer chose a charcter from the list, it added it to the running list. Then I used a shuffle function on that password list. On this password list, each character is a separate item and each is divieed by commas. To combine all the characters of the password into a single string I needed to pass another for-loop to add each character to a string variable. Finally I displayed the password on the consol for the user. 
