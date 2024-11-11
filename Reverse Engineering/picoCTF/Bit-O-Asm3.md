## Method:
1) *At +0* Assembly code runs.
2) *At +4* Base pointer is initialized and pushed onto stack.
3) *At +5* Base pointer points is set to current stack pointer.
4) *At +15* the hex value '0x9fe1a' is stored inside the pointer PTR[rbp-0xc] using the mov command.
5) *At +22* the hex value '0x4' is stored inside the pointer PTR[rbp-0x8] using the mov command.
6) *At +29* the hex value at pointer [rbp-0x8] is stored inside eax register.
7) *At +32* the values at eax and PTR [rbp-0x8] go under integer multiplication and stored insde eax register.
8) *At +36* the hex value 0x1f5 is added to eax register value through add function.
9) The value of eax to and fro PTR [rbp-0x4] at <+41> and <+44>.
10) *At +47* Base pointer is removed from stack.
11) *At +48* Function returns.

12) The value inside eax is the hex value stored in the pointer which is the flag.
