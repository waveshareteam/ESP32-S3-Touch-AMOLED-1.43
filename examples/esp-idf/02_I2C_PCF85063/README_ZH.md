# 02_I2C_PCF85063

[English](README.md) | [简体中文](README_ZH.md)

## 功能

通过 I2C 设置并读取板载 PCF85063 实时时钟。

## 硬件需求

ESP32-S3-Touch-AMOLED-1.43 开发板和可传输数据的 USB 线。

## 怎么运行

在本目录打开 ESP-IDF 终端，使用仓库首页所列版本运行：

```bash
idf.py set-target esp32s3 build flash monitor
```

## 预期现象

日志持续输出 RTC 日期和时间。

## 常见问题

示例每次启动都会写入固定初始时间；用作时钟前需修改 RTC 示例中的初始值。
