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

**Procedure**
~~~

~~~
**PROGRAM**
~~~
module exp_6(out,clk,rst); 
input clk,rst; 
output reg [3:0]out; 
always @ (posedge clk)
begin 
if(rst) 
out<=0; 
else 
out <= out-1; 
end endmodule
~~~
## Developed by: SANTHOSH KONDURU
## Register Number: 212225240074

**RTL LOGIC FOR 4 Bit Ripple Counter**

<img width="1490" height="836" alt="image" src="https://github.com/user-attachments/assets/dcd5929e-ee7c-4eac-a2ea-7fd6db1033f2" />

**TIMING DIGRAMS FOR 4 Bit Ripple Counter**

<img width="1529" height="799" alt="image" src="https://github.com/user-attachments/assets/0167f9f0-bc58-45cd-a4e5-670151070894" />

**RESULTS**
Thus the bit ripple counter executed successfully.
