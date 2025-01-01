# EXPERIMENT 2 : BOOLEAN_FUNCTION_MINIMIZATION
DATE : 4/10/24
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

Developed by: RegisterNumber:*/
```
module funct1(a,b,c,d,f1);

input a,b,c,d;

output f1;

assign f1=((~b&~d)|(~a&b&d)|(a&b&~c));

endmodule

module funct2(w,x,y,z,f2);

input w,x,y,z;

output f2;
**RTL realization**assign f2=((~y&z)|(w&y)|(x&y));

endmodule

```

**Output:**
![image](https://github.com/user-attachments/assets/d2d4c0e3-c089-4dd0-8fbd-a7709d363f8c)
![image](https://github.com/user-attachments/assets/5a5ddef4-ae78-40bc-b083-d55a35ddd291)
**RTL**
**Timing Diagram**
![image](https://github.com/user-attachments/assets/14a7cfec-2742-445b-8597-2c3daa973eea)

**Result:**

Thus the given logic functions are implemented using and their operations are verified using Verilog programming.
