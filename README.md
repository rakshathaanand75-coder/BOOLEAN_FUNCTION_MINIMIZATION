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
module exp2_0079(q, clk, reset);

output [3:0] q;
input clk, reset;

T_FF tff0(q[0], clk, reset);
T_FF tff1(q[1], q[0], reset);
T_FF tff2(q[2], q[1], reset);
T_FF tff3(q[3], q[2], reset);

endmodule


module T_FF(q, clk, reset);

output q;
input clk, reset;

wire d;

D_FF dff0(q, d, clk, reset);

not n1(d, q);

endmodule


module D_FF(q, d, clk, reset);

output q;
input d, clk, reset;

reg q;

always @(negedge clk or posedge reset)
begin
    if (reset)
        q = 1'b0;
    else
        q = d;
end

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

