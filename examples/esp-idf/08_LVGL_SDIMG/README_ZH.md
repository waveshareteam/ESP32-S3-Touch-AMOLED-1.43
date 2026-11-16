# 08_LVGL_SDIMG

[English](README.md) | [简体中文](README_ZH.md)

## 功能

列出 microSD 卡中的图片，并通过 LVGL 显示选中的图片。

## 硬件需求

ESP32-S3-Touch-AMOLED-1.43 开发板和可传输数据的 USB 线。 需要在根目录建立 `Test` 文件夹的 microSD 卡。

## 怎么运行

运行前将 `Test_IMG_SRC/` 内的图片复制到卡内 `Test/` 文件夹。

在本目录打开 ESP-IDF 终端，使用仓库首页所列版本运行：

```bash
idf.py set-target esp32s3 build flash monitor
```

## 预期现象

通过触摸界面扫描文件夹，选择图片后显示。

## 常见问题

文件列表最多显示 20 项，建议使用随附 BMP、JPG、PNG 示例图片；挂载失败可能格式化卡片。
