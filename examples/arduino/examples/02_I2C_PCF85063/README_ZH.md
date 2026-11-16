# 02_I2C_PCF85063

[English](README.md) | [简体中文](README_ZH.md)

## 功能

通过 I2C 设置并读取板载 PCF85063 实时时钟。

## 硬件需求

ESP32-S3-Touch-AMOLED-1.43 开发板和可传输数据的 USB 线。

## 怎么运行

安装仓库首页所列版本的 Arduino-ESP32，将草图目录设为 `examples/arduino/`，打开本目录同名 `.ino` 后上传。开发板选择 **ESP32S3 Dev Module**，串口监视器设为 **115200**。

| 工具菜单 | 设置 |
| --- | --- |
| Flash Size | 16MB (128Mb) |
| Partition Scheme | 16M Flash (3MB APP/9.9MB FATFS) |
| PSRAM | OPI PSRAM |
| USB CDC On Boot | Enabled |

## 预期现象

日志持续输出 RTC 日期和时间。

## 常见问题

示例每次启动都会写入固定初始时间；用作时钟前需修改 RTC 示例中的初始值。
