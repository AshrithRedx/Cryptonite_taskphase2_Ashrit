**In this question, a function called checkPassword is contained which takes the input string Password as a parameter and converts it into a char array.**
**The character array is compared to a predefined string from varying positions (0-8, 31-17, and so on) and stored in specific locations within the char array.**
**The character array is finally reverted back to the string and compared to check the password.**

### Method:
1) Create a separate function and create a separate character array to store the characters.
2) Make the loop of size 32 and run the same loops through the string and assign characters to character array based on the indice postions mentioned in the loop.
3) Convert the character array into a string and print it out.
4) obtain the flag.
