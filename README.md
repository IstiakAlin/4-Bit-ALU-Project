# 4-Bit-ALU-Project


This document is a model and instructions for
creating a 4-bit ALU which takes 2 inputs, generates 1 output
based on the inputs & the operations and also generates 3
flags. This 4-bit ALU is capable of performing 5 different
arithmetic or logical operations which is controlled by an
opcode. The whole ALU has been built using Verilog HDL.<br>

The 4-bit ALU takes 2 four-bit inputs: A & B and a
three-bit operation code(opcode). Depending on the
opcode, it performs five different operations on A and B and
produces a four-bit output, C. Based on the opcode,
different operations are performed on the positive edge of
the clock. For opcode: 000, the ALU will be at the reset
state and the output C will keep the result of the last
operation performed. For opcode: 001,The ALU will
perform bitwise XOR operation on A & B. For opcode: 010,
The ALU will perform ADD operation on A & B. For
opcode: 011 ,The ALU will perform bitwise AND operation
on A & B. Lastly, for opcode: 111,The ALU will
SUBTRACT B from A. Depending on the result(C) of a
particular operation, the ALU also produces three flags:
Carry(CF), Zero(ZF) and Sign(SF). Here, when the output C
is 0, zero flag is set to 1.Otherwise, zero flag is 0. Again,
when the MSB of the output C is 1, sign flag is set to 1.
Otherwise, it is set to 0. Lastly, if an extra carry is
generated, the carry flag is set to 1. Otherwise, it is set to 0.
The ALU has been built in Quartus 2(8.1) and Verilog HDL
has been used as the hardware language. The operations and
outputs of the ALU have been verified via generating the
timing diagram from simulation and analyzing it.<br>



<img width="550" height="400" alt="l1" align="middle" src="https://github.com/user-attachments/assets/fe5ea586-1998-4b73-af22-37ffada80a00" />
