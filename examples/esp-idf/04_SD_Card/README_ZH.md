# 04_SD_Card

[English](README.md) | [简体中文](README_ZH.md)

## 功能

挂载 microSD 卡并输出卡片信息与容量。

## 硬件需求

ESP32-S3-Touch-AMOLED-1.43 开发板和可传输数据的 USB 线。 启动前在板载卡槽插入 microSD 卡。

## 怎么运行

在本目录打开 ESP-IDF 终端，使用仓库首页所列版本运行：

```bash
idf.py set-target esp32s3 build flash monitor
```

## 预期现象

挂载成功后，日志输出卡片信息与容量。

## 常见问题

挂载配置启用了失败后格式化，使用前请备份卡内文件。
