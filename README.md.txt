# Proteus_Simulation

"Proteus_Simulation" is a simple STM32 project designed and simulated using **Proteus 8.13**.  
It demonstrates how to toggle an LED connected to pin "PA0" of the "STM32F103C8" microcontroller using the "HAL (Hardware Abstraction Layer)" library.

---

## 🔧 Tools Used
- STM32CubeIDE — for code generation and compilation  
- Proteus 8.13 — for hardware simulation  
- STM32F103C8 — ARM Cortex-M3 microcontroller  
- HAL GPIO library — for controlling input/output pins  

---

## ⚙️ Project Description
This project toggles an LED connected to PA0 every second.  
It demonstrates basic GPIO output control using STM32 HAL functions:

c
while (1)
{
    HAL_GPIO_WritePin(GPIOA, GPIO_PIN_0, GPIO_PIN_SET);   // Turn ON LED
    HAL_Delay(1000);
    HAL_GPIO_WritePin(GPIOA, GPIO_PIN_0, GPIO_PIN_RESET); // Turn OFF LED
    HAL_Delay(1000);
}




🚀 How to Use

1. Open the project in STM32CubeIDE.
2. Build the project to generate the `.hex` file.
3. Open Proteus 8.13, add the STM32F103C8 component, and attach the generated `.hex` file.
4. Run the simulation — the LED connected to PA0 will blink every second.
  



📁 Folder Structure

Proteus_Simulation/
├── src/              # Source and header files
├── Doc/           # HAL and CMSIS libraries
├proteus_design
── .cproject          # Project configuration file
── .project           # STM32CubeIDE project definition
└──hex_output


🧠 Author

Bouchra — Embedded Systems Engineer
Designed for educational and research purposes.


