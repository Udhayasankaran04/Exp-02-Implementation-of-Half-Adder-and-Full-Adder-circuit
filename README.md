# Exp-02-Implementation-of-Half-Adder-and-Full-Adder-circuit

# Implementation-of-Half-Adder-and-Full-Adder-circuit
### AIM:
To design a half adder and full adder circuit and verify its truth table in Quartus using Verilog programming.

### Equipments Required:
Hardware – PCs, Cyclone II , USB flasher
Software – Quartus prime
Theory
Adders are digital circuits that carry out addition of numbers.

### Half Adder
Half adder is a combinational circuit that performs simple addition of two binary numbers. The input variables designate the augend and addend bits; the output variables produce the sum and carry. It is necessary to specify two output variables because the result may consist of two binary digits.

Sum = A’B+AB’ =A ⊕ B Carry = AB

### Full Adder
Full adder is a digital circuit used to calculate the sum of three binary bits. It consists of three inputs and two outputs. Two of the input variables, denoted by A and B, represent the two significant bits to be added. The third input, Cin, represents the carry from the previous lower significant position. Two outputs are necessary because the arithmetic sum of three binary digits ranges in value from 0 to 3, and binary 2 or 3 needs two digits. The two outputs are sum and carry.

Sum =A’B’Cin + A’BCin’ + ABCin + AB’Cin’ = A ⊕ B ⊕ Cin Carry = AB + ACin + BCin

 ![image](https://user-images.githubusercontent.com/36288975/163552156-a13e5a56-c638-4110-97d9-8896907c8d25.png)

#### Figure -01 HALF ADDER 


![image](https://user-images.githubusercontent.com/36288975/163552057-b3547877-6d07-45b4-b7e0-bcfebfad9e1d.png)

#### Figure -02 FULL ADDER 

### Procedure

Connect the supply (+5V) to the circuit
Switch ON the main switch
If the output is 1, then the led glows.
### 
Program:
/*
Program to design a half adder and full adder circuit and verify its truth table in quartus using Verilog programming.
Developed by: 
RegisterNumber:  
*/
Logic symbol & Truthtable
RTL realization

### Output:
```

Program to design a half adder and full adder circuit and verify its truth table in quartus using Verilog programming.
Developed by: UDHAYA SANKARAN M
RegisterNumber:212222110051 

HALF ADDER

module HALF_SUB(a,b,diff,borr)
input a,b;
output diff,borr;
assign diff=(a^b)
assign borr=a((~a)&b);
end module;


FULL ADDER
module FULL_SUB (a,b,bin,diff,borr);
input a,b,bin;
output diff,borr;
assign diff=a^b^bin;
assign borr=((~a)&b)|(b&bin)|((~a)&bin);
endmodule
```
### RTL
## HAL FADDER
![image](https://github.com/Udhayasankaran04/Exp-02-Implementation-of-Half-Adder-and-Full-Adder-circuit/assets/119393933/a8768892-3ccf-4e3b-b790-a978bbd832cd)
## FULL ADDER
![image](https://github.com/Udhayasankaran04/Exp-02-Implementation-of-Half-Adder-and-Full-Adder-circuit/assets/119393933/fc8d841d-9194-4bb8-9b96-cb08bcb0e620)
### TIMING DIAGRAM
## HALF ADDER
![image](https://github.com/Udhayasankaran04/Exp-02-Implementation-of-Half-Adder-and-Full-Adder-circuit/assets/119393933/99ebee49-3b94-4bb0-8f33-c301305e67d7)
## FULL ADDER
![image](https://github.com/Udhayasankaran04/Exp-02-Implementation-of-Half-Adder-and-Full-Adder-circuit/assets/119393933/fa298eab-f76e-4f19-a521-241c16ec0c5f)
### TRUTH TABLE 
## HALF ADDER
![image](https://github.com/Udhayasankaran04/Exp-02-Implementation-of-Half-Adder-and-Full-Adder-circuit/assets/119393933/722abb14-b900-47dc-9913-363e96c06e48)
## FULL ADDER
![image](https://github.com/Udhayasankaran04/Exp-02-Implementation-of-Half-Adder-and-Full-Adder-circuit/assets/119393933/eb0d17b3-e1ee-4dfc-b508-47bf02f876a7)
### Result:
Thus the different digital IC's are studied and the truth table for different logic gates are verified.
