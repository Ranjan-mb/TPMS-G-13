# Tire Pressure Monitoring System (TPMS)

## Overview
This project aims to design and develop a cost-effective Tire Pressure Monitoring System (TPMS) that monitors and reports tire pressure and temperature in real-time. The system uses an ESP32 microcontroller to collect data from sensors and send it via Wi-Fi to an Android application for display and alerts.

---

## Features
- Real-time tire pressure and temperature monitoring
- Wireless data transmission using ESP32's Wi-Fi capabilities
- Android app integration for user-friendly data visualization
- Alerts for abnormal tire pressure or temperature
- Low-cost and scalable design suitable for multiple tire setups

---

## Hardware Components
- **ESP32**: Microcontroller for sensor data processing and Wi-Fi communication
- **Pressure and Temperature Sensor**: Measures tire pressure and temperature
- **Battery**: Powers the hardware unit
- **Voltage Regulator (if needed)**: Ensures proper voltage levels for sensors and ESP32
- **PCB/Prototyping Board**: Assembles all components
- **Miscellaneous**: Wires, connectors, resistors, capacitors, etc.

---

## Software Requirements
- **Arduino IDE**: For ESP32 programming
- **Android Studio**: For developing the companion Android application
- **Firebase or Custom Backend (optional)**: To store and retrieve historical data
- **Libraries**:
  - `WiFi.h`: ESP32 Wi-Fi library
  - Sensor-specific libraries (e.g., `Adafruit_BMP280`, `Adafruit_BME280`)

---

## Installation and Setup

### Hardware Setup
1. Assemble the hardware components:
   - Connect the pressure and temperature sensor to the ESP32. (Pin connections depend on the specific sensor model; refer to its datasheet.)
   - Connect a battery or power supply to the ESP32.
   - Secure all components onto a PCB or breadboard.
2. Ensure proper wiring and insulation for safe operation.
3. Double-check the connections to avoid short circuits.

### Software Setup
1. Clone this repository:
   ```bash
   git clone https://github.com/your-username/tpms.git
Install the required libraries in Arduino IDE.
Flash the ESP32 with the firmware from the ESP32_Firmware folder.
Set up the Android app:
Open the TPMS_App folder in Android Studio.
Modify the config.xml file to add your ESP32's Wi-Fi credentials (SSID and password).
Build and run the app on your Android device.
Usage
Power on the TPMS hardware.
Open the Android app and connect to the hardware via Wi-Fi.
View real-time data on the app dashboard.
Respond to alerts for abnormal conditions.
Project Architecture
Block Diagram

Data Flow
Sensor data is collected by the ESP32.
Data is transmitted via Wi-Fi to the Android app.
The Android app processes and displays the data on a user-friendly dashboard.
Future Enhancements
Expand to support multiple tires simultaneously
Integrate machine learning for predictive maintenance
Implement cloud storage for historical data tracking
Add BLE connectivity as an alternative to Wi-Fi
Contributing
Contributions are welcome! Please fork the repository, create a new branch, and submit a pull request with your changes.

License
This project is licensed under the MIT License.

Acknowledgments
Open-source libraries and tools
Community tutorials and forums for guidance

### Next Steps
- Replace placeholder text (e.g., `Ranjan mb`, `mbranjan92@gmail.com`) with your details.
- Add actual images/screenshots for the block diagram, hardware setup, and Android app.
- Upload supporting code and documents to the repository.

Let me know if you need assistance customizing any section!
