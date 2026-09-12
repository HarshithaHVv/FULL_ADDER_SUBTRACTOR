<img width="791" height="317" alt="Screenshot 2026-09-12 110637" src="https://github.com/user-attachments/assets/d52ee61d-6b89-4a95-a4ea-89e0a63e8ba5" /># FULL_ADDER_SUBTRACTOR

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
<img width="751" height="892" alt="Screenshot 2026-09-12 110957" src="https://github.com/user-attachments/assets/9f81e978-6203-429d-be5f-bd1e16918d4f" />
<img width="552" height="267" alt="Screenshot 2026-09-12 111423" src="https://github.com/user-attachments/assets/66d3bb59-cb67-4d8d-bc90-0a275a82cc69" />



**Procedure**

Write the detailed procedure here

**Program:**

/* Program to design a half subtractor and full subtractor circuit and verify its truth table in quartus using Verilog programming. Developed by: RegisterNumber:212225230098
half adder-
module half_adder(sum, carry, a, b);
  output sum;
  output carry;
  input a;
  input b;
  assign sum = a ^ b;
  assign carry = a & b;
endmodule
half subtractor-
module half_subtractor(diff, borrow, a, b);
  output diff;
  output borrow;
  input a;
  input b;
  assign diff = a ^ b;
  assign borrow = ~a & b;
endmodule
*/

**RTL Schematic**
<img width="791" height="317" alt="Screenshot 2026-09-12 110637" src="https://github.com/user-attachments/assets/b663f802-ef7b-4272-bb7f-1a60db2a1981" />

**Output Timing Waveform**
<img width="1662" height="538" alt="Screenshot 2026-09-12 110523" src="https://github.com/user-attachments/assets/2c5e943c-bc53-47d3-8601-6044523c0a37" />


**Result:**

Thus the Full Adder and Full Subtractor circuits are designed and the truth tables is verified using Quartus software.



