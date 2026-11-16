# 05_WIFI_AP

[English](README.md) | [简体中文](README_ZH.md)

## 功能

创建 2.4 GHz Wi-Fi 热点。

## 硬件需求

ESP32-S3-Touch-AMOLED-1.43 开发板和可传输数据的 USB 线。 需要带 Wi-Fi 的手机或电脑搜索热点。

## 怎么运行

安装仓库首页所列版本的 Arduino-ESP32，将草图目录设为 `examples/arduino/`，打开本目录同名 `.ino` 后上传。开发板选择 **ESP32S3 Dev Module**，串口监视器设为 **115200**。

| 工具菜单 | 设置 |
| --- | --- |
| Flash Size | 16MB (128Mb) |
| Partition Scheme | 16M Flash (3MB APP/9.9MB FATFS) |
| PSRAM | OPI PSRAM |
| USB CDC On Boot | Enabled |

## 预期现象

Wi-Fi 列表中出现热点，可连接客户端。

## 常见问题

默认热点为 `bsp_esp_demo`，密码为 `waveshare`；修改源码中的热点配置后重新上传。
