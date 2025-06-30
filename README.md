# iotBoard
This project showcases the complete PCB design of a custom IoT-enabled sensor board specifically developed for Unmanned Aerial Vehicles (UAVs). The board integrates several critical sensors and measurement circuits into a compact form factor, making it ideal for use in drones that require reliable and real-time data acquisition during flight. Designed with modularity, lightweight construction, and flight efficiency in mind, the board serves as a plug-and-play solution for drone developers, researchers, and enthusiasts aiming to improve onboard diagnostics and flight performance.

The sensor board includes a current sensing circuit to monitor power consumption, a voltage sensing module for battery and power system tracking, a temperature sensor to detect overheating or monitor environmental conditions, and an interface for load cells to measure payload weight or dynamic load changes during flight. These sensors provide real-time insights into the UAV's operational status, making it easier to detect anomalies, prevent system failures, and manage power resources efficiently.

This PCB is well-suited for a variety of UAV applications, such as telemetry systems, autonomous navigation, payload delivery drones, and environmental sensing platforms. By providing accurate and continuous monitoring, it enhances the reliability and intelligence of UAV systems, particularly when paired with flight controllers or IoT platforms for data logging and analysis.

Included in this repository are the complete schematic and layout files, a bill of materials (BOM) listing all components with part numbers, and Gerber files ready for PCB fabrication. Additionally, a reference designator map and basic usage documentation are provided to assist in assembly, testing, and integration.

To get started, you can manufacture the PCB using the provided Gerber files through any standard PCB fabrication service. Components listed in the BOM can be sourced from major suppliers and assembled either manually or with an SMT assembly service. Once assembled, the board can be connected to your UAV’s microcontroller or flight controller, and optionally integrated with wireless modules or IoT platforms for advanced data transmission and storage.

Future versions of this board may include features such as wireless communication (LoRa, BLE, or Wi-Fi), onboard GPS and IMU support, and compatibility with edge AI systems for real-time, autonomous decision-making. This project serves as a foundational sensor platform that can be expanded to meet the needs of various UAV missions.

| Component/Module          | Description / Value                 | Footprint / Package                        | Quantity |
| ------------------------- | ----------------------------------- | ------------------------------------------ | -------- |
| ARDUINO\_MEGA\_2560\_REV3 | Main Microcontroller Board          | ARDUINO\_ARDUINO\_MEGA\_2560\_REV3         | 1        |
| LOADCELL SECTION          | Load Cell Interface                 | RJ45\_Amphenol\_54602-x08\_Horizontal      | 1        |
| WING TILT                 | Tilt Sensor Connector               | RJ45\_Amphenol\_54602-x08\_Horizontal      | 1        |
| MOTOR currents            | Motor Current Sensor Interface      | RJ45\_Amphenol\_54602-x08\_Horizontal      | 1        |
| MOTOR TEMP                | Motor Temperature Sensor Interface  | RJ45\_Amphenol\_54602-x08\_Horizontal      | 1        |
| MOTOR RPM                 | Motor RPM Sensor Interface          | RJ45\_Amphenol\_54602-x08\_Horizontal      | 1        |
| ECU                       | ESC Connector                       | RJ45\_Amphenol\_54602-x08\_Horizontal      | 1        |
| UART                      | Serial Communication Port           | PinSocket\_2x02\_P2.54mm\_Vertical         | 1        |
| SEN-13879                 | Current Sensor Module               | SPARKFUN\_SEN-13879                        | 1        |
| MOT\_C\_GND / SIG / VCC   | Motor Current Sensor Breakout Pins  | PinHeader\_1x04\_P2.54mm                   | 3        |
| R                         | Through-Hole Resistor               | Axial\_DIN0207\_L6.3mm\_D2.5mm\_P7.62mm    | 1        |
| 113991054                 | Grove Connector Module (Likely RTC) | MODULE\_113991054                          | 1        |
| XT60PW-M                  | Power Connector (XT60)              | AMASS\_XT60PW-M\_1x02\_P7.20mm\_Horizontal | 1        |
| iot\_board                | Custom Modules (Unspecified)        | rtcModule / Untitled (Custom footprints)   | 2        |
