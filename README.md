<h1 align="center">
  <br>
  <a href="https://vejas.zip">
<p align="center">
  <img src="https://cdn.hackclub.com/019e6e25-928e-72ba-8381-df4277977a68/SCR-20260528-lhif.png" width="400">
</p>  </a>
  <br>
  <sub>VejasBadge</sub>
  <br>
</h1>

<div align="center">
  <a href="https://kicad.org"><img src="https://img.shields.io/badge/KiCad-%23314CB0.svg?style=for-the-badge&logo=kicad&logoColor=white" alt="KiCad"></a>
  <a href="https://www.raspberrypi.com/products/rp2040/"><img src="https://img.shields.io/badge/RP2040-%23E30B5C.svg?style=for-the-badge&logo=raspberrypi&logoColor=white" alt="RP2040"></a>
  <a href="https://hackclub.com"><img src="https://img.shields.io/badge/Hack_Club-%23EC3750?style=for-the-badge&logo=hackclub&logoColor=white"></a>
</div>

<h4 align="center">An E-ink badge powered by the RP2040 MCU.</h4>

<br>

## Overview

VejasBadge is a compact wearable badge built around the Raspberry Pi **RP2040** microcontroller. It features an **E-ink display**, **NFC** via the ST25DV04K, and is powered over **USB-C** with battery charging support. 

It will be used to display info like my name, website and a photo of some sort. If the NFC coil works, I will add functionality, to choose the info transmitted by the NFC tag so you could share multiple website links. I would also like to use it as an ebook reader, but there may not be enough storage for that.

## Features

| Feature | Details |
|---------|---------|
| MCU | RP2040 @ 133MHz, LQFN-56 |
| Display | E-ink panel via 24-pin FPC connector (4-wire SPI) |
| NFC | ST25DV04K (ISO 15693 / I²C, 4Kbit) |
| Flash | ZD25WQ32CEIGR 32Mbit SPI Flash |
| RTC / Clock | ABM8-272-T3 crystal oscillator |
| Power | USB-C input, NCP1117ST33T3G 3.3V LDO|
| USB Protection | USBLC6-2SC6 ESD clamp |
| Buttons | 5× tactile switches (SKRKAEE020) |
| LEDs | 2× white status LEDs (0402) |

## Software

Firmware will be written in C++ using PlatformIO.

## Images
<p align="center">
  <img src="https://cdn.hackclub.com/019e6e24-8685-7638-927f-3452a827c5ef/SCR-20260528-lhbq.png" width="100%">
</p>

## Bill of Materials

### LCSC Components

| Part | Mfr. | Qty | Unit Price | Ext. Price | LCSC# |
|------|------|-----|------------|------------|-------|
| RP2040 | Raspberry Pi | 5 | $0.95 | $4.74 | [C2040](https://www.lcsc.com/product-detail/C2040.html) |
| ZD25WQ32CEIGR (32Mbit Flash) | Zetta | 5 | $0.57 | $2.86 | [C5258281](https://www.lcsc.com/product-detail/C5258281.html) |
| ST25DV04K-JFR6D3 (NFC) | ST | 5 | $0.86 | $4.30 | [C2654815](https://www.lcsc.com/product-detail/C2654815.html) |
| ABM8-272-T3 (Crystal) | ABRACON | 5 | $0.29 | $1.47 | [C20625731](https://www.lcsc.com/product-detail/C20625731.html) |
| NCP1117ST33T3G (LDO 3.3V) | onsemi | 5 | $0.24 | $1.18 | [C26537](https://www.lcsc.com/product-detail/C26537.html) |
| FPC-05F-24PH20 (24P FPC Connector) | XUNPU | 5 | $0.10 | $0.48 | [C2856805](https://www.lcsc.com/product-detail/C2856805.html) |
| USBLC6-2SC6 (ESD Protection) | HXY MOSFET | 5 | $0.03 | $0.16 | [C5261088](https://www.lcsc.com/product-detail/C5261088.html) |
| SI1308EDL (N-MOSFET) | TECH PUBLIC | 5 | $0.08 | $0.42 | [C7603347](https://www.lcsc.com/product-detail/C7603347.html) |
| MBR0530 (Schottky Diode) | Shikues | 50 | $0.02 | $1.00 | [C475718](https://www.lcsc.com/product-detail/C475718.html) |
| LB2012T680M (68µH Inductor) | Taiyo Yuden | 10 | $0.05 | $0.47 | [C223256](https://www.lcsc.com/product-detail/C223256.html) |
| YLED0402W (White LED) | YONGYUTAI | 50 | $0.015 | $0.77 | [C28310435](https://www.lcsc.com/product-detail/C28310435.html) |
| SKRKAEE020 (Tactile Switch) | Alps Alpine | 35 | $0.13 | $4.67 | [C115357](https://www.lcsc.com/product-detail/C115357.html) |
| USB-C Receptacle 16P | SHOU HAN | 20 | $0.07 | $1.48 | [C2765186](https://www.lcsc.com/product-detail/C2765186.html) |
| Cap 100nF 0402 | YAGEO | 100 | $0.001 | $0.13 | [C60474](https://www.lcsc.com/product-detail/C60474.html) |
| Cap 15pF 0402 NP0 | YAGEO | 100 | $0.001 | $0.13 | [C106997](https://www.lcsc.com/product-detail/C106997.html) |
| Cap 33pF 0402 NP0 | YAGEO | 100 | $0.001 | $0.13 | [C107005](https://www.lcsc.com/product-detail/C107005.html) |
| Cap 1µF 10V 0402 | Samsung EM | 100 | $0.003 | $0.30 | [C14445](https://www.lcsc.com/product-detail/C14445.html) |
| Cap 4.7µF 10V 0402 | Samsung EM | 50 | $0.008 | $0.39 | [C368809](https://www.lcsc.com/product-detail/C368809.html) |
| Cap 10µF 10V 0402 | Samsung EM | 20 | $0.012 | $0.23 | [C315248](https://www.lcsc.com/product-detail/C315248.html) |
| Res 3Ω 0402 | YAGEO | 100 | $0.002 | $0.20 | [C227064](https://www.lcsc.com/product-detail/C227064.html) |
| Res 27Ω 0402 | YAGEO | 100 | $0.001 | $0.09 | [C138021](https://www.lcsc.com/product-detail/C138021.html) |
| Res 1kΩ 0402 | YAGEO | 100 | $0.001 | $0.09 | [C106235](https://www.lcsc.com/product-detail/C106235.html) |
| Res 5.1kΩ 0402 | YAGEO | 100 | $0.001 | $0.09 | [C105872](https://www.lcsc.com/product-detail/C105872.html) |
| Res 10kΩ 0402 | YAGEO | 100 | $0.001 | $0.09 | [C60490](https://www.lcsc.com/product-detail/C60490.html) |
