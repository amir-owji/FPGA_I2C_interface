# FPGA_I2C_interface
FPGA Based I2C Protocol Implementation with AHT10 Sensor
# I²C Master & Sensor Communication on FPGA (VHDL)

This project demonstrates a full VHDL-based implementation of the I²C protocol and its practical application by interfacing with the AHT10 temperature and humidity sensor. It is divided into two main parts:

---

##  Project Structure

### `I2C_master/`
A pure VHDL implementation of the I²C Master protocol, developed from scratch using a finite state machine (FSM). This module supports Start, Stop, Read, Write, and Re-Start conditions in compliance with I²C protocol timing.

**Files:**
- `i2c_master.vhd` – Core FSM implementation
- `fsm_diagram.png` – Visual representation of the FSM

---

### `I2C_with_AHT10/`
A complete sensor communication system that connects an AHT10 sensor to the FPGA via I²C and transmits the result over UART. Includes timing logic, UART transmitter, and I²C communication handler.

**Key Modules:**
- `AHT10.vhd` – Sensor state machine
- `i2c_com.vhd` – I²C transaction controller
- `uart_tx.vhd`, `main_uart.vhd` – UART output modules
- `mod_m_counter.vhd` – Timing generator

---

### `project_documentation/`
Includes the full English PDF report with detailed explanations, diagrams, and project structure.

- `I2C_FPGA_Project.pdf` – Full project documentation
- `fsm_diagram.png` – Repeated here for reference

---

##  Key Concepts

- FSM-based I²C Master implementation
- Multi-byte read/write operations
- AHT10 sensor interface via I²C
- UART transmission for sensor data
- Modular and reusable VHDL design

---

##  Contact

Created by **Amir Owji**  
•	Email: amir.owji003@gmail.com
•	LinkedIn: www.linkedin.com/in/amir-hossein-owji
•	GitHub: github.com/amir-owji

---
##  Acknowledgements

Part of the I²C implementation logic and structure in this project was inspired by the following educational course:

- **"I2C Interface in FPGA with VHDL – Practical Implementation and Testing"**  
  Instructor: [Firouz Hemmati]  
  Platform: [Faradars – www.faradars.org]

This course provided valuable insight into FSM-based protocol implementation and practical testing using real modules.  


##  License

This project is open-source for educational and non-commercial use.
