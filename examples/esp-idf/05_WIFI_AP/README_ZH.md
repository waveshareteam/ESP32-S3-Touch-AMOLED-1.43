# 05_WIFI_AP

[English](README.md) | [简体中文](README_ZH.md)

## 功能

创建 2.4 GHz Wi-Fi 热点。

## 硬件需求

ESP32-S3-Touch-AMOLED-1.43 开发板和可传输数据的 USB 线。 需要带 Wi-Fi 的手机或电脑搜索热点。

## 怎么运行

在本目录打开 ESP-IDF 终端，使用仓库首页所列版本运行：

```bash
idf.py set-target esp32s3 build flash monitor
```

## 预期现象

Wi-Fi 列表中出现热点，可连接客户端。

## 常见问题

默认热点为 `waveshare_esp32`，密码为 `wav123456`；修改源码中的热点配置后重新上传。
