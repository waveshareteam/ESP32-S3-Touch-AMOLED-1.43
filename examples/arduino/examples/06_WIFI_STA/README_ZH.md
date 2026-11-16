# 06_WIFI_STA

[English](README.md) | [简体中文](README_ZH.md)

## 功能

以 STA 模式连接 2.4 GHz Wi-Fi 热点。

## 硬件需求

ESP32-S3-Touch-AMOLED-1.43 开发板和可传输数据的 USB 线。 需要可用的 2.4 GHz Wi-Fi 热点。

## 怎么运行

编译前在示例的 Wi-Fi 源码中设置 SSID 和密码。

安装仓库首页所列版本的 Arduino-ESP32，将草图目录设为 `examples/arduino/`，打开本目录同名 `.ino` 后上传。开发板选择 **ESP32S3 Dev Module**，串口监视器设为 **115200**。

| 工具菜单 | 设置 |
| --- | --- |
| Flash Size | 16MB (128Mb) |
| Partition Scheme | 16M Flash (3MB APP/9.9MB FATFS) |
| PSRAM | OPI PSRAM |
| USB CDC On Boot | Enabled |

## 预期现象

连接成功后，日志输出分配到的 IP 地址。

## 常见问题

默认 SSID 和密码为 `bsp_esp_demo` / `waveshare`，需要与实际热点一致。
