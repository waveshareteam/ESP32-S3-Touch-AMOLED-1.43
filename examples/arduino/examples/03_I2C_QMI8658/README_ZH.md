# 03_I2C_QMI8658

[English](README.md) | [简体中文](README_ZH.md)

## 功能

通过 I2C 读取板载 QMI8658 IMU 的加速度和角速度。

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

移动开发板时，日志中的加速度和陀螺仪读数随之变化。

## 常见问题

暂无。
