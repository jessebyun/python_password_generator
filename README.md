<p align="center">
  <img src="" alt="header_image"/>
</p>

<h2>Password Generator</h2>

This password generator will ask the user specifically the number of letters, number of symbols, and the number of numbers as the input for a random password. 

<h3>Code structure</h3>

I created 3 lists where the program can randomly choose characters from according to user input:
>letters (lower-case, upper-case)</br>
>numbers</br>
>symbols</br>

Created an empty new list where I can append/ add the characters that the computer randomly chose into a running list. I used a for-loop with a range function and user input as a parameter, and ran it through each of the 3 lists. Everytime the computer chose a charcter from the list, it added it to the running list. Then I used a shuffle function on that password list. On this password list, each character is a separate item each divieed by commas. To combine all the characters of the password into a single string I needed to pass another for-loop to add each character to a string variable. 
