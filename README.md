# 4-BIT-RIPPLE-COUNTER

**AIM:**

To implement  4 Bit Ripple Counter using verilog and validating their functionality using their functional tables

**SOFTWARE REQUIRED:**

Quartus prime

**THEORY**

**4 Bit Ripple Counter**

A binary ripple counter consists of a series connection of complementing flip-flops (T or JK type), with the output of each flip-flop connected to the Clock Pulse input of the next higher-order flip-flop. The flip-flop holding the least significant bit receives the incoming count pulses. The diagram of a 4-bit binary ripple counter is shown in Fig. below.

![image](https://github.com/naavaneetha/4-BIT-RIPPLE-COUNTER/assets/154305477/cb4b74d4-31ab-4359-95d0-d22e67daba13)

In timing diagram Q0 is changing as soon as the negative edge of clock pulse is encountered, Q1 is changing when negative edge of Q0 is encountered(because Q0 is like clock pulse for second flip flop) and so on.

![image](https://github.com/naavaneetha/4-BIT-RIPPLE-COUNTER/assets/154305477/a573a7d6-014e-4e54-93e6-e2ac9530960b)

![image](https://github.com/naavaneetha/4-BIT-RIPPLE-COUNTER/assets/154305477/85e1958a-2fc1-49bb-9a9f-d58ccbf3663c)


**PROGRAM**

module ex12(out,clk,rst);

input clk,rst;

output reg [3:0]out;

always @ (posedge clk)

begin

   if(rst)
   
     out<=0;
     
   else 
   
     out <= out-1;
     
end

endmodule


 Developed by:Ezhilarasi N RegisterNumber:212224040088


**RTL LOGIC FOR 4 Bit Ripple Counter**

![EX12](https://github.com/user-attachments/assets/6291f5d2-ef1d-42d5-9cd6-dc7bd12fd831)


**TIMING DIGRAMS FOR 4 Bit Ripple Counter**

![EX12 TIME](https://github.com/user-attachments/assets/913610f6-0541-4a71-9933-3e28e46aa902)


**RESULTS**

Implementation of 4 Bit Ripple Counter using verilog and validating their functionality using their functional tables is verified.
