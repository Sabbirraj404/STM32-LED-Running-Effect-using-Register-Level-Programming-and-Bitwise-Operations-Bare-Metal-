# STM32 LED Running Effect (Bare Metal - GPIO)

This project demonstrates a simple LED running (shifting) effect using STM32F4 (STM32F446RE) with register-level programming (no HAL/LL). LEDs connected to GPIOA pins (PA5–PA8) turn ON one by one in sequence.

---

## Features

- Bare-metal (register-level) programming  
- Multiple GPIO control  
- LED shifting / running pattern  
- No HAL or external libraries  

---

## Working Principle

- Enable GPIOA clock  
- Configure PA5–PA8 as output pins  
- Turn ON one LED at a time  
- Create delay between transitions  
- Repeat continuously  

---

## Hardware Connections

| Pin  | Connection |
|------|-----------|
| PA5  | LED 1     |
| PA6  | LED 2     |
| PA7  | LED 3     |
| PA8  | LED 4     |

- All LEDs connected through resistors to GND  

---

## Code Explanation

### Clock Enable
- Enable GPIOA using RCC register  

### GPIO Configuration
- Set PA5–PA8 as output mode  

### LED Sequence
- Turn ON LEDs one by one using ODR  
- Delay creates visible shifting effect  

---

## Output

- LEDs connected to PA5 → PA8 glow sequentially  
- Creates a running / chasing light effect  

---

## Requirements

- STM32F446RE  
- 4 LEDs + resistors  
- ST-Link Debugger  
- Keil / STM32CubeIDE  

---

## Learning Outcomes

- Multi-pin GPIO control  
- Bit masking and shifting  
- Sequential logic in embedded systems  
- Bare-metal programming concepts  

---
=
