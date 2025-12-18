# Pinmap — MycoBrain V1

## SX1262 (Side-B + Gateway)

Authoritative schematic mapping:

- SX_Reset → **GPIO7**
- SX_Busy → **GPIO08**
- SX_CLK → **GPIO10**
- SX_CS → **GPIO09**
- SX_DI01 → **GPIO13**
- SX_DI02 → **GPIO14**
- SX_MISO → **GPIO11**
- SX_MOSI → **GPIO12**

## I2C

Board exposes **SCL** and **SDA** nets wired to ESP32 module pins.
Firmware defaults to SDA=GPIO4, SCL=GPIO5 but allows runtime override via `CMD_SET_I2C`.
