# SQUARE WAVE

## AIM:
Write a 8051 program to generate a square wave with frequency of 50khz

## APPARATUS REQUIRED
- Personal Computer  
- Keil µVision Software  

## PROGRAM:
```
CLR  P1.0          
MOV  TMOD, #01H    
AGAIN:
MOV  TL0, #0F7H  
MOV  TH0, #0FFH   
CPL  P1.0         
SETB TR0          
WAIT:
JNB  TF0, WAIT    
CLR  TR0          
CLR  TF0         
SJMP AGAIN       
END
```
### OUTPUT:
![WhatsApp Image 2025-10-18 at 16 03 16_9b38f22d](https://github.com/user-attachments/assets/8745cf3d-fff6-45bd-9548-ac774b01e1e3)

### RESULT:
Thus the 8051 prpgram to generate a square wave with the frequency of 50khz using 8051 KEIL was done and shown the output


