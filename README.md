# JK_FLIPFLOP
## Aim
To simulate and synthesis JK flipflop using vivado.

## Software Required
Vivado 2023.2 software

## Procedure:
STEP:1 Start the vivado software, Select and Name the New project.

STEP:2 Select the device family, device, package and speed.

STEP:3 Select new source in the New Project and select Verilog Module as the Source type.

STEP:4 Type the File Name and module name and Click Next and then finish button. Type the code and save it.

STEP:5 Select the run simulation and then run Behavioral Simulation in the Source Window and click the check syntax.

STEP:6 Click the simulation to simulate the program and give the inputs and verify the outputs as per the truth table.

STEP:7 compare the output with truth table.

![image](https://github.com/aashikriyaz/JK_FLIPFLOP/assets/165645036/056e7ae3-f0d8-4379-8573-13672b2b5948)


## Circuit Diagram
![image](https://github.com/aashikriyaz/JK_FLIPFLOP/assets/165645036/41ee771c-837d-4770-a85e-3c73344793f0)


## Truth Table

![image](https://github.com/aashikriyaz/JK_FLIPFLOP/assets/165645036/0623e08d-b24e-4b1c-8994-ebf3b5f99696)

## Program
```
module jkff(clk,j,k,rst,q );
input j,k,clk,rst;
output reg q;
always@(posedge clk)
begin
if(rst==1)
q=1'b0;
else
begin
case({j,k})
2'b00: q=q;
2'b01:q=1'b0;
2'b10:q=1'b1;
2'b11:q=~q;
endcase
end
end
endmodule
```
## Output

![image](https://github.com/aashikriyaz/JK_FLIPFLOP/assets/165645036/5d1c5f04-d8ac-4f69-b969-201e7905fdc3)


## Result
Thus the verilog program for JK flipflop has been simulated and verified successfully.

