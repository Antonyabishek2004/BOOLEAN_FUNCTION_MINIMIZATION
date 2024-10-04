### BOOLEAN_FUNCTION_MINIMIZATION

### AIM:

To implement the given logic function verify its operation in Quartus using Verilog programming.

F1= A’B’C’D’+AC’D’+B’CD’+A’BCD+BC’D

F2=xy’z+x’y’z+w’xy+wx’y+wxy

### Equipment Required:
Hardware – PCs, Cyclone II , USB flasher

### Software :
Quartus prime

### Procedure:
1 Type the program in Quartus software.

2 Compile and run the program.

3 Generate the RTL schematic and save the logic diagram.

4 Create nodes for inputs and outputs to generate the timing diagram.

5 For different input combinations generate the timing diagram.

### Program:

## Developed by: ANTONY ABISHEK

### RegisterNumber: 212223240009

F1= A’B’C’D’+AC’D’+B’CD’+A’BCD+BC’D
module ex022(a,b,c,d,f1);
input a,b,c,d;
output f1;
assign f1 =((~b&~d)|(~a&b&d)|(a&b&~c));
endmodule

F2=xy’z+x’y’z+w’xy+wx’y+wxy
module ex021(w,x,y,z,f2);
input w,x,y,z;
output f2;
assign f2=((~y&z)|(x&y)|(w&y));
endmodule

### Truth Table :

![image](https://github.com/user-attachments/assets/5f2f20bb-a68c-45bd-bef2-0811e54eb0e2)

![image](https://github.com/user-attachments/assets/7017de4d-7359-43db-b693-b435a2e7d238)

### RTL realization:

![image](https://github.com/user-attachments/assets/14f3e169-64f0-430a-80fd-ae390f58bcaf)

![image](https://github.com/user-attachments/assets/650839a3-f5a9-4d0b-a437-a71fcb1416e7)

### Timing Waveform:

![image](https://github.com/user-attachments/assets/7ef37f0f-6f4e-4d37-99f8-7f5568694b53)

![image](https://github.com/user-attachments/assets/05c92739-1c36-4bc3-9ae2-762e1c524f29)

### Result:

Thus the given logic functions are implemented using and their operations are verified using Verilog programming.

