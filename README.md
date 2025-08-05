
# 🌡️ Smart Home Climate Control System

This project is an embedded system designed to manage **temperature**, **security**, and **appliance control** in a smart home environment. It was developed as a final project for **ECE 36200 (Microcontroller Systems and Interfacing)** at **Purdue University**.

The system is built using the **Freescale HCS12/MC9S12 microcontroller**, programmed in **C and Assembly**, and tested in **CodeWarrior IDE**.

---

## 🎯 Project Objectives

- Monitor room temperature using a **potentiometer** or **ADC-based sensor**
- Allow secure access via a **user keypad** (password entry)
- Display system status and messages on **LCD**
- Control **stepper motors** and **alarms** for simulated smart devices
- Implement real-time features using **interrupts**
- Provide a basic **state machine** for smart appliance logic

---

## 🧰 Features

- 🔐 **Password-authenticated entry system**
- 🌡️ **Temperature monitoring** using ADC + potentiometer
- 🧼 **Washer state logic** with time tracking
- 🚨 **Alarm activation** with stop conditions
- 💡 **LCD display output** (via `lcddisp.c`)
- ⏱️ **Timer-based interrupt routines** for real-time behavior
- 🧭 **Stepper motor control** for simulating device movement
- 🧪 **Debug output** using `.dbg` and `.map` files

---

## 🗂️ Project Structure

```
Smart_Home_Climate/
├── Sources/                # All .asm and .c source files
│   ├── main.asm           # Main system logic
│   ├── IRQ_ISR.asm        # Interrupt Service Routines
│   ├── KEYPAD_FP.asm      # Keypad scanning
│   ├── pot.asm / potentiometer.c  # Temperature sensing
│   ├── stepperMOTOR.asm   # Motor control
│   └── washer_state.asm   # Appliance state logic
├── bin/                   # Compiled outputs & debug files
├── cmd/                   # CodeWarrior command files
├── prm/                   # Memory map configuration
├── Final_Project_Data/    # Project config and IDE support
├── smart home(final).mcp # CodeWarrior Project File
├── ECE 36200 Final Project 2.pdf  # Full project report
└── README.md              # Project summary
```

---

## 🛠️ Tools Used

- 🔄 **CodeWarrior IDE** (HCS12 variant)
- 🧠 **Assembly & Embedded C**
- 💾 **HCS12 MCU** platform
- 🧪 **Simulation & Debugging** via `.dbg` files

---

## 🔍 How to Run

1. Open the `.mcp` project file in **CodeWarrior IDE**
2. Connect your **MC9S12/HCS12 development board**
3. Build and flash the code
4. Use:
   - Keypad for input
   - Potentiometer or analog sensor for temperature
   - LCD screen for output
   - Observe motor/alarm responses

---

## 📄 Documentation

See [`ECE 36200 Final Project 2.pdf`](./ECE 36200 Final Project 2.pdf) for:
- System overview
- Circuit diagrams
- State diagrams
- Explanation of all modules
- Test cases and results

---

## 👨‍🎓 Author

**Amit Vardhan Suryadevara**  
Department of Electrical and Computer Engineering  
Purdue University, Indianapolis  
📧 avsuryad@purdue.edu

---

## 📚 Course Info

- **Course**: ECE 36200 – Microcontroller Systems and Interfacing  
- **Instructor**: Prof. John Lee
- **Institution**: Purdue University  
- **Semester**: Spring 2024

---

## 📝 License

This project is released for academic and learning purposes only.
