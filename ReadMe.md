### Freeskates

This project is a sensor and analysis kit for Freeskates.

## Getting started

For now, just run 'skate_analyzer copy 3.py'. It reads the 'skate_data.csv' file and creates a visualization. 
The biggest problem currently is drift in the sensors. 


## Hardware
- [Raspberry Pi Pico 2W](https://www.adafruit.com/product/6087)
- [Adafruit BNO085 9-DOF IMU Breakout](https://www.adafruit.com/product/4754)

## Pin Layout & Connections
```
RPI PICO 2 W          BNO085 BREAKOUT
+-----------+          +-------------+
|           |          |             |
|  3V3 (36) |--------->|  VIN        |  <-- Power (3.3V)
|           |          |             |
|  GND (38) |--------->|  GND        |  <-- Ground
|           |          |             |
|  GP4 (6)  |--------->|  SDA        |  <-- I2C Data
|           |          |             |
|  GP5 (7)  |--------->|  SCL        |  <-- I2C Clock
|           |          |             |
+-----------+          +-------------+
```