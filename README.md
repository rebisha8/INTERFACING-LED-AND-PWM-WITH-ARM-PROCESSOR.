# INTERFACING-OF-ADC-WITH-ARM-PROCESSOR

## AIM: 
To interface and toggle the led with ARM LPC 1768 microprocessor           
           
## COMPONENTS REQUIRED:

## Hardware:
ARM LPC1343 / LPC1768
LCD module

## Software:
Coocox IDE

## PROCEDURE:

- Step 1: Go to start All programs  COIDE.
  
- Step 2: Give a suitable file name for your project and give the destination folder and then next. Step 3: Go to chip NXP LPC 13XX  LPC1343  Next.
  
- Step 4: Select the required library file (SYSCON and GPIO) from the repository. Step 5: A new project will be created.
  
- Step 6: Double click on main.c and type the program.
  
- Step 7: Add the required library source file to the project (Right click on include Add file to group and add the source file).
  
- Step 8: Build the program using build option.
  
- Step 9: Flash the program by clicking on download code to flash. Step 10: Interface the required component and note down the output.

## ADD FILES:

Repository:

CMSIS core, CMSIS boot, common header files, SYSCON, GPIO.

## Source files:

simple example.c, Uart Receiver interrupt.c, lcd.c, lcd.h
 
## DIAGRAM:

<img width="1440" height="770" alt="image" src="https://github.com/user-attachments/assets/d7ba3987-3ebf-4037-a84b-de3986df0bdb" />
 
## PROGRAM:
```C
#include"lcd.h" 
void ADCExp(); 
int main(void) 
{ 
ReceiverInterrupt(); 
init_lcd(); 
lcd_putstring(LINE1, "RAANA ADC DEMO "); 
ADCExp(); 
while(1) 
{ 
} 
}
```

## OUTPUT

<img width="625" height="448" alt="image" src="https://github.com/user-attachments/assets/a42b65d2-3684-4d59-bae7-fb80d91e8574" />
 
## RESULTS
Thus, an embedded c program to interface ADC with ARM processor was executed and output was verified successfully.






