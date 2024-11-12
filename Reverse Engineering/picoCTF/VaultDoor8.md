**The checkPassword function scrambles each character of the password using two main components.**
**Scramble Function: Transforms each character in the password by repeatedly swapping bits within each character using the switchBits function.**
**SwitchBits Function: This function exchanges two bits within a character at specific positions.**

### Method:
1) To retrieve the original password, we need to reverse-engineer the scrambling process.
2) The reverse of each of these steps to work backwards from the scrambled characters in expected to the original password characters.
3) The switchBits function in the code swaps two bits at specified positions within a character.
4) This function is called within the scramble function.
5) To reconstruct the original password, we need to apply each bit swap from scramble.
6) Obtain the array again and append it in the form of a string to obtain the flag.
