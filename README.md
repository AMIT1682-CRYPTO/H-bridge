Open-Source H-Bridge Motor Controller (IRF3205 + IR2104S)

An open-source, high-current H-Bridge DC motor driver based on IRF3205 MOSFETs and IR2104S half-bridge gate drivers. Designed for robotics, RC vehicles, and DIY motor control projects.

This controller supports bidirectional DC motor control with PWM speed regulation and can be driven directly from common microcontrollers (Arduino, ESP32, STM32, PIC, AVR, etc.)

 Features
✔ Up to 30A peak (with proper cooling and PCB copper area)
✔ Uses N-channel MOSFETs in full H-Bridge configuration
✔ Fast switching and low MOSFET losses due to Schottky freewheel diodes
✔ Gate driver isolation using dual IR2104S high/low-side drivers
✔ 5V onboard regulator (78L05) for logic power
✔ Suitable for PWM control, robotics, RC cars, etc.

Core components:
MOSFETs	4 × IRF3205 (N-Channel, 55V, 110A)
Gate Drivers	2 × IR2104S
Freewheel Diodes	4 × 1N5822 Schottky
Bulk Capacitors	2 × 470µF / 25V electrolytic
Logic Filter Capacitor	1 × 100µF / 16V
Decoupling Capacitors	1 × 0.1µF 
Bootstrap Capacitors 2 × 1µF 0805 MLCC
Bootstrap Diodes	2 × 1N5822 Schottky
5V Regulator	78L05
Gate Resistors	4 × 10Ω
INPUT Pull-downs	2 × 10kΩ
Status LED	1 × 3mm LED + 1kΩ resistor


Motor Voltage	6V – 18V DC
Logic Voltage	5V
Continuous Current	15–20A (depending on cooling)
Peak Current	~30A (short duration)
PWM Frequency	up to 20–25 kHz
12V EXTERNAL DRIVE SUPPLY

Pinout / Control Interface

INA: H-Bridge input A 
INB: H-Bridge input B
SD1: SHUTDOWN PIN FOR DRIVER A (ACTIVE LOW)
SD2: SHUTDOWN PIN FOR DRIVER B (ACTIVE LOW)
5V: SUPPLY FOR MICROCONTROLLER 
GND: Common ground
