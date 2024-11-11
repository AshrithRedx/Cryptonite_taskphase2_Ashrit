## Method:
1) *At +0* Assembly code runs.
2) *At +4* Base pointer is initialized and pushed onto stack.
3) *At +5* Base pointer points is set to current stack pointer.
4) *At +15* the hex value '0x9fe1a' is stored inside the pointer PTR[rbp-0x4] using the mov command.
5) *At +22* the hex value '0x2710' is being compared to value stored in PTR[rbp-0x4] using cmp command.
6) *At +29* if the value is less than the hex value, it jumps to <+37>, else follows original flow througn jle command. 
7) *At +31* the values at PTR[rbp-0x4] undergoes subtraction with hex value 0x65.
8) *At +35* the program jumps to +41 through a unconditional jump statement, using jmp command.
9) *At +41* The value of eax is obtained from PTR [rbp-0x4] .

10) *At +44* Base pointer is removed from stack.
11) *At +45* Function returns.

12) The value inside eax is the hex value stored in the pointer which is the flag.
