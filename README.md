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

Developed by: RAKSHATHA S A  RegisterNumber: 212225220079*/
```
Emodule exp2_0079 (
input A, B, C, D,
output F
) ;
assign F = (~A & ~B & ~C & ~D) |
           (A & ~C & ~D )      |
           (~ B & C & ~ D)     |
           (~ A & B & C & D)   |
           ( B & ~C & D ); 

endmodule
```


**RTL realization**

<img width="1600" height="852" alt="image" src="https://github.com/user-attachments/assets/1634dabc-e609-4872-a731-30a9c450ad34" />

**RTL**

<img width="1600" height="848" alt="image" src="https://github.com/user-attachments/assets/baea6dc1-9ca3-43ed-98a0-1c7f9842b7cd" />


**Timing Diagram**

<img width="1041" height="586" alt="633235258-efce5864-0d93-4ddb-aa09-2b334a725974" src="https://github.com/user-attachments/assets/e8807e89-dbdd-40c3-a126-ca2fcac681ad" />


**Result:**
Thus the given logic functions are implemented using and their operations are verified using Verilog programming.

Thus the given logic functions are implemented using and their operations are verified using Verilog programming.

