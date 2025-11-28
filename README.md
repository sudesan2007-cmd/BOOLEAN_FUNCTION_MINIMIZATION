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
```
 Program to implement the given logic function and to verify its operations in quartus using Verilog programming. 
Developed by: SUDESAN T
RegisterNumber:25018208

module ex2 (a,b,c,d,w,x,y,z,f1,f2); 
input a,b,c,d,w,x,y,z; 
output f1,f2; 
assign f1 = ~a&~b&~c&~d | a&~c&~d | ~b&c&~d | ~a&b&c&d | b&~c&d; assign f2 = x&~y&z | ~x&~y&z | ~w&x&y | w&~x&y | w&x&y; 
endmodule
```


**RTL realization**

**Output:**
<img width="1918" height="980" alt="Screenshot 2025-11-22 201915" src="https://github.com/user-attachments/assets/9ce701a6-9d72-431d-9c98-6964a503cec9" />


**RTL**

**Timing Diagram**
<img width="1919" height="805" alt="Screenshot 2025-11-20 144426" src="https://github.com/user-attachments/assets/ab07c1b1-041e-480c-8c6e-7eab37183ef8" />


**Result:**

Thus the given logic functions are implemented using and their operations are verified using Verilog programming.

