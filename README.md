# Number Theory: Addition
In this lab you've learned the basics of number theory as it relates to addition.

## Rubric
| Item | Description | Value |
| ---- | ----------- | ----- |
| Summary Answers | Your writings about what you learned in this lab. | 25% |
| Question 1 | Your answers to the question | 25% |
| Question 2 | Your answers to the question | 25% |
| Question 3 | Your answers to the question | 25% |

## Name
Aprameya Koushik Sarukkai And Jay Berry

## Summary
We started with the simulation of staircase light with upstairs and downstairs light switches. This represented an XOR gate. Next we completed a single bit adder, which was a combination of a XOR gate for the sum and an AND gate for the carry. We expanded on this to create a 2 bit full adder which also takes in the carry out from the previous step as a carry in. After creating the equations from the K map we implemented them in verilog using 2 instances of an adder combined into one circuit inside the top level file. By testing on the Basys board we comfirmed the equations.

## Lab Questions
### 1 - How might you add more than two bits together?
We can make each of section individually and then add each bit together. This will create a chain of bits.

### 2 - What is the importance of the XOR gate in an adder?
The XOR gate allows us to make a circuit like the stairs example to only allow for one input at a time.

### 3 - What is the largest number a two bit adder can handle? What happens when you go over?
A two bit adder can handle up to 3, which would be 11 in binary. When you go over the result would go back to 0 for bother bits. This would be incorrect for numbers greater than 3 we would need another bit for every 2 numbers to take in the LSB and the MSB. A number of size requiring n bits would need n bit adders.