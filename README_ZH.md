<div align="center">
  <h1>ESP32-S3-Touch-AMOLED-1.43</h1>
  <p><strong>ESP32-S3 1.43 英寸 466 × 466 QSPI AMOLED 触摸开发板</strong></p>
  <p><a href="README.md">English</a> | <strong>简体中文</strong></p>
  <p>
    <a href="https://github.com/waveshareteam/ESP32-S3-Touch-AMOLED-1.43/actions/workflows/build.yml"><img alt="构建" src="https://github.com/waveshareteam/ESP32-S3-Touch-AMOLED-1.43/actions/workflows/build.yml/badge.svg"></a>
    <a href="https://github.com/waveshareteam/ESP32-S3-Touch-AMOLED-1.43/releases/latest"><img alt="最新版本" src="https://img.shields.io/github/v/release/waveshareteam/ESP32-S3-Touch-AMOLED-1.43"></a>
    <a href="LICENSE"><img alt="许可证" src="https://img.shields.io/github/license/waveshareteam/ESP32-S3-Touch-AMOLED-1.43"></a>
  </p>
  <p>
    <a href="https://www.waveshare.com/esp32-s3-touch-amoled-1.43.htm">🌐 产品</a> &middot;
    <a href="https://github.com/waveshareteam/ESP32-S3-Touch-AMOLED-1.43/releases/latest">📦 固件</a> &middot;
    <a href="examples/esp-idf/">🧩 ESP-IDF</a> &middot;
    <a href="examples/arduino/examples/">🔧 Arduino</a> &middot;
    <a href="hardware/">📚 文档</a>
  </p>
  <p><img src="docs/images/esp32-s3-amoled-1.43.jpg" alt="ESP32-S3-Touch-AMOLED-1.43 开发板" width="500"></p>
</div>

---

## ✨ 概述

ESP32-S3-Touch-AMOLED-1.43 集成圆形 AMOLED 触摸屏、RTC、IMU 和 microSD 卡槽，支持 Wi-Fi 与低功耗蓝牙。本仓库提供 ESP-IDF、Arduino 示例、出厂演示及硬件资料。

| 功能 | 器件或接口 |
| --- | --- |
| MCU | ESP32-S3R8 |
| 存储器 | 16 MB Flash，8 MB PSRAM |
| 显示 | 1.43 英寸 AMOLED，466 × 466，QSPI |
| 触摸 | 电容触摸，I2C |
| RTC / IMU | PCF85063 / QMI8658 |

## 📦 快速开始

发布后可使用[最新版本](https://github.com/waveshareteam/ESP32-S3-Touch-AMOLED-1.43/releases/latest)中的可烧录示例固件。首次发布前可在 [Build 工作流](https://github.com/waveshareteam/ESP32-S3-Touch-AMOLED-1.43/actions/workflows/build.yml) 的成功运行中下载构建产物，或按各示例说明从源码运行。

1. 下载所需示例和框架版本对应的 `*-combined.zip`。
2. 解压后通过 `python -m pip install esptool` 安装 esptool。
3. 通过 USB 连接开发板。
4. Windows 运行 `flash_combined.bat COMx`，Linux 运行 `./flash_combined.sh /dev/ttyACM0`。
5. 如果开发板未自动重启，请手动复位。

出厂固件（恢复开箱演示）：在 [`firmware`](firmware/) 目录下载文件名带 `FactoryOnly` 的文件。

## 🧪 示例

### ESP-IDF

| 示例 | 主要功能 |
| --- | --- |
| [01_ADC_Test](examples/esp-idf/01_ADC_Test/README_ZH.md) | 通过 ADC 采集板载电池电压分压信号，输出原始采样值和换算电压。 |
| [02_I2C_PCF85063](examples/esp-idf/02_I2C_PCF85063/README_ZH.md) | 通过 I2C 设置并读取板载 PCF85063 实时时钟。 |
| [03_I2C_QMI8658](examples/esp-idf/03_I2C_QMI8658/README_ZH.md) | 通过 I2C 读取板载 QMI8658 IMU 的加速度和角速度。 |
| [04_SD_Card](examples/esp-idf/04_SD_Card/README_ZH.md) | 挂载 microSD 卡并输出卡片信息与容量。 |
| [05_WIFI_AP](examples/esp-idf/05_WIFI_AP/README_ZH.md) | 创建 2.4 GHz Wi-Fi 热点。 |
| [06_WIFI_STA](examples/esp-idf/06_WIFI_STA/README_ZH.md) | 以 STA 模式连接 2.4 GHz Wi-Fi 热点。 |
| [07_LVGL_Test](examples/esp-idf/07_LVGL_Test/README_ZH.md) | 在板载 AMOLED 屏运行 LVGL 控件演示，并读取电容触摸输入。 |
| [08_LVGL_SDIMG](examples/esp-idf/08_LVGL_SDIMG/README_ZH.md) | 列出 microSD 卡中的图片，并通过 LVGL 显示选中的图片。 |

### Arduino

| 示例 | 主要功能 |
| --- | --- |
| [01_ADC_Test](examples/arduino/examples/01_ADC_Test/README_ZH.md) | 通过 ADC 采集板载电池电压分压信号，输出原始采样值和换算电压。 |
| [02_I2C_PCF85063](examples/arduino/examples/02_I2C_PCF85063/README_ZH.md) | 通过 I2C 设置并读取板载 PCF85063 实时时钟。 |
| [03_I2C_QMI8658](examples/arduino/examples/03_I2C_QMI8658/README_ZH.md) | 通过 I2C 读取板载 QMI8658 IMU 的加速度和角速度。 |
| [04_SD_Card](examples/arduino/examples/04_SD_Card/README_ZH.md) | 挂载 microSD 卡并输出卡片信息与容量。 |
| [05_WIFI_AP](examples/arduino/examples/05_WIFI_AP/README_ZH.md) | 创建 2.4 GHz Wi-Fi 热点。 |
| [06_WIFI_STA](examples/arduino/examples/06_WIFI_STA/README_ZH.md) | 以 STA 模式连接 2.4 GHz Wi-Fi 热点。 |
| [07_LVGL_Test](examples/arduino/examples/07_LVGL_Test/README_ZH.md) | 在板载 AMOLED 屏运行 LVGL 控件演示，并读取电容触摸输入。 |

草图使用的库随仓库提供，位于 [`examples/arduino/libraries`](examples/arduino/libraries/)。

## 🛠️ 开发环境

| 开发框架 | 版本 | 示例数 |
| --- | --- | ---: |
| ESP-IDF | `v5.5.6`, `v6.1.1` | 8 |
| Arduino-ESP32 | `3.3.12` | 7 |

出厂工程使用 ESP-IDF `v5.1.4`，源码见 [`examples/factory`](examples/factory/README_ZH.md)。

## 📚 资料

- [原理图](hardware/schematic/)
- [机械资料（尺寸图和 3D 模型）](hardware/mechanical/)
- [产品页](https://www.waveshare.com/esp32-s3-touch-amoled-1.43.htm)
- [Wiki](https://docs.waveshare.net/ESP32-S3-Touch-AMOLED-1.43/)

## 🤝 支持

- 产品使用、硬件或订单问题：[微雪技术支持](https://docs.waveshare.net/ESP32-S3-Touch-AMOLED-1.43/Technical-Support/)。

## 📄 许可证

Apache License 2.0，详见 [LICENSE](LICENSE)。
