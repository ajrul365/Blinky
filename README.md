# Blinky

a) Project Configuration
  1. Select the board in the STM32CubeMX software
  2. Configure PC7 as GPIO_OUTPUT as it is connected to LED1 and other respective settings like setting Sys>Debug Pins to Serial Wire
  3. Configure clock to maximum 120 MHz
  4. Configure GPIO Mode of PC7 to Output Push Pull.
  5. Generate code using STM32CubeMX with basic headers and settings structure

b) Program Development
  1. Pin PC7 was initialized as an LED output with a delay of 1000ms, which is the delay between each blink
  2. The code was compiled, built and run into the board and uploaded to GitHub.
  3. Code:  HAL_GPIO_TogglePin(GPIOC, GPIO_PIN_7); // LED1
              HAL_Delay(1000);
