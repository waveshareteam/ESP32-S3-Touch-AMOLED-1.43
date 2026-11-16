# 01_ADC_Test

[English](README.md) | [简体中文](README_ZH.md)

## What It Does

Samples the onboard battery-voltage divider with ADC and prints raw readings and the calculated voltage.

## Hardware Required

ESP32-S3-Touch-AMOLED-1.43 development board and a USB data cable. An optional compatible battery is needed to measure battery voltage.

## How to Run

Install the Arduino-ESP32 version listed in the repository README, set the sketchbook to `examples/arduino/`, then open and upload the matching `.ino`. Select **ESP32S3 Dev Module** and use **115200** in the serial monitor.

| Tools menu | Value |
| --- | --- |
| Flash Size | 16MB (128Mb) |
| Partition Scheme | 16M Flash (3MB APP/9.9MB FATFS) |
| PSRAM | OPI PSRAM |
| USB CDC On Boot | Enabled |

## Expected Result

The log repeatedly shows ADC readings and voltage values.

## Troubleshooting

The voltage calculation includes the board's divider ratio; an unconnected battery input does not represent a battery measurement.
