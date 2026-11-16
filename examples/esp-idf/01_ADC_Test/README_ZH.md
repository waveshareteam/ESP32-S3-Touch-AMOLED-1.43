# 01_ADC_Test

[English](README.md) | [简体中文](README_ZH.md)

## 功能

通过 ADC 采集板载电池电压分压信号，输出原始采样值和换算电压。

## 硬件需求

ESP32-S3-Touch-AMOLED-1.43 开发板和可传输数据的 USB 线。 测量电池电压时需连接与开发板匹配的电池。

## 怎么运行

在本目录打开 ESP-IDF 终端，使用仓库首页所列版本运行：

```bash
idf.py set-target esp32s3 build flash monitor
```

## 预期现象

日志持续输出 ADC 采样值和电压。

## 常见问题

电压换算包含板载分压比例；未接电池时的读数不能作为电池电压。
