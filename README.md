### ENCODER 8TO3 DATAFLOW Modelling

**AIM:**

To implement  Encoder 8 To 3 in Dataflow Modelling using verilog and validating their functionality using their functional tables

**SOFTWARE REQUIRED:** Quartus prime

**THEORY**

**Encoder 8 To 3**

The 8 to 3 line Encoder is also known as Octal to Binary Encoder. In 8 to 3 line encoder, there is a total of eight inputs, i.e., D0, D1, D2, D3, D4, D5, D6, and D7 and three outputs, i.e., A0, A1, and A2. In 8-input lines, one input-line is set to true at a time to get the respective binary code in the output side. Below are the block diagram and the truth table of the 8 to 3 line encoder.

![image](https://github.com/user-attachments/assets/f36a1381-f63f-45be-a328-b4fa78d088af)

Figure 01  Block Diagram of Encoder 8 * 3

**Truth Table**

![image](https://github.com/user-attachments/assets/c2956352-4c77-4df3-9f13-a9b6e974073b)

The logical expression of the term A0, A1, and A2 are as follows:

A0 = D1 + D3 + D5 + D7

A1 = D2 + D3 + D6 + D7

A2 = D4 + D5 + D6 + D7

Logical circuit of the above expressions is given below:

![image](https://github.com/user-attachments/assets/34692785-fbc6-44c8-8f99-990bd18fef11)

Figure 02  Encoder 8 * 3

**Procedure**

/* write all the steps invloved */

**PROGRAM**

/* Program for Encoder 8 To 3 in Dataflow Modelling and verify its truth table in quartus using Verilog programming. 

Developed by:Paveen Kumaran SV
RegisterNumber:24000025

module encoder(a,b,c,y0,y1,y2,y3,y4,y5,y6,y7);

input y0,y1,y2,y3,y4,y5,y6,y7;

output a,b,c;

assign a= ( y4 | y5 | y6 | y7);

assign b= ( y2 | y3 | y6 | y7);

assign c= ( y1 | y3 | y5 | y7);

endmodule

**RTL LOGIC FOR Encoder 8 To 3 in Dataflow Modelling**

![image](https://github.com/user-attachments/assets/4296fde3-8516-46f6-a770-55f08f88e2c0)

**TIMING DIGRAMS FOR Encoder 8 To 3 in Dataflow Modelling**

**RESULTS**

Thus the truth table of Encoder 8 to 3 in Dataflow Modelling in Quartus || using verilog programming are studied, verified and executed successfully.


