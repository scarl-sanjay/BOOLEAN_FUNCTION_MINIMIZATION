# BOOLEAN_FUNCTION_MINIMIZATION

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

/* Program to implement the given logic function and to verify its operations in quartus using Verilog programming. 

Program

~~~

module Boolean_min(A,B,C,D,W,X,Y,Z,F1,F2);
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
assign F1=x1|x2|x3|x4|x5;
assign F2=x6|x7|x8|x9|x10;
endmodule

Developed by: Sanjay S
RegisterNumber: 212223040184
~~~

Logic Symbol and Truth table
![319427043-ab520f8d-0d6f-4bb9-96e6-33968a037418](https://github.com/scarl-sanjay/BOOLEAN_FUNCTION_MINIMIZATION/assets/147120917/b51919fc-aa9d-4aa9-be80-15a1f08b29c2)
![319427157-21cb2aef-7529-4ced-a473-68b7a9e53d62](https://github.com/scarl-sanjay/BOOLEAN_FUNCTION_MINIMIZATION/assets/147120917/955e6020-9e32-4dbf-b7d1-ca6ebf495199)

RTL realization output
![319427331-4d407a87-3dc2-49e6-bea8-bb7683f1857d](https://github.com/scarl-sanjay/BOOLEAN_FUNCTION_MINIMIZATION/assets/147120917/8864d9ea-29fd-440b-a422-6a9532bdfa45)


**RTL**
![319427514-042b4487-4220-4e63-a855-f1475debf723](https://github.com/scarl-sanjay/BOOLEAN_FUNCTION_MINIMIZATION/assets/147120917/e08c4c3c-7f02-46da-8a1a-8fffb7bfdbd3)


**Result:**

Thus the given logic functions are implemented using and their operations are verified using Verilog programming.

