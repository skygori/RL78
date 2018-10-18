# RL78

테스트 Renesas RL78

Device : R5F100GE

Serial UART0 test

CS+ for CA,CX 사용


Setting used for Code generation
--------------------------------
  * Serial Array Unit 0 is used as a UART
    * Single transfer mode
    * Data Lenght = 8 bits
    * Transfer direction setting : LSB first
    * Parity : None
    * Stop Bit : 1
    * Baud Rate : 9600
 
After generating the code Call the required functions in *R_MAIN_UserInit()*
 
```
void R_MAIN_UserInit(void)
{
   /* Start user code. Do not edit comment generated here */
   EI();
   R_UART0_Start();
   /* End user code. Do not edit comment generated here */
}
```


  
