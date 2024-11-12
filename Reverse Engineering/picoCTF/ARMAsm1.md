**The program accepts a command line input and stores it in w0. This is passed to the function as a parameter.**

**The .LC0 and .LC1 segments are responsible for stating whether You Win or You Lose respectively.**

### Method:
1) The input integer, which is received in register w0, is stored at stack location [sp + 12].
2) Then, three constants are stored in other locations on the stack:
  79 at [sp + 16]
  7 at [sp + 20]
  3 at [sp + 24]

3) The value 7 (from [sp + 20]) is loaded into w0.
4) The value 79 (from [sp + 16]) is loaded into w1.
5) A lsl operator is used, to indicate shift , accepting three arguments(store-in-which, shift-which, shift-by-which).
6) A left-shift operation is performed,  w0 is assigned the value of w1 shifted left by 7 bits, the value is once again stored at w0.
7) The value of w0 is again passed into [sp+28].
8) ldr w1, [sp, 28]: Stores value at [sp,28] into w1, ldr w0, [sp, 24]: Stores value [sp,24] into w0.
9) A sdiv function is used which is used for division accepts three arguments (store-in-which, divide-which, divide-by-which).
10) The result is stored back in [sp + 28].
11) The value at [sp+28] is loaded into w1, and the value at [sp + 12] is loaded into w0.
12) The program subtracts the original input from value at [sp+28]. This final result is stored back at [sp + 28].
13) Finally, this value is returned for comparison of argument whether it is equal to 0 or not, if yes then it prints out .LC0.
14) The value at w0 is the answer in the form of hex.
