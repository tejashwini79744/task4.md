As per the Update given for the next task "Should Use the RISC-V Core Verilog netlist and testbench for functional Simulation.
Veriog code is being executed and the waveforms are generated using the gtkwave
Aim: To verify the Functional Simulation:-
Table of contents
1.RISC-V RV32I
2.BLOCK DIAGRAM OF RISC-V RV32I
3.INSTRUCTION SET OF RISC-V RV32I
4.FUNCTIONAL SIMULATION
4.1 About iverilog and gtkwave
4.2 Installing iverilog and gtkwave
4.3 The output waveform

1. RISC-V RV32I
   
   This project provides an insight into the working of a few important instructions of the instruction set of a Single cycle Reduced Instruction Set Computer - Five(RISC-V) Instruction Set Architecture suitable for use across wide-spectrum of Applications from low-power embedded devices to high-performance Cloud-based Server processors. The base RISC-V is a 32-bit processor with 31 general-purpose registers, so all the instructions are 32-bit long. Some Applications where the RISC-V processors have begun to make some significant threads are in Artificial intelligence and machine learning, Embedded systems, ultra-low power processing systems, etc.
2. BLOCK DIAGRAM OF RISC-V RV321
![image](https://github.com/tejashwini79744/task4.md/assets/161418020/a30a6893-7f36-4b11-8929-1a787a72e42e)
3. INSTRUCTION SET OF RISC-V RV32I
![image](https://github.com/tejashwini79744/task4.md/assets/161418020/ba97fc07-3c08-4197-bb27-6a7100176ecb)
![image](https://github.com/tejashwini79744/task4.md/assets/161418020/b95a842c-2dbe-47e7-a877-b9e9aacea453)
4. FUNCTIONAL SIMULATION
   
4.1 About iverilog and gtkwave

Icarus Verilog is an implementation of the Verilog hardware description language.

GTKWave is a fully featured GTK+ v1. 2 based wave viewer for Unix and Win32 which reads Ver Structural Verilog Compiler generated AET files as well as standard Verilog VCD/EVCD files and allows their viewing.

4.2 Installing iverilog and gtkwave

For Ubuntu

Open your terminal and type the following to install iverilog and GTKWave

$   sudo apt get update
$   sudo apt get install iverilog gtkwave
![image](https://github.com/tejashwini79744/task4.md/assets/161418020/0be11f08-4b4c-43c5-808e-08a15b17ff44)
To clone the repository and download the netlist files for simulation, enter the following commands in your terminal.

$ git clone https://github.com/task4.md

$ cd task4.md
![image](https://github.com/tejashwini79744/task4.md/assets/161418020/bf60bf52-d46d-48bf-a62d-258efd8a2899)
To simulate and run the Verilog code, enter the following commands in your terminal.

$ iverilog -o hello hello hello.v h

$ ./hello
![image](https://github.com/tejashwini79744/task4.md/assets/161418020/7f11fd07-e61f-426c-8122-72e65ac2d024)

To see the output waveform in gtkwave, enter the following commands in your terminal.

$ gtkwave hello.vcd
![image](https://github.com/tejashwini79744/task4.md/assets/161418020/68316def-4bbd-42c0-9583-73e280e80611)
4.3 The output waveform

The output waveform showing the instructions performed in a 5-stage pipelined architecture.

Instruction 1:add r6,r2,r1
![image](https://github.com/tejashwini79744/task4.md/assets/161418020/3be7e23b-20e9-4318-bc81-281e051dca91)
Instruction 2:sub r7,r1,r2
![image](https://github.com/tejashwini79744/task4.md/assets/161418020/4b185d1b-0f78-4d7b-a714-9e4c38ebe6fd)
Instruction 3:and r8,r1,r3 
![image](https://github.com/tejashwini79744/task4.md/assets/161418020/dcf85b07-a33c-41c9-9331-11099103e73a)
Instruction 4:or r9,r2,r5
![image](https://github.com/tejashwini79744/task4.md/assets/161418020/feb62fd2-de94-4cf0-9687-5f9b6a283d96)
Instruction 5:xor r10,r1,r4
![image](https://github.com/tejashwini79744/task4.md/assets/161418020/505e3113-9cde-466f-be7d-2259af65f0d1)
Instruction 6:slt r11,r2,r4
![image](https://github.com/tejashwini79744/task4.md/assets/161418020/ed44a6b1-af0a-42f2-9dce-19fa55270152)
Instruction 7:addi r12,r4,5
![image](https://github.com/tejashwini79744/task4.md/assets/161418020/d6c603ca-2156-4fc3-9fb4-a6576e090d64)
Instruction 8:sw r3,r1,2 
![image](https://github.com/tejashwini79744/task4.md/assets/161418020/7706d5bd-4e1f-40d9-967d-23a3dbe4941f)
Instruction 9:lw r13,r1,2
![image](https://github.com/tejashwini79744/task4.md/assets/161418020/f0570d7d-39a8-4707-a354-1b0707643334)
Instruction 10:beq r0,r0,15
![image](https://github.com/tejashwini79744/task4.md/assets/161418020/32fdc2a1-678f-4871-8320-cb210ad65eaa)
After branching, performing Instruction 11:add r14,r2,r2
![image](https://github.com/tejashwini79744/task4.md/assets/161418020/eaa45583-c84c-4d4e-99e3-aa60d724504a)
Full 5-stage instruction pipeline and pc-increment description Waveform
![image](https://github.com/tejashwini79744/task4.md/assets/161418020/b06a0232-363d-4317-a93a-8ee41ed69e3e)
![image](https://github.com/tejashwini79744/task4.md/assets/161418020/28749ad5-541a-493d-ae09-9f941dc78b9e)
![image](https://github.com/tejashwini79744/task4.md/assets/161418020/d412bfe2-c01f-477c-a08b-24415a52b7a1)





