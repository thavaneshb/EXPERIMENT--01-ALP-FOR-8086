# EXPERIMENT--01-ALP-FOR-8086

## Developed by:
```
Name :thavanesh
Roll no:212224040352
```




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







# Programs for arithmetic  operations

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
MOV [3007H],CL
HLT 
```


## Output  
 <img width="1919" height="1127" alt="Screenshot 2025-08-22 154210" src="https://github.com/user-attachments/assets/fc97cebd-6672-4d9d-a855-e80a348582f6" />

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
<img width="1919" height="1128" alt="Screenshot 2025-08-22 160956" src="https://github.com/user-attachments/assets/b1dfa8f0-95f3-4552-a4f4-7a0cc42e3a27" />

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
<img width="1919" height="1124" alt="Screenshot 2025-08-22 162728" src="https://github.com/user-attachments/assets/7f832912-2ab0-465b-b4e4-379e4ee630d6" />


## Division alp 
```
MOV AX,[3001H]
MOV BX,[3003H]
DIV BX
MOV [3005H],AX
MOV [3007H],DX
HLT
```
## Output  

<img width="1919" height="1124" alt="Screenshot 2025-08-22 162854" src="https://github.com/user-attachments/assets/140b48f7-fa59-406e-aefd-b2108e1413a3" />

# LOGICAL OPERATIONS

## TRUTH TABLE FOR LOGICAL OPERATIONS

![symbols-truth-tables-of-common-logic-gates](https://github.com/user-attachments/assets/6caae067-aca0-4b9c-83e3-d22429c1b3ec)



## AND alp
```
MOV AX,[3001H]
MOV BX,[3003H]
AND AX,BX
MOV [3005H],AX
HLT
```
## Output
<img width="1919" height="1125" alt="Screenshot 2025-08-29 153617" src="https://github.com/user-attachments/assets/5ababc18-7a91-43be-9144-db10836a3dc6" />


## OR alp
```
MOV AX,[3001H]
MOV BX,[3003H]
OR AX,BX
MOV [3005H],AX
HLT
```
## Output
<img width="1919" height="1130" alt="Screenshot 2025-08-29 153720" src="https://github.com/user-attachments/assets/fc6eed27-dceb-43c1-883d-982f8d85a06b" />


## NAND alp
```
MOV AX,[3001H]
MOV BX,[3003H]
AND AX,BX
NOT AX
MOV [3005H],AX
HLT
```
## Output
<img width="1919" height="1128" alt="Screenshot 2025-08-29 153824" src="https://github.com/user-attachments/assets/c5973365-3bea-4348-8395-cc6253104cf6" />


## NOR alp
```
MOV AX,[3001H]
MOV BX,[3003H]
OR AX,BX
NOT AX
MOV [3005H],AX
HLT
```
## Output
<img width="1920" height="1131" alt="Screenshot 2025-08-29 153525" src="https://github.com/user-attachments/assets/fda88936-7740-4f5f-a1a3-c5e65ba199cc" />


## NOT alp
```
MOV AX,[3001H]
MOV BX,[3003H]
NOT AX
MOV [3005H],AX
HLT
```
## output
<img width="1919" height="1128" alt="Screenshot 2025-08-29 154610" src="https://github.com/user-attachments/assets/8c678f13-8ff0-4f69-bef8-067eebf5228b" />


## XOR alp
```
MOV AX,[3001H]
MOV BX,[3003H]
XOR AX,BX
MOV [3005H],AX
HLT
```
## output

<img width="1919" height="1132" alt="Screenshot 2025-08-29 154841" src="https://github.com/user-attachments/assets/0a969de6-0da8-4a09-949c-3ede57e28f52" />


## XNOR alp
```
MOV AX,[3001H]
MOV BX,[3003H]
XOR AX,BX
NOT AX
MOV [3005H],AX
HLT
```
## output

<img width="1918" height="1130" alt="Screenshot 2025-08-29 154938" src="https://github.com/user-attachments/assets/5b8085bc-dd02-44d4-8e6b-44f4e3b11dae" />


## Result :
 
The Write and execute ALP on fundamental arithmetic and logical operations is executed successfully.








