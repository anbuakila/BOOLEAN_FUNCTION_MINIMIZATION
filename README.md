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

Developed by:A.AKILA RegisterNumber:24900889


**RTL realization**

**Output:**
```
module boolean (a,b,c,d,w,x,y,z,f1,f2);
input a,b,c,d,w,x,y,z;
output f1,f2;
assign f1=(~a&~b&~c&~d)|(a&~c&~d)|(~b&c&~d)|(~a&b&c&d)|(b&~c&d);
assign f2=(x&~y&z)|(~x&~y&z)|(~w&x&z)|(w&~x&y)|(w&x&y);
endmodule
```

**RTL**

![BOOLEAN](https://github.com/user-attachments/assets/85169ef4-2628-4697-b423-156acf42b822)


**Timing Diagram**


![BOOLEAN WAVEFORM](https://github.com/user-attachments/assets/a1eb051f-efd7-4a1b-86ed-543e2c7a0b45)


**Result:**

Thus the given logic functions are implemented using and their operations are verified using Verilog programming.

