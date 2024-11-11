## Method:
1) *At +0* Assembly code runs.
2) *At +4* Base pointer is initialized and pushed onto stack.
3) *At +5* Base pointer points is set to current stack pointer.
4) *At +15* the hex value '0x9fe1a' is stored inside the pointer PTR[rbp-0x4] using the mov command.
5) *At +22* the value inside the pointer is being copied to the eax register through mov command.
6) *At +25* Base pointer is removed from stack.
7) *At +26* Function returns.

8) The value inside eax is the hex value stored in the pointer which is the flag.
