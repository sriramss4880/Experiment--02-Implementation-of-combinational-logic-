# Experiment--02-Implementation-of-combinational-logic
Implementation of combinational logic gates
 
## AIM:
To implement the given logic function verify its operation in Quartus using Verilog programming.
 F1= A’B’C’D’+AC’D’+B’CD’+A’BCD+BC’D
F2=xy’z+x’y’z+w’xy+wx’y+wxy
 
 
 
## Equipments Required:
## Hardware – PCs, Cyclone II , USB flasher
## Software – Quartus prime

##Procedure:
1.Create a project with required entities.

2.Create a module along with respective file name.

3.Run the respective programs for the given boolean equations.

4.Run the module and get the respective RTL outputs.

5.Create university program(VWF) for getting timing diagram.

6.Give the respective inputs for timing diagram and obtain the results.



## Program:
/*
```
Program to implement the given logic function using NAND and NOR gates and to verify its operations in quartus using Verilog programming.
Developed by: S.S.SRIRAM
RegisterNumber:  212222230150

module logic(a,b,c,d,w,x,y,z,f1,f2);
input a,b,c,d,w,x,y,z;
output f1,f2;
wire A1,A2,A3,A4,A5,B1,B2,B3,B4,B5;
assign A1=((~a)&(~b)&(~c)&(~d));
assign A2=(a&(~c)&(~d));
assign A3=((~b)&c&(~d));
assign A4=((~a)&b&c&d);
assign A5=(b&(~c)&d);
assign B1=(x&(~y)&z);
assign B2=((~x)&(~y)&z);
assign B3=((~w)&x&y);
assign B4=(w&(~x)&y);
assign B5=(w&x&y);
assign f1=A1|A2|A3|A4|A5;
assign f2=B1|B2|B3|B4|B5;
endmodule
*/
```
## TIMING DIAGRAM

![com1w](https://user-images.githubusercontent.com/120554177/234528708-bc4f6c30-6363-44ee-a7dd-395ff1993c7b.jpg)

## RTL REALIZATION

![com1](https://user-images.githubusercontent.com/120554177/234528518-b25382f6-2b5e-4af0-b0d3-902367288d16.jpg)

![com2](https://user-images.githubusercontent.com/120554177/234528606-46d561d2-ca29-43be-92ea-f5ced676bba6.jpg)

## TRUTH TABLE

![WhatsApp Image 2023-04-26 at 14 07 42](https://user-images.githubusercontent.com/120554177/234521626-83c7f7bf-65fa-45c8-a281-708905e63079.jpg)


## Result:
Thus the given logic functions are implemented using  and their operations are verified using Verilog programming.
