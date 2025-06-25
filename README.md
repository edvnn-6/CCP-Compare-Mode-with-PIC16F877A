# CCP Compare Mode with PIC16F877A (LAB 12)

This project demonstrates the use of **Compare Mode** of the **CCP1 module** in the PIC16F877A. A timer compare match event is used to trigger periodic interrupts, and after 31 such events, an LED is toggled.

## 👨‍💻 Author
**Edvin Jose Vakaparamban**  
📅 LAB 12 – CCP Compare Mode

---

## 🔧 Description

- **Timer1** is used as a time base.
- **CCP1** is configured in **Compare Mode** with a special event trigger.
- **CCPR1** is set to 65000, meaning Timer1 triggers a match near overflow.
- An interrupt is generated on match, and after **31 matches**, the system toggles an LED on **RC4**.

This simulates a periodic timer-based action with precise interrupt-driven timing logic.

---

## 🧰 Hardware Requirements

- **PIC16F877A** Microcontroller
- **LED** with current-limiting resistor
- Breadboard, wires, and power supply
- Optional: Oscilloscope to observe toggling on RC4

---

## ⚙️ Features

- Timer1 counting in internal clock mode (16 MHz)
- Compare match using CCP1 generates interrupts
- LED toggles on RC4 after every 31 matches (programmable count)
- Fully interrupt-driven – no polling inside the main loop

---

## 🔌 Pin Configuration

| Signal       | PIC Pin |
|--------------|---------|
| LED Output   | RC4     |

---

