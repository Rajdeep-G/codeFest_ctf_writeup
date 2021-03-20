# C is hard  

The pawning question was vulnerable to buffer overflow. 

So i designed the payload to buffer overflow the local_20 char array and the passed the print_flag() function address into the stack to call the print_flag function.

![vuln](./vuln.PNG)

I found out the address of the function print_flag by objdump.

![objdump](./objdump.PNG)

Then i inserted the payload and it worked....yay!!!!

![payload](./payload.PNG)
