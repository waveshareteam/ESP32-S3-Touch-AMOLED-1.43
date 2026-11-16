# 03_I2C_QMI8658

[English](README.md) | [简体中文](README_ZH.md)

## What It Does

Reads acceleration and angular velocity from the onboard QMI8658 IMU over I2C.

## Hardware Required

ESP32-S3-Touch-AMOLED-1.43 development board and a USB data cable.

## How to Run

Open an ESP-IDF terminal in this directory and run with a version listed in the repository README:

```bash
idf.py set-target esp32s3 build flash monitor
```

## Expected Result

Acceleration and gyroscope readings change as the board is moved.

## Troubleshooting

None yet.
