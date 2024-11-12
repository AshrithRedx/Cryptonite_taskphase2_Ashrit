### Method:
1) The function begins by allocating 32 bytes of space on the stack. It then stores the input, passed iy into w0 register, in the stack location [sp + 12].
2) The *wzr (zero) register* is used to store 0 at two locations- [sp + 24] and [sp + 28].
3) Two Labels are present, .L2 and .L3 , function jumps to label .L2, which starts the main loop.

4) The loop increments two values on the stack each time it runs:
  [sp + 24] is incremented by 3.
  [sp + 28] is incremented by 1.

5) After each iteration, the function checks if value at [sp+28] is equal to the input argument.
6) The function then loads the modified value from [sp + 24] ( increased by 3 each loop iteration) into w0 and returns this value as the function's result.

7) The converted integer argument in main using atoi is passed to func1. The result from func1 is stored in w0.
8) Finally, main prints out the number which when converted to hexadecimal, is the flag.
