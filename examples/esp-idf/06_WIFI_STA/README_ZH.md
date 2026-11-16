# 06_WIFI_STA

[English](README.md) | [简体中文](README_ZH.md)

## 功能

以 STA 模式连接 2.4 GHz Wi-Fi 热点。

## 硬件需求

ESP32-S3-Touch-AMOLED-1.43 开发板和可传输数据的 USB 线。 需要可用的 2.4 GHz Wi-Fi 热点。

## 怎么运行

编译前在示例的 Wi-Fi 源码中设置 SSID 和密码。

在本目录打开 ESP-IDF 终端，使用仓库首页所列版本运行：

```bash
idf.py set-target esp32s3 build flash monitor
```

## 预期现象

连接成功后，日志输出分配到的 IP 地址。

## 常见问题

默认 SSID 和密码为 `bsp_esp_demo` / `waveshare`，需要与实际热点一致。
