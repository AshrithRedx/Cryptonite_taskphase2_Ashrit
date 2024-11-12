**This ARM assembly program comprises three main functions: func1, func2, and main.**
**The main accepts a single parameter as input which is later on passed on to func1 and func2.**

### Method:
1) The func1 function takes a single integer as input, processes it through a loop, and outputs a result.
2) The input argument is stored at [x29 + 28].
3) The another variable for accumulating results is initialized to zero with the wzr register at [x29 + 44].
4) The func1 calls .L2 label.
5) The value  stored in [x29 + 28] undegoes AND operation with 1 which results in either odd or evem.
6) If the value is odd, it calls func2. Regardless of odd/even status, the value is right-shifted by 1 bit (divided by 2).
7) This loop continues until the input value becomes zero. Once the loop ends, func1 loads the accumulated result from [x29 + 44] and returns it to the caller
8) Func2 is called b func1 whenever the current value is odd.
9) Each time it’s called, it adds 3 to the running result in func1.
10) Main passes the converted integer to func1, which performs the calculations and returns a result.
11) This value obtained turned into hex is the flag required.
