# Challenge level 2 - Instructions

In this challenge, there was bug in configuration file which was used to generate AAPG.
## BUG:
In configuration file, we can specify the type of instruction to be included in AAPG. 
![Screenshot (464)](https://github.com/vyomasystems-lab/riscv-ctb-challenge-Pavanpm199/assets/84024750/414a795c-5e0e-4bbf-a972-76c31b57c3ad)
We know that processor supports rv32i instruction set. As we can see in the configuration 10 value given for rv64m. This generates rv64m instructions 
which are 64 bit and do not comply with the processors architecture.   

BUG fix:
Removing the value for rv64m generates correct AAPG.
![Uploading Screenshot (465).png…]()
