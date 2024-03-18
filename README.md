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

Program to implement the given logic function and to verify its operations in quartus using Verilog programming. 

Developed by : Shanmuga Vasanth M

RegisterNumber : 212223040191  

```
module ex02(A,B,C,D,F1);
input A,B,C,D;
output F1;
wire x1,x2,x3,x4,x5;
assign x1=(~A)&(~B)&(~C)&(~D);
assign x2=(A)&(~C)&(~D);
assign x3=(~B)&(C)&(~D);
assign x4=(~A)&(B)&(C)&(D);
assign x5=(B)&(~C)&(D);
assign F1=x1|x2|x3|x4|x5;
endmodule
```

**RTL realization**

**Output:**


**Truth Table**

![311433313-399f99d5-79cc-443a-b54a-41d7a0326a5c](https://github.com/shanmugavasanth/BOOLEAN_FUNCTION_MINIMIZATION/assets/144870621/6fe2526f-a70e-419b-aded-98ef5293f09f)


**RTL**

**Timing Diagram**

![312692316-ec1bfefa-87c6-4983-8cc9-a98c8ce47a06](https://github.com/shanmugavasanth/BOOLEAN_FUNCTION_MINIMIZATION/assets/144870621/a988a3ce-2a02-4ae6-88a2-632fbf5beee4)


**Result:**

Thus the given logic functions are implemented using and their operations are verified using Verilog programming.

