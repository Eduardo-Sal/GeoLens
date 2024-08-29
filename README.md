# Vehicle Fleet Manager

This project serves as a purpose-built fleet management system for large-scale logistics or transportation operations.

The repository includes the following components:

## Hardware

We utilize an ESP32 Development Board along with the SIM7600G module for GPS and 4G capabilities. A crucial component of this project is the ADXL345 accelerometer, which is used to preserve battery life.

## Software

On the software side of the tracker, we leverage the ADXL345 to greatly reduce current consumption by determining the state of the vehicle. By setting specific parameters, we can put the device into sleep mode, which can reduce power usage from 96mA to 7mA. Additionally, we configure the Wi-Fi to detect if it is within a known network to further preserve battery life. To map the object we utilize php post request with arduinohttp and send it to an open source dashboard called traccar that includes a much cleaner user interface with map API we send information such as latitude, longitude, accuracy, battery, speed, and direction.

## Future Outlook

- Potentially implement OpenHaystack to further reduce power consumption
- Create a website with map API integration
