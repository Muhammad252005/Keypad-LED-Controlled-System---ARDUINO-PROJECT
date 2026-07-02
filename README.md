# Keypad-Controlled LED Brightness and 7-Segment Display System using Arduino

## Overview

The **Keypad-Controlled LED Brightness and 7-Segment Display System** is an Arduino-based embedded systems project that demonstrates the integration of multiple input and output peripherals within a single application. Using a **4×4 matrix keypad**, the system accepts numeric user input (0–9), displays the selected number on a **7-segment display**, and simultaneously adjusts the brightness of an LED using **Pulse Width Modulation (PWM)**.

This project highlights fundamental embedded systems concepts, including keypad interfacing, digital display control, PWM-based brightness regulation, and coordinated input–output processing.

---

# Project Objectives

The primary objectives of this project are to:

* Interface a 4×4 matrix keypad with an Arduino Uno
* Read and interpret numeric keypad inputs
* Display entered numbers on a 7-segment LED display
* Control LED brightness using PWM (`analogWrite`)
* Map a single user input to multiple hardware outputs
* Strengthen understanding of embedded input–output integration

---

# Hardware Components

* Arduino Uno
* 4×4 Matrix Keypad
* 1-Digit 7-Segment Display
* LED
* 220 Ω Resistors
* Breadboard
* Jumper Wires
* 9V Battery
* 9V Battery Clip with DC Barrel Jack

---

# Circuit Diagram

The complete circuit diagram for this project is included in this repository.
![circuit_diagram]()
Additional hardware images and wiring references are also provided to assist with assembly and verification.

---

# System Operation

## 1. Keypad Input Detection

The 4×4 matrix keypad is connected to the Arduino through dedicated row and column pins. Using the Arduino **Keypad** library, the microcontroller continuously scans the keypad matrix to detect user key presses.

When a numeric key (0–9) is pressed, the corresponding value is identified and processed in real time.

---

## 2. Numeric Display

Once a valid numeric key is detected, the Arduino activates the appropriate segments of the 7-segment display to visually present the selected digit.

This provides immediate visual confirmation of the user's input.

---

## 3. LED Brightness Control

The same keypad input is simultaneously used to regulate the brightness of an LED.

Brightness levels are mapped proportionally to the entered numeric value:

* Lower numbers produce lower LED brightness.
* Higher numbers generate progressively brighter illumination.
* The maximum numeric value corresponds to full LED intensity.

LED brightness is controlled using Arduino's **Pulse Width Modulation (PWM)** through the `analogWrite()` function, enabling smooth and efficient brightness adjustment.

---

## 4. Serial Monitoring

For debugging and system validation, the Arduino Serial Monitor continuously logs the keypad inputs as they are detected.

This allows developers to monitor system behavior and verify correct operation during testing.

---

# Source Code

The complete Arduino source code for this project is available in the repository's [code](code/keypad_led_controlled_project_on_6th_november_2025.ino) directory.

---

# Demonstration

A demonstration video illustrating the complete operation of the system is included in this repository.

The demonstration showcases:

* Numeric keypad input
* Real-time 7-segment display updates
* PWM-controlled LED brightness adjustment
* Integrated input and output operation

---

# Learning Outcomes

This project provided practical experience in several key embedded systems concepts, including:

* Matrix keypad interfacing
* Digital input scanning techniques
* 7-segment display control
* Pulse Width Modulation (PWM)
* Multi-output hardware control
* Embedded system debugging using the Serial Monitor
* Coordinating multiple peripherals within a single application

---

# Challenges Encountered

Several technical challenges were addressed during development, including:

* Correctly mapping keypad key codes to numeric values
* Synchronizing keypad input with display updates
* Coordinating simultaneous LED brightness control and display operation
* Managing multiple hardware peripherals efficiently

Addressing these challenges strengthened practical skills in embedded software design and hardware integration.

---

# Technical Highlights

* Arduino Embedded Programming
* Matrix Keypad Interfacing
* 7-Segment Display Control
* Pulse Width Modulation (PWM)
* Digital Input Processing
* Multi-Peripheral Integration
* Real-Time Embedded Systems
* Hardware and Software Integration

---

# Future Enhancements

Potential improvements for future versions include:

* Support for alphabetic keypad inputs (A–D, *, #)
* OLED or LCD display for enhanced user feedback
* Software-based keypad debouncing
* Multi-digit 7-segment display support
* Configurable brightness scaling
* EEPROM storage for user settings
* Wireless control via Bluetooth or Wi-Fi
* Interactive menu system using the keypad

---

# Project Status

**Completed**

This project successfully demonstrates the integration of keypad input, digital display control, and PWM-based LED brightness regulation in an embedded system. It provides a solid foundation for more advanced human–machine interface (HMI) applications using Arduino.

---

# Author

**Muhammad Musa**

**Computer Engineering Student | Embedded Systems | Arduino | Microcontrollers | IoT**

Passionate about developing intelligent embedded solutions that combine efficient hardware design with reliable software implementation.
