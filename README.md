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
![386819811-90788abf-e155-4e81-8bfd-1d9a6cde43cd](https://github.com/user-attachments/assets/91b2d743-3dc0-4a4b-970f-fef34f78ced1)

**Truthtable**
![386819817-b2909f47-359f-49b5-ab50-8f1fcdd601df](https://github.com/user-attachments/assets/907c2124-2636-421a-92e7-9d9417a46d4f)

**Procedure**

**Write the detailed procedure here**
1.Write the code in Quartus software by creating a new project wizard. 2.Run the program to get output. 3.Then open RTL viewer and download that image. 4.Open new file with University program VWF 5.Set end timer and execute, then download the waveform.

**Program:**

/* Program to design a half subtractor and full subtractor circuit and verify its truth table in quartus using Verilog programming.
//full adder module EXP_4(sum, cout, a, b, cin); output sum; output cout; input a; input b; input cin; //internal nets wire sl,cl,c2; //Instantiate logic gate primitives xor (sl,a,b); and(cl,a,b); xor(sum, sl, cin); and (c2, sl,cin); or (cout, c2,cl); endmodule

module EXP_4_2 (df, bo, a, b, bin); output df; output bo; input a; input b; input bin; wire w1,w2,w3; assign w1=a^b; assign w2=(~a&b); assign w3=(~w1&bin); assign df=w1^bin; assign bo=w2|w3; endmodule

Developed by: RegisterNumber:
*/24000942

**RTL Schematic**
![386819881-1a838d28-1644-48e8-85fb-9981e7f1dfb1](https://github.com/user-attachments/assets/5669a591-11b9-4d08-a7f1-8c4b4c1a9723)
![386819889-5e9534a0-cb58-4e61-8474-b21ad815d68c](https://github.com/user-attachments/assets/a06d74f8-165a-419f-9c57-ac833998e40e)

**Output Timing Waveform**
![386819892-62813e23-7377-4318-b215-888fd014f030](https://github.com/user-attachments/assets/bd4ad705-870d-4fb7-aa9c-96472e3c64a0)
![386819900-84b13751-a005-4d8f-adc5-ce17185ff732](https://github.com/user-attachments/assets/5ec56b89-c811-4c62-8e92-f6ac168c7aff)

**Result:**
Thus the Full Adder and Full Subtractor circuits are designed and the truth tables is verified using Quartus software.
Thus the Full Adder and Full Subtractor circuits are designed and the truth tables is verified using Quartus software.



