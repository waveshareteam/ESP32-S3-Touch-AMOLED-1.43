# 02_I2C_PCF85063

[English](README.md) | [简体中文](README_ZH.md)

## What It Does

Sets and reads the onboard PCF85063 RTC over I2C.

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

The log repeatedly prints the RTC date and time.

## Troubleshooting

The demo writes a fixed initial date and time on every boot; change it in the RTC example before using it as a clock.
