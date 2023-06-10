# addon-u6143_ssd1306
Home Assistant Community Add-on: Pi Rack (U6143) OLED Display

This is a add-on wrapper for the UCTRONICS [U6143_ssd1306](https://github.com/darkgrue/U6143_ssd1306) Pi Rack OLED display driver.

## Prerequisites
The Home Assistant Operating System is a managed environment, which means `raspi-config` can’t be used to enable the I2C bus on a Raspberry Pi.
In order to use I2C devices you will have to follow the instructions on the [Common Tasks - Operating System](https://www.home-assistant.io/common-tasks/os/#enable-i2c) page to enable I2C for Home Assistant OS.
