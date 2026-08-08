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
~~~
implement F1= A’B’C’D’+AC’D’+B’CD’+A’BCD+BC’D, F2=xy’z+x’y’z+w’xy+wx’y+wxy

module ex2 (a,b,c,d,w,x,y,z,f1,f2);
input a,b,c,d,w,x,y,z;
output f1,f2;
assign f1 = ~a&~b&~c&~d | a&~c&~d | ~b&c&~d | ~a&b&c&d | b&~c&d;
assign f2 = x&~y&z | ~x&~y&z | ~w&x&y | w&~x&y | w&x&y;
endmodule
~~~
Developed by: Lenasri R
RegisterNumber:212225040199

**RTL realization**
<img width="1038" height="747" alt="image" src="https://github.com/user-attachments/assets/df9c3243-fe50-440e-87ec-c59a7e8bea39" />

**Output:**
**RTL**
<img width="1043" height="287" alt="image" src="https://github.com/user-attachments/assets/65c2ed89-09e8-40b2-b2f8-740fbcbcaebd" />

**Timing Diagram**
<img width="1041" height="586" alt="image" src="https://github.com/user-attachments/assets/efce5864-0d93-4ddb-aa09-2b334a725974" />

**Result:**

Thus the given logic functions are implemented using and their operations are verified using Verilog programming.


