# Wio-WM1110-Quick-Start-Guide-for-Seamless-Integration

![alt text](https://hackster.imgix.net/uploads/attachments/1662437/proj_pic_jMd411WgYU.JPG?auto=compress%2Cformat&w=740&h=555&fit=max)

The seeed studio Wio-WM1110 Dev Kit is based on the Wio-WM1110 Wireless Module, which integrates both a Semtech LoRa® transceiver and a multi-purpose radio front-end for geolocation functionalities. The LoRa® transceiver enables low-power, high-sensitivity network coverage, while GNSS (GPS/BeiDou) and Wi-Fi scanning work together to offer comprehensive location coverage. Additionally, the Dev Kit provides connectivity options for a variety of peripherals, making it a versatile platform for developing diverse IoT applications.

The Wio-WM1110 is a powerful fusion positioning module designed for developing low-power, long-range IoT applications. It combines the capabilities of the Semtech LR1110 LoRa transceiver and the Nordic nRF52840 microcontroller, offering a comprehensive solution for building connected devices with the following features:

Long-range wireless communication: Utilizing Semtech's LoRa technology, the Wio-WM1110 enables low-power communication over vast distances, making it ideal for connecting devices in remote locations.
Global Navigation Satellite System (GNSS): Integrated GNSS support, including GPS and BeiDou, provides accurate location tracking capabilities for your IoT devices.
Wi-Fi connectivity: In addition to LoRaWAN and GNSS, the Wio-WM1110 also offers Wi-Fi connectivity, providing another option for device communication and internet access.
Bluetooth: The module further extends its connectivity options by supporting Bluetooth protocols, enabling communication with other Bluetooth-enabled devices.
Fusion positioning: By combining the data from LoRaWAN, GNSS, Wi-Fi, and Bluetooth, the Wio-WM1110 can achieve highly accurate and reliable positioning, even in challenging environments.
Low-power operation: The Wio-WM1110 is designed for low-power consumption, allowing your devices to operate for extended periods on battery power.
Open-source platform: The Wio-WM1110 is based on an open-source platform, providing developers with access to the underlying hardware and software, allowing for greater customization and flexibility.

![alt text](https://hackster.imgix.net/uploads/attachments/1661286/lr1110_bd_cXS0jXzi4x.JPG?auto=compress%2Cformat&w=740&h=555&fit=max)

LR1110 Features
Low-Power, High-Sensitivity LoRa®/(G)FSK Half-Duplex RF Transceiver

Supports worldwide ISM frequency bands in the range of 150 MHz to 960 MHz.
Features a low-noise figure RX front-end for enhanced LoRa®/(G)FSK sensitivity.
Offers two high-power PA paths: +22 dBm and +15 dBm, with a high-efficiency PA path at +15 dBm.
Provides a long-range FHSS (LR-FHSS) modulator.
Includes an integrated PA regulator supply selector for simplified dual power (+15 dBm/+22 dBm) implementation with one board design.
Supports worldwide multi-region BoMs, with the circuit adapting to matching networks to satisfy regulatory limits.
Fully compatible with SX1261/2/8 devices and the LoRaWAN® standard, defined by the LoRa Alliance®.
Multi-Purpose Radio Front-End for Geolocation Applications

GNSS (GPS/BeiDou) low-power scanning
802.11b/g/n Wi-Fi ultra-low-power passive scanning
150 - 2700 MHz continuous frequency coverage
High-bandwidth RX ADC (up to 24 MHz DSB)
Digital baseband processing
Cryptographic Engine: Securing Your LoRaWAN Applications

The Wio-WM1110 integrates a powerful cryptographic engine to safeguard your LoRaWAN applications. Here's a breakdown of its key features:

Hardware-Accelerated Encryption/Decryption:

Provides efficient AES-128 encryption and decryption, crucial for securing data communication in LoRaWAN networks.
Dedicated hardware offloads the processing burden from the main CPU, enhancing performance and reducing power consumption.
Device Parameter Management:

Securely stores and manages device parameters like DevEUI and JoinEUI, defined by the LoRa Alliance.
These unique identifiers are essential for device authentication and network access, and the cryptographic engine ensures their integrity and confidentiality.
Enhanced Security:

Protects sensitive information like encryption keys from unauthorized access, preventing potential breaches and data leaks.
Offers a secure environment for storing critical data like NwkKey and AppKey, as defined in the LoRaWAN standard.
Overall, the cryptographic engine plays a crucial role in safeguarding the security and reliability of your LoRaWAN applications. It provides comprehensive protection for sensitive data and facilitates secure communication within the network.

![alt text](https://hackster.imgix.net/uploads/attachments/1661288/nrf52840_bd_IvmwAqJuDa.JPG?auto=compress%2Cformat&w=740&h=555&fit=max)

The NRF52840 is a powerful and versatile Bluetooth Low Energy (BLE) SoC from Nordic Semiconductor, offering a wide range of features for various IoT applications. Here's a breakdown of its key highlights:

CPU and Memory:

64 MHz Arm Cortex-M4F CPU with FPU: Delivers ample processing power for running complex applications.
1 MB Flash memory: Stores application code and data.
256 KB RAM: Provides sufficient memory for application execution and data handling.
Wireless Connectivity:

Bluetooth 5.3: Supports the latest Bluetooth standard for long-range, high throughput, and improved security.
2 Mbps PHY: Enables faster data transfer compared to previous Bluetooth versions.
Long Range: Achieves extended communication range for IoT applications.
802.15.4: Supports additional protocols like Thread and Zigbee for wider ecosystem compatibility.
Peripherals and Interfaces:

Multiple GPIOs: Enables connection to various sensors, actuators, and peripherals.
High-speed SPI and QSPI: Offers fast data transfer for external memory and displays.
PDM and I2S: Supports digital microphones and audio applications.
Full-speed USB device: Enables data transfer and battery charging.
ADC and DAC: Allows analog signal acquisition and generation.
Power Management:

Ultra-low power consumption: Enables long battery life for IoT devices.
Multiple power saving modes: Dynamically adjusts power consumption based on application requirements.
Security:

Hardware Cryptographic Engine: Provides secure data encryption and decryption.
Secure Boot: Ensures only authorized code can be executed on the device.
Other Features:

Real-time clock (RTC): Enables accurate timekeeping.
Temperature sensor: Provides temperature readings for environmental monitoring.
On-chip debugger: Simplifies development and debugging process.
Open-source platform:

Access to extensive resources and libraries for easier development and customization.
Overall, the NRF52840 is a powerful and feature-rich SoC that empowers developers to build innovative and efficient IoT solutions with low power consumption and robust capabilities.

![alt text](https://hackster.imgix.net/uploads/attachments/1661330/connection_diagram_y1mXRn1NXC.jpg?auto=compress%2Cformat&w=740&h=555&fit=max)

CONNECTION:

3V3 (Wio-WM1110 Dev Board) -> VTG (J-Link Debug Programmer nrf52dk)CLK (Wio-WM1110 Dev Board) -> SWCLK (J-Link Debug Programmer nrf52dk)DIO (Wio-WM1110 Dev Board) -> SWDIO (J-Link Debug Programmer nrf52dk)GND (Wio-WM1110 Dev Board) -> GND (J-Link Debug Programmer nrf52dk)

Programming Software:

A variety of programming software options exist for developing firmware on the WM1110. I have tested the module using Arduino IDE, PlatformIO, Keil uVision, Visual Studio Code, SEGGER Embedded Studio (SES), and Mbed Studio. From my experience, Mbed Studio and SEGGER Embedded Studio (SES) offer the most user-friendly experience for firmware development. This Getting Started guide will utilize SEGGER Embedded Studio (SES) for developing the firmware.

SEGGER Embedded Studio (SES) is a comprehensive and user-friendly IDE for managing, building, testing, and deploying embedded applications. This translates to smooth and efficient development operations thanks to its extensive feature set.

Powerful Project Management: Effortlessly manage your Wio-WM1110 firmware projects, regardless of size or complexity, with SES's robust project management tools.
Seamless Version Control: Leverage built-in version control features to track changes and deploy applications automatically.
Integrated Build and Debugging Tools: Utilize SES's powerful integrated build and debugging tools to streamline your Wio-WM1110 firmware development workflow.
Installing SEGGER Embedded Studio :

The software can be downloaded from this link: It's recommended to use the 5.68 version.https://www.segger.com/downloads/embedded-studio/

Download the nRF5 SDK and place it in the same directory where SEGGER Embedded Studio is installed.

The nRF5 SDK provides a comprehensive development environment for nRF5 Series devices. It includes a broad selection of drivers, libraries, examples for peripherals, SoftDevices, and proprietary radio protocols. All code examples within the SDK are specifically designed to compile and run on the Wio-WM1110 Dev Kit, streamlining your development process.

The software can be downloaded from this link: nRF5 SDK-Download

Download the Seeed Example Package and place it in the same directory where the nRF5 SDK is installed.

The Seeed Example Package can be downloaded from this link:Seeed Example-Download

Seeed Studio provides an example project to jumpstart developers' progress. This project encompasses LoRaWAN communication, positioning information acquisition, onboard sensor data acquisition, and more.

Add Seeed Example file to nRF5 SDK

Copy the Seeed Example file to the following path of nRF5 SDK: .../nRF5_SDK_17.1.0_ddde560/examples/peripheral/

![alt text](https://hackster.imgix.net/uploads/attachments/1651031/nextpcb_4r1pEG3pxS.JPG?auto=compress%2Cformat&w=740&h=555&fit=max)

This project was successfully completed because of the help and support from [NextPCB](https://www.nextpcb.com/pcb-assembly-quote). Guys if you have a PCB project, please visit their website and get exciting discounts and coupons.

NextPCB offers high-quality, reliable PCB starting at $1.9, and multilayer starting at $6.9. Also, everyone can enjoy free [PCB assembly](https://www.nextpcb.com/pcb-assembly-quote) for 5 boards! Also, NextPCB is having a year end sale in which anyone can register through their website and get a $30 Coupon which can be used for ordering PCBs.

You can also try HQDFM free online [PCB Gerber viewer](https://www.nextpcb.com/free-online-gerber-viewer.html) to check your PCB design and avoid costly errors.
