**In this question, the checkPassword function uses bytes and compares it to another predefined byte array**
**It returns true if all the consequent bytes match with the predefined byte array**

### Method:
1) Convert the byte values into character using the ASCII table.
2) The first 8 bytes are in the form of decimal which have to be matched with the ASCII table.
3) The next 8 bytes are in the form of hexadecimal which have to be matched with the ASCII table.
4) The next 8 bytes are in the form of octal which have to be matched with the ASCII table.
5) The last 8 bytes are in the form of octal which can be directly appended to the string.
6) Join all the 4 strings to obtain a char string in the form of a flag.
