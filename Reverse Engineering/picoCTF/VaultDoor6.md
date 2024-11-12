**In this question, the checkPassword function initally checks whether the length of the string is 32.**
**It then then converts the password into a byte array and XOR's with a predefined hex value(0x55).**
**It then compares if the result is equal to a predefined byte array.**

### Method:
1) Create a new function which performs XOR and takes no parameters.
2) A^B= C which can be reversed to obtain B^c=A. We will use this logic to obtain the password byte array.
3) Since in the inital function the password array is made to XOR with hex value, we will reverse the XOR and make the hex value XOR with predefined byte array.
4) While XOR'ing the explicit byte casting must be done to convert integers into byte to store it into passbytes[32].
5) Print out the byte array while type casting the byte into character to obtain the flag.
