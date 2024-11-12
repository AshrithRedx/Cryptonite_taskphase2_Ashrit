**In this question , the checkPassword function checks whether length of string entered is 32.**
**It calls another function which accepts a String input and converts it into a byte array, and returns the byte array.**
**It then shifts the bytes left by 24,16,8,0 for indice multiples of 4i,4i+1,4i+2,4i+3 respectively.**

### Method:
1) Take the predetermined values in the checkPassword function and make it into a array of int.
2) This question can be solved by backtracing.
3) Convert the values into hex values, and shift the values at indice positions multiple of 4, 4i+1 etc.
4) Obtain the new hex values and use ASCII table to decode it to a string which is the required flag.
