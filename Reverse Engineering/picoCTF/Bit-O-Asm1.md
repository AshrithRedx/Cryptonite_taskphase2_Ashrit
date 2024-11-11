**There is a assembly file given which contains information , one line containing information about the eax register.**

### Method:
1) *At +4* Base pointer is being initialised.
2) *At +5* The base pointer is updated to point to the currect stack pointer.
3) *At +15* The hex value 0x30(decimal:48) is stored inside eax register. This is our required flag.
4) *At +20* Base pointer is being popped.
5) *At +21* the assembly function is returned.
