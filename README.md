# Smart-Irrigation-System-Using-Raspberry-Pi
This project implements a Smart Irrigation System using a Raspberry Pi, temperature sensor, moisture sensor, and rain sensor. The system automates the irrigation process based on real-time environmental conditions and ensures efficient water usage.
How It Works
Sensors Read Data:

Temperature Sensor (TMP36): Measures ambient temperature.
Moisture Sensor (MCP3008): Detects soil moisture level.
Rain Sensor: Detects rainfall presence.
Data Processing:

The Raspberry Pi reads the sensor values using the SPI (Serial Peripheral Interface) bus.
It converts the analog data from sensors into digital form for further processing.
Decision Making:

If temperature > 25°C, moisture level < 100, and no rain detected, the motor starts.
Otherwise, the motor remains off.
Motor Control:

The motor (connected via a relay) is turned ON or OFF based on the sensor readings.
LCD Display:

Displays real-time temperature, moisture levels, and motor status.
SMS Notification:

Sends an SMS alert to the registered user via UART communication whenever the motor starts or stops.
Component	Function
Raspberry Pi	Controls the irrigation system and processes sensor data.
LCD Display (16x2) -	Shows real-time temperature, soil moisture, and system status.
Temperature Sensor (TMP36) -	Measures the ambient temperature.
Soil Moisture Sensor -	Detects the water content in the soil.
Rain Sensor -	Detects the presence of rainfall.
Relay Module -	Controls the water pump motor.
SPI-based ADC (MCP3008) -	Converts analog sensor signals to digital.
