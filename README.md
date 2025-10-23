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
*Half_adder*
module halfadd_top(a,b,sum,carry);
input a,b;
output sum,carry; 
 assign sum = a^b;
 assign carry = a & b;
endmodule

*Half_subtractor*
module halfsub_top(a,b,D,Bo);
input a,b;
output D,Bo; // Outputs sum and carry for half adder:Outputs difference D,Borrow Bo for half subtractor
assign D = a ^ b;
  assign Bo = ~a & b;
endmodule

/* Program to implement the given logic function and to verify its operations in quartus using Verilog programming. 

Developed by: RegisterNumber:*/


**RTL realization**
<img width="1920" height="1080" alt="Screenshot (23)" src="https://github.com/user-attachments/assets/755d8968-4d9a-4534-9489-1d8fcfcc3450" />


**Output:**
<img width="1920" height="1080" alt="Screenshot (24)" src="https://github.com/user-attachments/assets/d46f6767-7592-4ea8-be45-48b361454bec" />

**RTL**
<img width="1920" height="1080" alt="Screenshot (22)" src="https://github.com/user-attachments/assets/95280545-8c22-462a-9b5e-396cf8a98cb5" />

**Timing Diagram**
<img width="1920" height="1080" alt="Screenshot (24)" src="https://github.com/user-attachments/assets/ce1d5e8a-135a-47d3-b43c-02e462237c08" />

**Result:**

Thus the given logic functions are implemented using and their operations are verified using Verilog programming.

