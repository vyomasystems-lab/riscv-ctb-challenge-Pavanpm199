# Challenge Level 1 - logical
In this Challenge, there were 2 bug in the instructions.  


![Screenshot (453)](https://github.com/vyomasystems-lab/riscv-ctb-challenge-Pavanpm199/assets/84024750/abbc3431-5a24-425b-b7e2-6943f786e130)
## Bug1 : 
While using assembly language to program any processor either we can use the register names or the names supported by ABI(application binary interface), therefore here z4 is neither a register name nor used in ABI. I have changed z4 to s4(a valid register name under ABI) to solve this. 
![Screenshot (455)](https://github.com/vyomasystems-lab/riscv-ctb-challenge-Pavanpm199/assets/84024750/21a54ead-a47d-42eb-97a0-e10da1008800)


## Bug2 :
addi is an immediate type of instruction that requires immediate value, hence s0 is an invalid immediate value. Hence s0 must be replaced by any 12 bit value(immediate field is of 12 bit).
![Screenshot (450)](https://github.com/vyomasystems-lab/riscv-ctb-challenge-Pavanpm199/assets/84024750/15686138-eec0-439b-996e-30a2de6c2b72)
