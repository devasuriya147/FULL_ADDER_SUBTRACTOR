# FULL_ADDER_SUBTRACTOR

Implementation-of-Full-Adder-and-Full-subtractor-circuit

**AIM:**

To design a Full Adder and Full Subtractor circuit and verify its truth table in Quartus using Verilog programming.

**Equipments Required:**

Hardware – PCs, Cyclone II , USB flasher

Software – Quartus prime

**Full Adder and Full Subtractor**

**Full Adder**

Full adder is a digital circuit used to calculate the sum of three binary bits. It consists of three inputs and two outputs. Two of the input variables, denoted by A and B, represent the two significant bits to be added. The third input, Cin, represents the carry from the previous lower significant position. Two outputs are necessary because the arithmetic sum of three binary digits ranges in value from 0 to 3, and binary 2 or 3 needs two digits. The two outputs are sum and carry.

Sum =A’B’Cin + A’BCin’ + ABCin + AB’Cin’ = A ⊕ B ⊕ Cin 

Carry = AB + ACin + BCin

![image](https://github.com/naavaneetha/FULL_ADDER_SUBTRACTOR/assets/154305477/0f30ba51-5ffb-4198-845f-18e054f675e7)

**Figure -1 FULL ADDER**

**Full Subtractor**

A full subtractor is a combinational circuit that performs subtraction involving three bits, namely minuend, subtrahend, and borrow-in . It accepts three inputs: minuend, subtrahend and a borrow bit and it produces two outputs: difference and borrow.

![image](https://github.com/naavaneetha/FULL_ADDER_SUBTRACTOR/assets/154305477/02b24f51-ab51-4304-9ad6-7b81ffc1ead5)

Diff = A ⊕ B ⊕ Bin 

Borrow out = A'Bin + A'B + BBin

**Truthtable**

## FULL ADDDER
<img width="433" height="398" alt="Screenshot 2026-03-11 103522" src="https://github.com/user-attachments/assets/7e040ebe-6271-43d0-8ab8-4dd5aec9f44d" />


## FULL SUBRACTOR
<img width="448" height="392" alt="Screenshot 2026-03-11 103529" src="https://github.com/user-attachments/assets/f96e4b06-af67-4015-8be8-6970ef697cd4" />


**Procedure**

Write the detailed procedure here

**Program:**

** Program to design a half subtractor and full subtractor circuit and verify its truth table in quartus using Verilog programming.** 
```
**Developed by: DEVASURYA M**
**RegisterNumber:212225230048**
**Full adder**
module exp3(A,B,Cin,S,C);
input A,B,Cin;
output S,C;
assign S=A^B^Cin;
assign C=(A&B)|(A&Cin)|(B&Cin);
endmodule
**Full sub**
module expfs (A,B,Bin,diff,Borr);
input A,B,Bin;
output diff,Borr;
assign diff = A ^ B ^ Bin;
assign Borr = (~A & Bin) | (~A & B) | (B & Bin);
endmodule
```


**RTL Schematic**
## FULL ADDER

<img width="1153" height="754" alt="Screenshot 2026-03-11 102818" src="https://github.com/user-attachments/assets/7b55bde2-f153-4127-87d0-ba3f0366a4e3" />

## FULL SUB
<img width="1118" height="648" alt="Screenshot 2026-03-11 102833" src="https://github.com/user-attachments/assets/6b852f9f-c341-4957-9508-5a947f7232d8" />


**Output Timing Waveform**
## FULL ADD
<img width="1216" height="370" alt="Screenshot 2026-03-11 103111" src="https://github.com/user-attachments/assets/560cb72e-eabb-4850-83b1-4790928f5141" />

## FULL SUB
<img width="1215" height="265" alt="image" src="https://github.com/user-attachments/assets/8db620c9-1543-4434-9f6e-7481114969be" />


**Result:**

Thus the Full Adder and Full Subtractor circuits are designed and the truth tables is verified using Quartus software.



