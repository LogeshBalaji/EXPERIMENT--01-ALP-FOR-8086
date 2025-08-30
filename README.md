<img width="1919" height="1015" alt="Screenshot 2025-08-30 135745" src="https://github.com/user-attachments/assets/a14da7a0-dd42-459f-a99c-8ba089a8c76a" /># EXPERIMENT--01-ALP-FOR-8086
Name : Shehan Shajahan
Roll no : 212223240154
Date of experiment : 30/08/2025





## Aim: To Write and execute ALP on fundamental arithmetic and logical operations
## Components required: 8086  emulator 
## Theory 
Running The Emulator (emu8086) Intro 8086 Microprocessor Emulator, also known as EMU8086, is an emulator of the program 8086 microprocessor. It is developed with a built-in 8086 assembler. This application is able to run programs on both PC desktops and laptops. This tool is primarily designed to copy or emulate hardware. These include the memory of a program, CPU, RAM, input and output devices, and even the display screen. There are instructions to follow when using this emulator. It can be executed into one of the two ways: backward or forward. There are also examples of assembly source code included. With this, it allows the programming of assembly language, reverse engineering, hardware architecture, and creating miniature operating system (OS). The user interface of 8086 Microprocessor Emulator is simple and easy to manage. There are five major buttons with icons and titles included. These are “Load”, “Reload”, “Step Back”, “Single Step”, and “Run”. Above those buttons is the menu that includes “File”, “View”, “Virtual Devices”, “Virtual Drive”, and “Help”. Below the buttons is a series of choices that are usually in numbers and codes. At the leftmost part is an area called “Registers” with an indication of either “H” or “L”. The other side is divided into two, which enables users to manually reset, debug, flag, etc. What is 8086 emulator emu8086 is an emulator of Intel 8086 (AMD compatible) microprocessor with integrated 8086 assembler and tutorials for beginners. Emulator runs programs like the real microprocessor in step-by-step mode. it shows registers, memory, stack, variables and flags.


 ## Running the Emulator :
1.	Download and install emu8086 (www.emu8086.com) It is usually installed in C:\EMU8086 subfolder in the “Windows” directory
2.	  Run  emu8086 icon (on the desktop or in the c:\EMU8086 folder of window) It has green color 
 
 
3.		write the code for the appropriate program for ADDITION,SUBTRACTION, MULTIPLICATION,  DIVISION operations 

4.	 Compile the program and check for the errors 
5.	Run (once there is no syntax error) 

6.	Click OK to see/view the output of your program on the Emulator screen. 


7.	After running the program, another menu screen will be displayed, where you have the option to “View” symbol table,
8.	 


![image](https://user-images.githubusercontent.com/36288975/189273263-d65baae9-4b8f-4723-afb3-c0ffa4052b04.png)











9.	Click on emulate to start emulation 








![image](https://user-images.githubusercontent.com/36288975/189273273-9bb36ec1-e2e8-4892-8d35-37707332bfdc.png)








10.	If no errors are found click on run the program and check the status of various flags in the flags tab as shown below 






![image](https://user-images.githubusercontent.com/36288975/189273277-113a2a33-4a40-4ff8-95a5-ecd3a1f504fe.png)







## Programs for arithmetic  operations

## Addition  of 8 bit ALP 
```
MOV CL,00
MOV AX,[3001H]
MOV BX,[3003H]
ADD AX,BX
JNC Loop
INC CL
Loop:
MOV [3005H],AX
MOV [3007H],CL
HLT    
```

## Output  
<img width="1919" height="1021" alt="Screenshot 2025-08-30 134819" src="https://github.com/user-attachments/assets/12396533-1748-4c2c-b038-cd5b629b0974" />

 
## Subtraction   of 8 bit numbers  ALP 
```
MOV CL,00
MOV AX,[3001H]
MOV BX,[3003H]
SUB AX,BX
JNC Loop
INC CL  
NOT AX
INC AX
Loop:
MOV [3005H],AX
MOV [3007H],CL
HLT 
```
 
## Output  
<img width="1919" height="1015" alt="Screenshot 2025-08-30 135745" src="https://github.com/user-attachments/assets/b6125f22-1fde-4160-a066-f9a8e65fe4e8" />

## Multiplication alp 
```
MOV AX,[3001H]
MOV BX,[3003H]
MUL BX
MOV [3005H],AX
MOV [3007H],DX
HLT  
```
## Output  
<img width="1919" height="1017" alt="Screenshot 2025-08-30 135949" src="https://github.com/user-attachments/assets/782a79bd-bdea-42cb-b249-cfb22a02b14f" />


## Division alp 
```
MOV AX,[3001H]
MOV BX,[3003H]
DIV BX
MOV [3005H],AX
MOV [3007H],DX
HLT
```

## Output  
<img width="1919" height="1021" alt="Screenshot 2025-08-30 140343" src="https://github.com/user-attachments/assets/93a4e987-7a55-4733-bd91-82db6e567ef5" />

## Logical Operations
## AND Operator
```
MOV AX,[3001H]
MOV BX,[3003H]
AND AX,BX
MOV [3005H],AX
HLT
```
## Output
<img width="1919" height="1017" alt="Screenshot 2025-08-30 142027" src="https://github.com/user-attachments/assets/01a7422d-1e91-4fbb-8960-5ed7e449d777" />

## NAND Operator
```
MOV AX,[3001H]
MOV BX,[3003H]
AND AX,BX
NOT AX
MOV [3005H],AX
HLT
```
## Output
<img width="1919" height="1015" alt="Screenshot 2025-08-30 143257" src="https://github.com/user-attachments/assets/3a0abb35-f9bb-4bef-9623-2186b615d019" />

## OR Operator
```
MOV AX,[3001H]
MOV BX,[3003H]
OR AX,BX
MOV [3005H],AX
HLT

```
## Output
<img width="1919" height="1017" alt="Screenshot 2025-08-30 141349" src="https://github.com/user-attachments/assets/0c63e6d8-06ed-4011-9e09-29175a930765" />

## NOR Operator
```
MOV AX,[3001H]
MOV BX,[3003H]
OR AX,BX
NOT AX
MOV [3005H],AX
HLT
```
## Output
<img width="1919" height="1020" alt="Screenshot 2025-08-30 141453" src="https://github.com/user-attachments/assets/032cf49a-8324-4e61-ba9d-3e39aac36e30" />

## NOT Operator
```
MOV AX,[3001H]
NOT AX
MOV [3003H],AX
HLT
```
## Output
<img width="1919" height="1016" alt="Screenshot 2025-08-30 141638" src="https://github.com/user-attachments/assets/df269066-cbe9-474e-bcf3-b23701f8f75a" />

## XOR Operator
```
MOV AX,[3001H]
MOV BX,[3003H]
XOR AX,BX
MOV [3005H],AX
HLT
```
## Output
<img width="1919" height="1018" alt="Screenshot 2025-08-30 141731" src="https://github.com/user-attachments/assets/71088b8f-8380-4bfa-b88d-959db2276328" />

## XNOR Operator
```
MOV AX,[3001H]
MOV BX,[3003H]
XOR AX,BX
NOT AX
MOV [3005H],AX
HLT
```
## Output
<img width="1919" height="1020" alt="Screenshot 2025-08-30 141915" src="https://github.com/user-attachments/assets/10d78ee9-fd86-4db2-b689-ba58625f0000" />


## Result :
Successfully executed ALP on fundamental arithmetic and logical operations.
 








