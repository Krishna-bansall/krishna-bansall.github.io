+++
title = "Assembly and C"
date = 2026-10-29
type = "notes"
url = "/notes/optical/assembly-and-c/"
+++

## Looking at Assembly

One interesting thing about this particular assembly code 
**C:**	Tiny = 255;
**ASM:** 00007FF605CB17CC  mov         byte ptr [Tiny],0FFh 

1. here-> 0FFH is (remember Tiny = __-->255<--_;) - 255 which is hexadecimally represented as 0FFH 
2. More on assembly as you can see there are certain commands like mov, also i noticed on char its byte, but with the keyword int its dword, so there is a difference there as well
3. you would also notice that the computer gives you access to the bare cpu registers

---
more on:
Pointer and arrays
asm ops