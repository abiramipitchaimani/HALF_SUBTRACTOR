# HALF_SUBTRACTOR

## AIM:
To simulate and synthesis Half subractor using Xilinx ISE.
## APPARATUS REQUIRED: 
Xilinx 14.7 Spartan6 FPGA
## PROCEDURE: 
### STEP:1 
Start the Xilinx navigator, Select and Name the New project.
### STEP:2 
Select the device family, device, package and speed. 
### STEP:3 
Select new source in the New Project and select Verilog Module as the Source type.
### STEP:4 
Type the File Name and Click Next and then finish button. Type the code and save it. 
### STEP:5 
Select the Behavioral Simulation in the Source Window and click the check syntax. 
### STEP:6 
Click the simulation to simulate the program and give the inputs and verify the outputs as per the truth table.
### STEP:7 
Select the Implementation in the Sources Window and select the required file in the Processes Window.
### STEP:8 
Select Check Syntax from the Synthesize XST Process. Double Click in the Floorplan Area/IO/Logic-Post Synthesis process in the User Constraints process group. UCF(User constraint File) is obtained.
### STEP:9 
In the Design Object List Window, enter the pin location for each pin in the Loc column Select save from the File menu.
### STEP:10 
Double click on the Implement Design and double click on the Generate Programming File to create a bitstream of the design.(.v) file is converted into .bit file here.
### STEP:11 
Load the Bit file into the SPARTAN 6 FPGA
### STEP:12 
On the board, by giving required input, the LEDs starts to glow light, indicating the output.
# Truth Table
![image](https://github.com/RESMIRNAIR/HALF_SUBTRACTOR/assets/154305926/d0d5980a-6bcf-4ede-a54e-6aae3fb5f5f2)
# Circuit Diagram
![image](https://github.com/RESMIRNAIR/HALF_SUBTRACTOR/assets/154305926/df70da69-5a12-4a0d-ab84-a98dad3f7e70)
![image](https://github.com/RESMIRNAIR/HALF_SUBTRACTOR/assets/154305926/2f2d6a4d-9eda-4165-8579-1d7490b5fe97)
# PROGRAM:
```
 SUBMITTED BY:
   P.ABIRAMI
   212222060006
```
```
module half_subractor(a,b,difference,borrow);
       input a,b;
       output difference,borrow;
       wire w;
       xor g1(difference,a,b);
       and g2(borrow,w,b);
       not g3(w,a);
 endmodule
```
# OUTPUT:
![Screenshot 2024-03-17 194002](https://github.com/abiramipitchaimani/HALF_SUBTRACTOR/assets/163704307/27b291a2-8dfb-42dd-9a6f-24c0cdc74f65)
# RESULT:
Hence, the stimulation and synthesis of a half subractor was run successfully by using Xilinx ISE.
