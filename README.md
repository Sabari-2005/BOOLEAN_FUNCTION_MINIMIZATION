# BOOLEAN FUNCTION MINIMIZATION

**AIM:**

To implement the given logic function verify its operation in Quartus using Verilog programming.

F1= A’B’C’D’+AC’D’+B’CD’+A’BCD+BC’D 

F2=xy’z+x’y’z+w’xy+wx’y+wxy

**Equipment Required:**

Hardware – PCs, Cyclone II , USB flasher

**Software – Quartus prime**

**Theory**

**Logic Diagram**

**Procedure**

1.	Type the program in Quartus software.

2.	Compile and run the program.

3.	Generate the RTL schematic and save the logic diagram.

4.	Create nodes for inputs and outputs to generate the timing diagram.

5.	For different input combinations generate the timing diagram.


**Program:**

Developed by: R.Sabarinath

Register Number:212223100048
```
module EXP2(A,B,C,D,W,X,Y,Z,F1,F2);
input A,B,C,D,W,X,Y,Z;
wire x1,x2,x3,x4,x5,x6,x7,x8,x9,x10;
output F1,F2;
assign x1=(~A)&(~B)&(~C)&(~D);
assign x2=(A)&(~C)&(~D);
assign x3=(~B)&(C)&(~D);
assign x4=(~A)&(B)&(C)&(D);
assign x5=(B)&(~C)&(D);
assign x6=(X)&(~Y)&(Z);
assign x7=(~X)&(~Y)&(Z);
assign x8=(~W)&(X)&(Y);
assign x9=(W)&(~X)&(Y);
assign x10=(W)&(X)&(Y);
assign F1=(~B)&(~D)|(A)&(B)&(~C)|(~A)&(B)&(D);
assign F2=(~Y)&(Z)|(X)&(Y)|(W)&(Y);
endmodule
```


**RTL realization**

**Output:**

![EX 02 DE OP](https://github.com/user-attachments/assets/82924313-e5d3-4c72-a8b6-daeba1fc8600)

**RTL**

![image](https://github.com/user-attachments/assets/b786036d-50a4-4301-8ea6-a4fe8d3e4f15)

**Timing Diagram**

![image](https://github.com/user-attachments/assets/84574de4-2db0-4cd7-9430-b740d5257e5d)

**Result:**

Thus the given logic functions are implemented using and their operations are verified using Verilog programming.

