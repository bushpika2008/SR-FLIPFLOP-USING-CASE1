# SR-FLIPFLOP-USING-CASE1
# AIM:

To implement SR flipflop using verilog and validating their functionality using their functional tables

# SOFTWARE REQUIRED:

Quartus prime

# THEORY

SR Flip-Flop SR flip-flop operates with only positive clock transitions or negative clock transitions. Whereas, SR latch operates with enable signal. The circuit diagram of SR flip-flop is shown in the following figure.

<img width="738" height="451" alt="image" src="https://github.com/user-attachments/assets/1a3b5d0b-ec17-4c54-b863-cbbcaba207ea" />

This circuit has two inputs S & R and two outputs Qtt & Qtt’. The operation of SR flipflop is similar to SR Latch. But, this flip-flop affects the outputs only when positive transition of the clock signal is applied instead of active enable. The following table shows the state table of SR flip-flop.

<img width="805" height="427" alt="image" src="https://github.com/user-attachments/assets/c01d2a06-9d6b-4736-bdbe-c43ffa0ffc5b" />
Here, Qtt & Qt+1t+1 are present state & next state respectively. So, SR flip-flop can be used for one of these three functions such as Hold, Reset & Set based on the input conditions, when positive transition of clock signal is applied. The following table shows the characteristic table of SR flip-flop. Present Inputs Present State Next State

<img width="656" height="565" alt="image" src="https://github.com/user-attachments/assets/b409098a-f725-4a09-90de-2581e363ad0c" />
By using three variable K-Map, we can get the simplified expression for next state, Qt+1t+1. The three variable K-Map for next state, Qt+1t+1 is shown in the following figure.

<img width="408" height="277" alt="image" src="https://github.com/user-attachments/assets/bfa2ff31-bc04-433d-9a3b-c7554b169977" />

The maximum possible groupings of adjacent ones are already shown in the figure. Therefore, the simplified expression for next state Qt+1t+1 is Q(t+1)=S+R′Q(t)Q(t+1)=S+R′Q(t)

# Procedure

/* write all the steps invloved */ 1.Open quarts || and creat New project wizard.2.Write the program in Verilog HDL file and run the program.3.Download the RTL viewer.4.Now open the university program VEF and download waveform after the execution.

# PROGRAM

/* Program for flipflops and verify its truth table in quartus using Verilog programming.
```
module exp_6(S,R,clk,Q,Qbar); 
input S,R,clk; 
output reg Q; 
output reg Qbar; 
initial Q=0;
initial Qbar=1; 
always @(posedge clk) begin Q=S|((~R)&Q); 
Qbar=~Q; 
end endmodule
```
# Developed by:BUSHPIKA C
# RegisterNumber:25007434
# RTL LOGIC FOR FLIPFLOPS
 
  <img width="1061" height="600" alt="image" src="https://github.com/user-attachments/assets/3b0c6b95-7759-456f-b485-1abe0d7658a8" />
# TIMING DIGRAMS FOR FLIP FLOPS

<img width="1007" height="146" alt="image" src="https://github.com/user-attachments/assets/d7c1d045-7d60-460e-b407-e99e06b56095" />
# RESULTS 
Thus the logic gate and timing diagram for Filpflop is verified.
