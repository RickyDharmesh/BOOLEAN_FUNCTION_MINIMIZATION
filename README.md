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

**Truth Table**

<img width="483" height="292" alt="image" src="https://github.com/user-attachments/assets/a4835aa4-34ee-420b-a5ad-c824a31c7dbd" />



**Program:**

~~~
 module ex2 (a,b,c,d,w,x,y,z,f1,f2);
 input a,b,c,d,w,x,y,z; output f1,f2;
 assign f1 = ~a&~b&~c&~d | a&~c&~d | ~b&c&~d | ~a&b&c&d | b&~c&d;
 assign f2 = x&~y&z | ~x&~y&z | ~w&x&y | w&~x&y | w&x&y;
 endmodule
~~~

Developed by: RICKY DHARMESH . P

RegisterNumber:25016025


**RTL realization**

<img width="1918" height="1079" alt="Screenshot 2025-12-14 222252" src="https://github.com/user-attachments/assets/9e478100-4199-46f5-b15d-da354e1ec653" />


**Timing Diagram**

<img width="1919" height="1079" alt="Screenshot 2025-12-14 223157" src="https://github.com/user-attachments/assets/c07684ce-6549-4606-9352-0c31b8ef140f" />



**Result:**

Thus the given logic functions are implemented using and their operations are verified using Verilog programming.

