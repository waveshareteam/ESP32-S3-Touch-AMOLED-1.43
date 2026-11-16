# 03_I2C_QMI8658

[English](README.md) | [简体中文](README_ZH.md)

## What It Does

Reads acceleration and angular velocity from the onboard QMI8658 IMU over I2C.

## Hardware Required

ESP32-S3-Touch-AMOLED-1.43 development board and a USB data cable.

## How to Run

Install the Arduino-ESP32 version listed in the repository README, set the sketchbook to `examples/arduino/`, then open and upload the matching `.ino`. Select **ESP32S3 Dev Module** and use **115200** in the serial monitor.

| Tools menu | Value |
| --- | --- |
| Flash Size | 16MB (128Mb) |
| Partition Scheme | 16M Flash (3MB APP/9.9MB FATFS) |
| PSRAM | OPI PSRAM |
| USB CDC On Boot | Enabled |

## Expected Result

Acceleration and gyroscope readings change as the board is moved.

## Troubleshooting

None yet.
