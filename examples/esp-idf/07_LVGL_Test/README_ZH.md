# 07_LVGL_Test

[English](README.md) | [简体中文](README_ZH.md)

## 功能

在板载 AMOLED 屏运行 LVGL 控件演示，并读取电容触摸输入。

## 硬件需求

ESP32-S3-Touch-AMOLED-1.43 开发板和可传输数据的 USB 线。

## 怎么运行

在本目录打开 ESP-IDF 终端，使用仓库首页所列版本运行：

```bash
idf.py set-target esp32s3 build flash monitor
```

## 预期现象

屏幕显示 LVGL 控件，触摸可进行交互。

## 常见问题

本示例使用 LVGL 8 API，不可直接替换为 LVGL 9。
