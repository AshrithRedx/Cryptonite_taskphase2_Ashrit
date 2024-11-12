**The program starts in main, where it saves the necessary registers and sets up the stack frame.**
**It then retrieves command-line arguments  and uses the atoi function to convert these arguments from strings to integers.**

### Method:
1) The value at w0 is loaded into w19 and then it is loaded back into w0 at the subsequent steps.
2) The main function expects two arguments w1 and w0 and compares them in function func.

3) The function is called with two arguments w0 and w1 , with w1 as first argument and w0 as second argument.
4) If w1 is less than w0, then it calls .L2 segment which puts the second argument value into w0
5) Else, it is retaining the same value of w0. It finally returns the value at w0.

6) This is a program which returns the greater value in the two arguments and returns it in the form of a hex value.
