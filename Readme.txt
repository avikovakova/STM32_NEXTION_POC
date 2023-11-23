This Project is an example for working with a nextion NX4827p042 screen.

UART COMMECT - when working with uart do not forget to add to 'stm32h7xx_it.c' file in the 'void HardFault_Handler(void)' function the reset command 'NVIC_SystemReset();' in case the uart buffer have overflow and the code jumps to that function.