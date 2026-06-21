
## Introduction to Binary Adder
A binary adder is a circuit which adds two binary numbers. It takes two binary numbers as input and gives sum of the two binary numbers and their carry as output. Arithmetic Logic Units uses a binary adders for addition. Binary Adders can be implemented using various Configuration,but the most common configuration is using Half Adder and Full Adder. A half adder adds two single-digit binary numbers and produces the sum and carry output. However, a full adder extends this functionality to accommodate an additional carry input from the previous bit position, allowing it to add three input bits (two operands and the carry from the previous addition) to produce the sum and carry output.

## Design Explanation
In this project, I have designed a 1-bit Full Adder using a 1-bit Half Adder. The Full Adder adds three numbers and produces two outputs.
The **Sum** output is given by **S = A ⊕ B ⊕ C-in**.TThe **Carry** output is given by **C-out = AB + C-in(A ⊕ B)**
The Half Adder was instantiated twice to provide a correct functionality of the full adder. The Sum output from the first Half Adder acts as 
an one input to the second half adder. The other input to the second half adder is the input carry value (carry value of the previous adder). 
The final Sum and Carry are taken from the outputs of the second half adder. 
More information about Binary Adders can be found [here](https://www.geeksforgeeks.org/digital-logic/full-adder-in-digital-logic/) .
