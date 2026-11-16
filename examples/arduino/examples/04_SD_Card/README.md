# 04_SD_Card

[English](README.md) | [简体中文](README_ZH.md)

## What It Does

Mounts a microSD card and reports card information and capacity.

## Hardware Required

ESP32-S3-Touch-AMOLED-1.43 development board and a USB data cable. Insert a microSD card into the onboard slot before starting.

## How to Run

Install the Arduino-ESP32 version listed in the repository README, set the sketchbook to `examples/arduino/`, then open and upload the matching `.ino`. Select **ESP32S3 Dev Module** and use **115200** in the serial monitor.

| Tools menu | Value |
| --- | --- |
| Flash Size | 16MB (128Mb) |
| Partition Scheme | 16M Flash (3MB APP/9.9MB FATFS) |
| PSRAM | OPI PSRAM |
| USB CDC On Boot | Enabled |

## Expected Result

The log shows card information and capacity after a successful mount.

## Troubleshooting

The mount configuration enables formatting on mount failure; use a card whose contents are backed up.
