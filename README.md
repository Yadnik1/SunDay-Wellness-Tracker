# SunDay-Wellness-Tracker

SunDay Wellness Tracker is a comprehensive health monitoring device based on the Atmega328P MCU. It measures UV exposure, differentiates between artificial and natural light exposure for the user, and assesses air quality. The real-time data captured by our advanced sensors is transmitted to a user-friendly Flutter-based mobile application via Bluetooth for drawing inferences from the data. This app not only displays the data but also stores it in the Firebase Cloud Realtime Database for long-term analysis and health tracking.

## Development Procedure

### Firmware Development and System Integration:
- Utilized the ATmega328P microcontroller, interfacing it with HC05 Bluetooth Sensor over UART and GUVA S12-SD sensor over ADC.
- Wrote custom drivers for I2C communication with the ENS160 MOX Gas sensor and the AS7262 Light Sensor.
- Integrated a TFT LCD via SPI to display environmental data in real-time.
- Implemented a buzzer in the device to indicate the user when the AQI went over 3, based on timer interrupts.
- Devised a firmware for synchronizing tasks of the device and smooth wireless operation with the mobile device over Bluetooth.
- Assembled all components on a perfboard, ensuring effective system functionality.

### Mobile Application and Cloud Integration:
- Developed a mobile application using Flutter for intuitive data visualization and interaction.
- Leveraged Firebase for robust cloud-based data management and security.
- Crafted a visually appealing interface to represent sensor data and health insights effectively.
- Focused on enhancing user experience by providing intuitive navigation and actionable insights.



