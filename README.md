# EXPERIMENT-02

# IMPLEMENTATION-OF-HALF-ADDER-AND-FULL-ADDER-CIRCUIT

### AIM :
To design a half adder and full adder circuit and verify its truth table in Quartus using Verilog programming.

### EQUIPMENTS REQUIRED : 

- Hardware – PCs, Cyclone II , USB flasher  
- Software – Quartus prime  

## THEORY :
Adders are digital circuits that carry out addition of numbers.

### HALF ADDER :
Half adder is a combinational circuit that performs simple addition of two binary numbers. The input variables designate the augend and addend bits; the output variables produce the sum and carry. It is necessary to specify two output variables because the result may consist of two binary digits.

Sum = A’B+AB’ =A ⊕ B Carry = AB

### FULL ADDER : 
Full adder is a digital circuit used to calculate the sum of three binary bits. It consists of three inputs and two outputs. Two of the input variables, denoted by A and B, represent the two significant bits to be added. The third input, Cin, represents the carry from the previous lower significant position. Two outputs are necessary because the arithmetic sum of three binary digits ranges in value from 0 to 3, and binary 2 or 3 needs two digits. The two outputs are sum and carry.

Sum =A’B’Cin + A’BCin’ + ABCin + AB’Cin’ = A ⊕ B ⊕ Cin Carry = AB + ACin + BCin

 ![image](https://user-images.githubusercontent.com/36288975/163552156-a13e5a56-c638-4110-97d9-8896907c8d25.png)

#### Figure -01 HALF ADDER 


![image](https://user-images.githubusercontent.com/36288975/163552057-b3547877-6d07-45b4-b7e0-bcfebfad9e1d.png)

#### Figure -02 FULL ADDER 

### PROCEDURE :
```
Connect the supply (+5V) to the circuit
Switch ON the main switch
If the output is 1, then the led glows.
```
### 
### PROGRAM : 
```python
Program to design a half adder and full adder circuit and verify its truth table in quartus using Verilog programming.  

Developed by: MIDHUN AZHAHU RAJA P  
RegisterNumber:  22008311
```
HALF ADDER :
```python
module threxp(A,B,Sum,Carry);  
input A,B;   
output Sum,Carry; 
xor(Sum,A,B);  
and(Carry,A,B);  
endmodule
```
FULL ADDDER :  
```
module threxp(A,B,C,Sum,Carry);  
input A,B,C;  
output Sum,Carry;    
assign Sum = ((A^B)^C);  
assign Carry = ((A&B)|(B&C)|(C&A));   
endmodule  
```
## LOGIC GATES : 

### AND GATE :

<img width="145" alt="210804186-b2fd26ff-4908-4580-b064-b49bb33c4b6b" src="https://user-images.githubusercontent.com/118054670/211067110-3f48e804-9284-408a-ac7c-2c5d43cee25a.png">

### OR GATE :

<img width="162" alt="210804152-d3067756-db97-49b6-81f9-859224ab815e" src="https://user-images.githubusercontent.com/118054670/211066726-53d1cea4-2666-44cc-a9d0-6c6f868087ca.png">


### NOT GATE : 

<img width="153" alt="210804437-c8289936-6877-4420-ac8e-b6de9497de25" src="https://user-images.githubusercontent.com/118054670/211067802-a0a0d45d-573b-4899-8564-8d08a53f8425.png">

### XOR GATE :

<img width="157" alt="210804204-908a6987-8a7f-449d-b33b-42b08166e0d9" src="https://user-images.githubusercontent.com/118054670/211067911-0fb99182-1b1a-4f16-9bd8-d61c5a477b57.png">

## OUTPUT : 

## RTL REALIZATION :

### RTL REALIZATION FOR HALF ADDER :

![image](https://user-images.githubusercontent.com/118054670/211161751-572d5548-4bf1-41a8-b1fe-bd1505c21b69.png)

### RTL REALIZATION FOR FULL ADDER :

![image](https://user-images.githubusercontent.com/118054670/211162748-d082d6ef-c27d-41ef-98ee-bc33b13db3b6.png)



## TRUTH TABLE :

### TRUTH TABLE FOR HALF ADDER :

![half-adder2](https://user-images.githubusercontent.com/118054670/211164200-505cd797-c838-4090-9628-00952377db36.png)

### TRUTH TABLE FOR FULL ADDER :

![full-adder2](https://user-images.githubusercontent.com/118054670/211164162-fa1e9a14-b88c-4b07-abe2-07ab62d789f1.png)

## TIMING DIAGRAM :

### TIMING DIAGRAM FOR HALF ADDER :
![ha](https://user-images.githubusercontent.com/118054670/215306559-c0f8079c-85c3-438e-ad6b-8c5e57f5fb76.png)


### TIMING DIAGRAM FOR FULL ADDER :

![fa](https://user-images.githubusercontent.com/118054670/215306561-63759f27-3a5c-4424-b732-f012d8711f62.png)

## RESULT :
Thus The Half Adder And Full Adder Circuit Succesfully Implemented
