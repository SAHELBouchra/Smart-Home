# Smart Home Project

<p align="center">
  <img width="285" height="294" alt="h" src="https://github.com/user-attachments/assets/5181bb5a-dc74-4d09-a992-57b28acf7000"
"/>
</p>

## Introduction

Welcome to my **Smart Home Project**! This system utilizes Arduino microcontrollers to monitor and control various home automation features. By integrating sensors, actuators, and communication modules, it provides a smart and safe environment for everyday living.

## Project Description

The goal of this project is to create a flexible and efficient smart home prototype that includes:

- Monitoring temperature and humidity levels
- Detecting motion in key areas
- Alerting users of potential gas leaks
- Allowing remote control of lighting systems
- Enabling secure access control through RFID

## Hardware Overview

### Microcontrollers

#### Arduino Uno
- Compact board powered by ATmega328P
- 14 digital inputs/outputs, 6 analog inputs, 32 KB flash memory
- Interfaces with sensors and output devices

<img width="474" height="405" alt="image" src="https://github.com/user-attachments/assets/cc56ddc1-6ed6-46b1-9174-bbe3845d8fc5" />

#### Arduino Mega
- More powerful board with ATmega2560
- 54 digital inputs/outputs, 16 analog inputs, 256 KB flash memory
- Used for handling multiple sensors and complex tasks

<img width="474" height="1024" alt="image" src="https://github.com/user-attachments/assets/a98e1864-f043-4021-a67d-533ddb74f14b" />

### Sensors

#### DHT11 (Temperature and Humidity)
- Measures ambient temperature and humidity levels
- Data shown on LCD and triggers specific actions

![DHT11](https://github.com/mariamAboujenane/SmartHome/assets/106840796/b677bd72-c8a4-4266-9442-9d96b99c9fa6)

#### PIR HC-SR501 (Motion Sensor)
- Detects movement through infrared sensing
- Activates lights or alarms based on detection

![PIR Sensor](https://github.com/mariamAboujenane/SmartHome/assets/106840796/ac053f37-4de0-4af4-92d2-53a9a087e127)

#### MQ-135 (Gas Sensor)
- Detects hazardous gases like CO, NH3, benzene
- Triggers buzzer alerts on gas leakage

![MQ-135](https://github.com/mariamAboujenane/SmartHome/assets/106840796/46766469-bfe4-4733-8388-d1182c3982a4)
![MQ-135 Alert](https://github.com/mariamAboujenane/SmartHome/assets/106840796/a12d2df9-63ff-4887-af93-77edd8051357)

#### 1838 IR Receiver
- Captures infrared signals from remotes
- Enables remote control of RGB LEDs

![IR Receiver](https://github.com/mariamAboujenane/SmartHome/assets/106840796/dac0a4be-454e-4135-a7a1-51b0b1920747)
![IR Receiver Setup](https://github.com/mariamAboujenane/SmartHome/assets/106840796/a2b140e5-d077-4b5b-ae6e-9299b7751166)
![IR Receiver Usage](https://github.com/mariamAboujenane/SmartHome/assets/106840796/550c4143-d663-4088-8664-362b6adbed63)

#### LDR (Light Dependent Resistor)
- Measures ambient light intensity
- Automatically controls garden lighting accordingly

![LDR](https://github.com/mariamAboujenane/SmartHome/assets/106840796/e3bbee1d-2e84-423f-8fe5-c009c39964ee)
![LDR in Action](https://github.com/mariamAboujenane/SmartHome/assets/106840796/56aea067-6df7-44a0-a69e-5180b4fa15f4)

### Actuators

#### Stepper Motor (Curtain Automation)
- Precisely moves curtains to desired positions
- Controlled via Arduino for open/close operations

![Stepper Motor](https://github.com/mariamAboujenane/SmartHome/assets/106840796/4383dade-24fc-4dfa-86b9-083376b48c60)

#### 8x8 LED Matrix
- Shows alerts and sensor data visually
- Activated based on motion detection

![8x8 LED Matrix](https://github.com/mariamAboujenane/SmartHome/assets/106840796/e67a9169-3ea2-4460-9ba6-86304a929369)
![8x8 LED in Action](https://github.com/mariamAboujenane/SmartHome/assets/106840796/0b203760-b181-49f1-969a-d538c4e5223d)

#### 16x2 LCD Display
- Displays real-time temperature, humidity, date, and time
- Serves as the main user interface

![16x2 LCD Display](https://github.com/mariamAboujenane/SmartHome/assets/106840796/d0b1f58e-2b99-421c-8bf4-189e6e34be9a)

### Communication Modules

#### RFID RC522
- Provides secure access control via RFID tags
- Manages door locking and logs entry events

![RFID RC522](https://github.com/mariamAboujenane/SmartHome/assets/106840796/33d28252-7f18-469b-84bf-f8112a0edae3)
![RFID in Action](https://github.com/mariamAboujenane/SmartHome/assets/106840796/a11d6dbb-5bb9-4493-af7e-1ff6a70b0902)

#### Bluetooth HC-05
- Enables wireless communication with smartphones
- Controls lighting and devices via a mobile app

![Bluetooth HC-05](https://github.com/mariamAboujenane/SmartHome/assets/106840796/0a216f96-4cdd-46be-aef1-6b2725925e56)
![Bluetooth in Action](https://github.com/mariamAboujenane/SmartHome/assets/106840796/3ff0e711-7b03-44ae-9ab3-7e4ac06a707b)

## Software Tools

- **Arduino IDE:** The main development environment for writing, compiling, and uploading code to Arduino boards.

### Libraries Utilized

- DHT Sensor Library (temperature & humidity)
- IRremote Library (infrared decoding)
- Stepper Library (motor control)
- LiquidCrystal Library (LCD interface)
- MFRC522 Library (RFID communication)
- SoftwareSerial Library (Bluetooth communication)

## System Architecture

The system features a modular design where sensors and actuators interface with Arduino microcontrollers. Data from sensors is processed and triggers automated responses. Communication protocols include I2C, SPI, and UART.


## Conclusion

This Smart Home project showcases the seamless integration of various technologies to create a functional, efficient, and user-friendly home automation system. By combining environmental sensors, actuators, wireless communication, and access control, it highlights how embedded systems can be used to improve comfort, security, and energy efficiency within a modern living space. The modular design allows for easy scalability and customization, making it adaptable to diverse user needs and future technological upgrades. Overall, the project reflects a strong understanding of system integration, real-world problem-solving, and the growing potential of IoT in everyday life.
