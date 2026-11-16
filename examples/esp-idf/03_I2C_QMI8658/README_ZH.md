# 03_I2C_QMI8658

[English](README.md) | [简体中文](README_ZH.md)

## 功能

通过 I2C 读取板载 QMI8658 IMU 的加速度和角速度。

## 硬件需求

ESP32-S3-Touch-AMOLED-1.43 开发板和可传输数据的 USB 线。

## 怎么运行

在本目录打开 ESP-IDF 终端，使用仓库首页所列版本运行：

```bash
idf.py set-target esp32s3 build flash monitor
```

## 预期现象

移动开发板时，日志中的加速度和陀螺仪读数随之变化。

## 常见问题

暂无。
