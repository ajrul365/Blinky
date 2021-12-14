# Blinky

a)	Project Configuration
  1.	Select the board in the STM32CubeMX software
  2.	Configure PC7 and PC13 as GPIO_OUTPUT and GPIO_EXTI13 respectively and other respective settings like setting Sys>Debug Pins to Serial Wire
  3.	Configure clock to 120 MHz
  4.	Configure GPIO Mode of PC7 and PC13 to Output Push Pull and External Interrupt Mode with Rising edge trigger detection, respectively
  5.	Generate code using STM32CubeMX with basic headers and settings structure


b)	Program Development
  1.	Pin PC7 was initialized as an LED output with a delay of 1000ms, which is the delay between each blink
  2.	Pin PC13 is the switch selection to activate the blinking function.
  3.	The code was compiled, built and run into the board and uploaded to GitHub.
  4.	Code:  HAL_GPIO_TogglePin(GPIOC, GPIO_PIN_7);
           HAL_Delay(1000);
