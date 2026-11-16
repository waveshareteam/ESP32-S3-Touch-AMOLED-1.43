# 01_ADC_Test

[English](README.md) | [简体中文](README_ZH.md)

## 功能

通过 ADC 采集板载电池电压分压信号，输出原始采样值和换算电压。

## 硬件需求

ESP32-S3-Touch-AMOLED-1.43 开发板和可传输数据的 USB 线。 测量电池电压时需连接与开发板匹配的电池。

## 怎么运行

安装仓库首页所列版本的 Arduino-ESP32，将草图目录设为 `examples/arduino/`，打开本目录同名 `.ino` 后上传。开发板选择 **ESP32S3 Dev Module**，串口监视器设为 **115200**。

| 工具菜单 | 设置 |
| --- | --- |
| Flash Size | 16MB (128Mb) |
| Partition Scheme | 16M Flash (3MB APP/9.9MB FATFS) |
| PSRAM | OPI PSRAM |
| USB CDC On Boot | Enabled |

## 预期现象

日志持续输出 ADC 采样值和电压。

## 常见问题

电压换算包含板载分压比例；未接电池时的读数不能作为电池电压。
