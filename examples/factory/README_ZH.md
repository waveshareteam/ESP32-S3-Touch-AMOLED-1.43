# factory

[English](README.md) | [简体中文](README_ZH.md)

## 功能

运行出厂测试界面，包含显示、触摸、RTC、IMU、电池 ADC、SD 卡、Wi-Fi/BLE 扫描及按键/GPIO 测试。

## 硬件需求

ESP32-S3-Touch-AMOLED-1.43 开发板和可传输数据的 USB 线。 电池和 microSD 卡用于对应测试；GPIO 测试需按 `components/gpio_bsp/` 的定义连接回环线路。

## 怎么运行

在本目录打开 ESP-IDF 终端，使用 **v5.1.4**运行：

```bash
idf.py set-target esp32s3 build flash monitor
```

## 预期现象

触摸界面显示外设读数和测试状态，扫描按钮可列出附近无线设备。

## 常见问题

未接回环线路时 GPIO 测试会显示失败；SD 挂载配置可能在失败后格式化卡片。
