# Experiment--02-Implementation-of-combinational-logic
## Implementation of combinational logic gates

## AIM:

To implement the given logic function verify its operation in Quartus using Verilog programming. F1= A’B’C’D’+AC’D’+B’CD’+A’BCD+BC’D

## Components Required:

1.Hardware – PCs, Cyclone II , USB flasher

2.Software – Quartus prime

## Theory:

1.Logic gates are electronic circuits which perform logical functions on one or more inputs to produce one output.

2.Using AND gate:
An AND gate is a fundamental digital logic gate that performs a logical conjunction on its input signals. It produces an output signal only when all of its input signals are high (logic level 1). If any of the input signals is low (logic level 0), the output of the AND gate remains low.

3.using NOT gate:
A NOT gate, also known as an inverter, is a basic digital logic gate that performs the operation of negation on its input signal. In other words, it produces the opposite (complementary) output to its input. If the input is high (logic level 1), the output will be low (logic level 0), and if the input is low, the output will be high.

4.using OR gate:
An OR gate is a fundamental digital logic gate that performs a logical disjunction on its input signals. It produces an output signal when at least one of its input signals is high (logic level 1). The output remains low only if all input signals are low (logic level 0).

## Procedure

1.Create a project with required entities.

2.Create a module along with respective file name.

3.Run the respective programs for the given boolean equations.

4.Run the module and get the respective RTL outputs.

5.Create university program(VWF) for getting timing diagram. 

6.Give the respective inputs for timing diagram and obtain the results.

## Program:
Program to implement the given logic function and to verify its operations in quartus using Verilog programming.

Developed by: Abdul hameed.H

RegisterNumber: 212222050001

```
module expression(a,b,c,d,f1);
input a,b,c,d;
output f1;
wire x1,x2,x3,x4,x5;
assign x1=(~a)&(~b)&(~c)&(~d);
assign x2=(a)&(~c)&(~d);
assign x3=(~b)&(c)&(~d);
assign x4=(~a)&(b)&(c)&(d);
assign x5=(b)&(~c)&(d);
assign f1=x1|x2|x3|x4|x5;
endmodule
```
## RTL diagram:

![image](https://github.com/lovelydevil36/Experiment--02-Implementation-of-combinational-logic-/assets/123564624/61d0297e-24a3-4940-9286-46b443b60548)

## Truth Table:

![image](https://github.com/lovelydevil36/Experiment--02-Implementation-of-combinational-logic-/assets/123564624/ab0d48a1-55ff-4381-9273-4ef7187efe87)


## Output waveform:

![image](https://github.com/lovelydevil36/Experiment--02-Implementation-of-combinational-logic-/assets/123564624/b8fa94b0-dab3-4ad5-ac97-fda39da9b506)


## Result:
Thus the given logic functions are implemented using and their operations are verified using Verilog programming.
