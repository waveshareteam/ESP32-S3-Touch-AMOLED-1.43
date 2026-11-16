# 01_ADC_Test

[English](README.md) | [简体中文](README_ZH.md)

## What It Does

Samples the onboard battery-voltage divider with ADC and prints raw readings and the calculated voltage.

## Hardware Required

ESP32-S3-Touch-AMOLED-1.43 development board and a USB data cable. An optional compatible battery is needed to measure battery voltage.

## How to Run

Open an ESP-IDF terminal in this directory and run with a version listed in the repository README:

```bash
idf.py set-target esp32s3 build flash monitor
```

## Expected Result

The log repeatedly shows ADC readings and voltage values.

## Troubleshooting

The voltage calculation includes the board's divider ratio; an unconnected battery input does not represent a battery measurement.
