# Challenge level 1 - loops 
In this challenge, the code was running infinitly due to a bug. 
![Screenshot (458)](https://github.com/vyomasystems-lab/riscv-ctb-challenge-Pavanpm199/assets/84024750/4ac10592-04b6-43df-afbf-658daa6f9420)
![Screenshot (459)](https://github.com/vyomasystems-lab/riscv-ctb-challenge-Pavanpm199/assets/84024750/b8d348a4-6999-417c-9c6f-92d17c5c63e0)

This piece of code adds two value and compares if the sum is equal to the third value. Here 1st, 2nd and 3rd value are taken from consequent locations. 
Hence there is an increment of +4 in address. The code goes into loop until sum of two values is equal to 3rd value. In the set of given values 
the sum of 1st two values is equal to 3rd in every iteration. Hence the code never breaks out of the loop.

## Solution:
To solve this, I have used t5 register which has the value 3. As this set of data requires 3 iterations to check all values, I increment t6(which is intially 0) by 1 in each iteration. 
When the t6 equals t5 control goes to end of code
![Screenshot (461)](https://github.com/vyomasystems-lab/riscv-ctb-challenge-Pavanpm199/assets/84024750/95c888bc-90ae-4bd9-ac4e-9058f5a20a65)


# Bug fix :
![Screenshot (463)](https://github.com/vyomasystems-lab/riscv-ctb-challenge-Pavanpm199/assets/84024750/10f4a7ea-e177-4c29-82a8-636256b198b0)
