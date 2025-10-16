### ENCODER 8TO3 DATAFLOW Modelling

## Name: K rahul royal
## Reg No: 212224240126

*AIM:*

To implement  Encoder 8 To 3 in Dataflow Modelling using verilog and validating their functionality using their functional tables

*SOFTWARE REQUIRED:* Quartus prime

*THEORY*

*Encoder 8 To 3*

The 8 to 3 line Encoder is also known as Octal to Binary Encoder. In 8 to 3 line encoder, there is a total of eight inputs, i.e., D0, D1, D2, D3, D4, D5, D6, and D7 and three outputs, i.e., A0, A1, and A2. In 8-input lines, one input-line is set to true at a time to get the respective binary code in the output side. Below are the block diagram and the truth table of the 8 to 3 line encoder.

![image](https://github.com/naavaneetha/ENCODER8TO3DATAFLOW/assets/154305477/0bc242c1-eb9e-4c47-afe5-30428470efc3)

Figure 01  Block Diagram of Encoder 8 * 3

*Truth Table*

![image](https://github.com/naavaneetha/ENCODER8TO3DATAFLOW/assets/154305477/35496b14-ae6e-4cd1-9abd-d6736b576575)

The logical expression of the term A0, A1, and A2 are as follows:

A0 = D1 + D3 + D5 + D7

A1 = D2 + D3 + D6 + D7

A2 = D4 + D5 + D6 + D7

Logical circuit of the above expressions is given below:

![image](https://github.com/naavaneetha/ENCODER8TO3DATAFLOW/assets/154305477/95acaee6-c873-4c75-89eb-ef09fb158053)

Figure 02  Encoder 8 * 3

*Procedure*
1.Type the program in Quartus software.*\
2.Compile and run the program.*\
3.Generate the RTL schematic and save the logic diagram.*\
4.Create nodes for inputs and Outputs to generate the timing diagrams.*\
5.For different input combinations generate the tiiming diagram.\
*PROGRAM*

module EX_05(a0,a1,a2,d0,d1,d2,d3,d4,d5,d6,d7);
input d0,d1,d2,d3,d4,d5,d6,d7;
output a0,a1,a2;
assign a0=d1|d3|d5|d7;
assign a1=d2|d3|d6|d7;
assign a2=d4|d5|d6|d7;
endmodule



*RTL LOGIC FOR Encoder 8 To 3 in Dataflow Modelling*
<img width="1920" height="1133" alt="489964642-41f2c439-247f-4f9a-b968-d736db725db0 (1)" src="https://github.com/user-attachments/assets/914c4bc1-e13b-4ccf-83e8-89d9e6ebef66" />

*TIMING DIGRAMS FOR Encoder 8 To 3 in Dataflow Modelling*
<img width="1920" height="1130" alt="489964708-fb03ca9f-5a9d-447e-8408-7442fe74b8e3 (1)" src="https://github.com/user-attachments/assets/e5133969-fb39-4642-bdf3-b852b68c68fd" />

*RESULTS*
The code executed successfully.



