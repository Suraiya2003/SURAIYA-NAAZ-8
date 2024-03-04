# As per the Update given for the next task "Should Use the RISC-V Core Verilog netlist and testbench for functional Simulation.
# Veriog code is being executed and the waveforms are generated using the gtkwave

# Aim: To verify the Functional Simulation:-
# Table of contents
- [1.RISC-V RV32I](#1-RISC-V-RV32I)
 - [2.BLOCK DIAGRAM OF RISC-V RV32I](#2-BLOCK-DIAGRAM-OF-RISC-V-RV32I)
 - [3.INSTRUCTION SET OF RISC-V RV32I](#3-INSTRUCTION-SET-OF-RISC-V-RV32I)
 - [4.FUNCTIONAL SIMULATION](#4-FUNCTIONAL-SIMULATION)
    - [4.1 About iverilog and gtkwave](#41-About-iverilog-and-gtkwave)
    - [4.2 Installing iverilog and gtkwave](#42-Installing-iverilog-and-gtkwave)
    - [4.3 The output waveform](#43-The-output-waveform)
    ## 1. RISC-V RV32I

This project provides an insight into the working of a few important instructions of the instruction set of a Single cycle Reduced Instruction Set Computer - Five(RISC-V) Instruction Set Architecture suitable for use across wide-spectrum of Applications from low-power embedded devices to high-performance Cloud-based Server processors. The base RISC-V is a 32-bit processor with 31 general-purpose registers, so all the instructions are 32-bit long. Some Applications where the RISC-V processors have begun to make some significant threads are in Artificial intelligence and machine learning, Embedded systems, ultra-low power processing systems, etc.

## 2. BLOCK DIAGRAM OF RISC-V RV32I
<img width="526" alt="Screenshot 2024-03-04 210627" src="https://github.com/Suraiya2003/SURAIYA-NAAZ-8/assets/160725650/fd90ac63-84d9-401a-ac62-4b8c00f13337">


## 3. INSTRUCTION SET OF RISC-V RV32I
<img width="828" alt="Screenshot 2024-03-04 210958" src="https://github.com/Suraiya2003/SURAIYA-NAAZ-8/assets/160725650/7a9da4db-8e07-4c71-8f98-0279c32b72e9">
<img width="414" alt="Screenshot 2024-03-04 211051" src="https://github.com/Suraiya2003/SURAIYA-NAAZ-8/assets/160725650/3b781b80-e4aa-4003-9dbe-e23bc11cc35a">
### 4.1 About iverilog and gtkwave
- Icarus Verilog is an implementation of the Verilog hardware description language.
- GTKWave is a fully featured GTK+ v1. 2 based wave viewer for Unix and Win32 which reads Ver Structural Verilog Compiler generated AET files as well as standard Verilog VCD/EVCD files and allows their viewing.
  
### 4.2 Installing iverilog and gtkwave
- **For Ubuntu**

 Open your terminal and type the following to install iverilog and GTKWave
 ```
 $   sudo apt get update
 $   sudo apt get install iverilog gtkwave
 ```
![WhatsApp Image 2024-03-04 at 9 01 22 PM](https://github.com/Suraiya2003/SURAIYA-NAAZ-8/assets/160725650/af07f36e-c4f7-499c-a977-01dd2a0ef04f)
- **To clone the repository and download the netlist files for simulation, enter the following commands in your terminal.**

 ```
 $ git clone https://github.com/Suraiya2003/SURAIYA-NAAZ-8/blob/main/task4.md
 $ cd suraiya2003
```
![WhatsApp Image 2024-03-04 at 9 26 26 PM](https://github.com/Suraiya2003/SURAIYA-NAAZ-8/assets/160725650/2f8349bf-6f03-4607-b187-1ae8cf73eee1)
- **To simulate and run the Verilog code, enter the following commands in your terminal.**

```
$ iverilog -o hello hello.v hello_tb.v
$ ./hello
```
![WhatsApp Image 2024-03-04 at 9 36 50 PM](https://github.com/Suraiya2003/SURAIYA-NAAZ-8/assets/160725650/212f9428-25b6-491c-aaa3-ce26cd782788)
- **To see the output waveform in gtkwave, enter the following commands in your terminal.**

`$ gtkwave hello.vcd`


![WhatsApp Image 2024-03-04 at 9 39 55 PM](https://github.com/Suraiya2003/SURAIYA-NAAZ-8/assets/160725650/027d86a8-8d8f-41ff-a470-8d4b431d3b40)
### 4.3 The output waveform

 The output waveform showing the instructions performed in a 5-stage pipelined architecture.
 
 Instruction 1:add r6,r2,r1
 <img width="960" alt="Screenshot 2024-03-04 214136" src="https://github.com/Suraiya2003/SURAIYA-NAAZ-8/assets/160725650/226e1b93-bde9-4d11-b9ec-2dd17449cda3">
Instruction 2:sub r7,r1,r2 
<img width="960" alt="Screenshot 2024-03-04 214242" src="https://github.com/Suraiya2003/SURAIYA-NAAZ-8/assets/160725650/2cfdc1a7-f4a7-4fd0-b6b6-a85af435ab41">
Instruction 3:and r8,r1,r3
<img width="959" alt="Screenshot 2024-03-04 214321" src="https://github.com/Suraiya2003/SURAIYA-NAAZ-8/assets/160725650/a2143b75-466e-4d29-96f0-60f916f414dd">
Instruction 4:or r9,r2,r5 
<img width="959" alt="Screenshot 2024-03-04 214431" src="https://github.com/Suraiya2003/SURAIYA-NAAZ-8/assets/160725650/dbc791c1-fcbc-4924-862b-43f5ff4ada2c">
Instruction 5:xor r10,r1,r4
<img width="960" alt="Screenshot 2024-03-04 214528" src="https://github.com/Suraiya2003/SURAIYA-NAAZ-8/assets/160725650/3f0925cc-005b-4ba6-91d4-c05c1f302ce4">
Instruction 6:slt r11,r2,r4
<img width="757" alt="Screenshot 2024-03-04 214636" src="https://github.com/Suraiya2003/SURAIYA-NAAZ-8/assets/160725650/3631edb7-a824-4710-b226-a7a26d2504aa">
Instruction 7:addi r12,r4,5
<img width="854" alt="Screenshot 2024-03-04 214748" src="https://github.com/Suraiya2003/SURAIYA-NAAZ-8/assets/160725650/216cb80b-d5ae-40fc-93e9-fce5c9e492fd">
Instruction 8:sw r3,r1,2
<img width="858" alt="Screenshot 2024-03-04 214837" src="https://github.com/Suraiya2003/SURAIYA-NAAZ-8/assets/160725650/fec78ed3-f9e7-483e-9bf2-e963d40582bf">
Instruction 9:lw r13,r1,2
<img width="848" alt="Screenshot 2024-03-04 214921" src="https://github.com/Suraiya2003/SURAIYA-NAAZ-8/assets/160725650/ddd782bf-f751-434c-848a-15bbffb0489f">
Instruction 10:beq r0,r0,15
<img width="850" alt="Screenshot 2024-03-04 215021" src="https://github.com/Suraiya2003/SURAIYA-NAAZ-8/assets/160725650/329ea04c-5cc0-4f5e-b217-0d952bcefb25">
After branching, performing Instruction 11:add r14,r2,r2
<img width="850" alt="Screenshot 2024-03-04 215120" src="https://github.com/Suraiya2003/SURAIYA-NAAZ-8/assets/160725650/5b4fbbae-f324-4da0-90ba-e4ad2440815d">
Full 5-stage instruction pipeline and pc-increment description Waveform
<img width="849" alt="Screenshot 2024-03-04 215231" src="https://github.com/Suraiya2003/SURAIYA-NAAZ-8/assets/160725650/2d49a4f3-0b39-4db0-8d95-92b38f879a29">
![WhatsApp Image 2024-03-04 at 9 53 43 PM](https://github.com/Suraiya2003/SURAIYA-NAAZ-8/assets/160725650/0ecdd140-83b5-4569-ab53-886d27157798)
![WhatsApp Image 2024-03-04 at 9 58 37 PM](https://github.com/Suraiya2003/SURAIYA-NAAZ-8/assets/160725650/cbb4dd16-8eb4-449f-8223-63106d8a9b3f)
