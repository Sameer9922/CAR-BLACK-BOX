# 🚗 CAR Black Box

An embedded automotive event-logging system designed to monitor and record vehicle-related parameters and events. The project uses a PIC18F4580 microcontroller with peripherals such as UART, I2C, RTC, EEPROM, and LCD for data acquisition, storage, and display.

## 📌 Features

- Real-time monitoring of vehicle parameters
- Event logging and retrieval
- Date and time tracking using RTC
- Persistent event storage using EEPROM
- LCD-based display interface
- UART communication for data transfer/debugging
- Menu-based user interaction
- Embedded C firmware for microcontroller control

## 🛠️ Hardware & Technologies

### Microcontroller
- PIC18F4580

### Programming
- Embedded C

### Peripherals & Interfaces
- UART
- I2C
- RTC
- EEPROM
- LCD
- GPIO

### Development Tools
- MPLAB X IDE
- XC8 Compiler

## 🏗️ System Overview

```text
             ┌─────────────────────┐
             │    PIC18F4580       │
             │    Microcontroller  │
             └──────────┬──────────┘
                        │
       ┌────────────────┼────────────────┐
       │                │                │
       ▼                ▼                ▼
    Sensors            RTC             EEPROM
       │                │                │
       │                │                │
       └────────────────┼────────────────┘
                        │
                        ▼
                     LCD
                        │
                        ▼
                 Event Display
                        │
                        ▼
                      UART
