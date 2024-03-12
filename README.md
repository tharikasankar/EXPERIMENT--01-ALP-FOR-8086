# EXPERIMENT--01-ALP-FOR-8086

Name : Tharika S

Roll no : 212222230159

Date of experiment : 29/02/2024





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

## Addition  
```python
org 100h
MOV al,11h;
MOV bl,20h;
ADD al,bl;
MOV [6379h],al;
ret
```
## Output  
![image](https://github.com/tharikasankar/EXPERIMENT--01-ALP-FOR-8086/assets/119475507/def345e3-2e91-40c1-9059-74931d1ea8cd)

 
## Subtraction 
```python
org 100h
MOV al,20h;
MOV bl,[8778h];
SUB bl,al;
MOV [8798h],bl;
ret
```
## Output
![image](https://github.com/tharikasankar/EXPERIMENT--01-ALP-FOR-8086/assets/119475507/ccb60854-f420-442a-99b2-d3da73f84f8a)


## Multiplication
```python
org 100h
MOV al,13h;
MOV bl,2h;
MUL bl;
MOV [6063h],bl;
ret
```
 ## Output  
![image](https://github.com/tharikasankar/EXPERIMENT--01-ALP-FOR-8086/assets/119475507/3cbdd0fd-6c7d-4747-9188-c6df37e13044)


## Division
```python
org 100h
MOV al,26h;
MOV bl,[2369h];
DIV bl;
MOV [2399h],al;
ret
```
## Output
![image](https://github.com/tharikasankar/EXPERIMENT--01-ALP-FOR-8086/assets/119475507/1a44fd4e-609e-4e1c-a642-76effbd8aaab)

## Programs for logical  operations

## AND
```python
org 100h
MOV bx,1000h;
AND bx,1111h;
MOV [0040h+02],bx;
ret
```
## Output 
![image](https://github.com/tharikasankar/EXPERIMENT--01-ALP-FOR-8086/assets/119475507/aa5a3832-6b9d-4f9f-8541-20d16d7dd24c)


## OR
```python
org 100h
MOV ax,[0070h];
MOV bx,1000h;
OR ax,bx;
MOV [0060h],ax;
ret
```
## Output
![image](https://github.com/tharikasankar/EXPERIMENT--01-ALP-FOR-8086/assets/119475507/aacea97c-846f-414b-af65-845ed6128e38)

## NOT
```python
org 100h
MOV bx,0060h;
MOV ax,[bx]; 
NOT al;
MOV [0060h+04],ax;
ret
```
## Output
![image](https://github.com/tharikasankar/EXPERIMENT--01-ALP-FOR-8086/assets/119475507/a3353470-e3cc-49c2-be96-2295d037a973)


## XOR
```python
org 100h
MOV bx,0050h;
MOV ax,[bx]; 
XOR ax,bx;
MOV [0050h+03],ax;
ret
```
## Output
![image](https://github.com/tharikasankar/EXPERIMENT--01-ALP-FOR-8086/assets/119475507/d13f5ea9-105e-469d-9463-14026890b9a1)


## Result :
Thus, ALP for fundamental arithmetic and logical operations are executed successfully.
