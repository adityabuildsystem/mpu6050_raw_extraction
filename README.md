# MPU6050 Raw Data Extraction

This repository establishes baseline communication with the MPU6050 6-axis inertial measurement unit (IMU) to read raw accelerometer, gyroscope, and temperature telemetry over I2C.

## Hardware Requirements

- Microcontroller (tested on ESP32-S3)
- MPU6050 breakout board
- Connecting wires

## Pin Configuration (I2C)

| MPU6050 Pin | Microcontroller Pin (Standard I2C) |
| :--- | :--- |
| VCC | 3.3V / 5V |
| GND | GND |
| SCL | SCL (GPIO configurable per board architecture) |
| SDA | SDA (GPIO configurable per board architecture) |

## Dependencies

Install the following libraries via the Arduino Library Manager:
- `Adafruit MPU6050`
- `Adafruit Unified Sensor`
- `Adafruit BusIO`

## Usage

1. Open `mpu6050_raw.ino` in the Arduino IDE.
2. Select the target board and port.
3. Open the Serial Monitor at a baud rate of `115200`.
