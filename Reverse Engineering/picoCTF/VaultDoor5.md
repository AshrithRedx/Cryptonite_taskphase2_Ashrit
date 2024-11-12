**This question consists of a function checkPassword which accepts string as a password.**
**The string first undergoes URL encoding and then undergoes base64 encoding.**
**This is then matched with a predetermined string to check if the password is either correct or incorrect.**

### Method:
1) Piece together the three subparts of the expected string. This can be solved using reverse decoding.
2) Since the Expected string undergoes base64 encoding at the end, decode it to base 64.
3) Next, use URL decode on the base64 decoded string to obtain the flag.
