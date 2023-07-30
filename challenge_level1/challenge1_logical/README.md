Challenge Level 1 - logical
In this Challenge, there were 2 bug in the instructions.  
![Screenshot (448)](https://github.com/vyomasystems-lab/riscv-ctb-challenge-Pavanpm199/assets/84024750/8e74b314-d73a-4d59-bf0c-d83faf95c750)
## Bug1 : 
While using assembly language to program any processor either we can use the register names or the names supported by ABI(application binary interface), therefore here z4 is neither a register name nor used in ABI. I have changed z4 to s4(a valid register name under ABI) to solve this. 
## Bug2 :
addi is an immediate type of instruction that requires immediate value, hence s0 is an invalid immediate value. Hence s0 must be replaced by any 12 bit value(immediate field is of 12 bit).
