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

module ex2(A,B,C,D,F1);
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


**RTL realization**
<img width="329" alt="ed ex2 1" src="https://github.com/Mythili7339267708/BOOLEAN_FUNCTION_MINIMIZATION/assets/144260246/33274556-a0d6-48d3-89d7-d972a5843668">


**Output:**
<img width="597" alt="de ex2 2" src="https://github.com/Mythili7339267708/BOOLEAN_FUNCTION_MINIMIZATION/assets/144260246/616c072e-3990-4fc1-b53a-cae5ee40c7a7">


**Timing Diagram:**
<img width="785" alt="de ex 2 3" src="https://github.com/Mythili7339267708/BOOLEAN_FUNCTION_MINIMIZATION/assets/144260246/902260b9-1a1c-413e-b4e5-242b31ea89e4">




**Result:**

Thus the given logic functions are implemented using and their operations are verified using Verilog programming.

