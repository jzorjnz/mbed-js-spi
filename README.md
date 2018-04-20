# mbed-js-spi
JavaScript wrappers for SPI by STMircroelectronics.

# About library
Helper class SPI providing functions for SPI communication common for a series of SPI devices.

# Requirements
This library is to be used with the following tools:
* [Mbed](https://www.mbed.com/en/platform/mbed-os/)
* [JerryScript](https://github.com/jerryscript-project/jerryscript)

See this project for more information: [mbed-js-example](https://github.com/ARMmbed/mbed-js-example)

# Installation
* Before installing this library, make sure you have a working JavaScript on Mbed project.
Follow [mbed-js-example](https://github.com/ARMmbed/mbed-js-example) to create the project.
Make sure the project builds for your target device before proceeding.

* Install this library using npm (Node package manager) with the following command:
```
cd project_path
npm install syed-zeeshan/mbed-js-spi
```

# Usage
```
//Initialize SPI with mosi, miso, sclk pins
var spi = SPI(mosi_pin, miso_pin, sclk_pin);

//To use with another library, 
var hts221 = HTS221_JS();

// Example 1:
hts221.init_spi(spi, cs_pin);

// Example 2:
hts221.init_spi(spi, cs_pin, int1_pin, int2_pin, spi_type);

```

# Dependents
This library is requred if using SPI for connecting with the following devices:
* [mbed-js-hts221](https://www.github.com/syed-zeeshan/mbed-js-hts221)
* [mbed-js-lps22hb](https://www.github.com/syed-zeeshan/mbed-js-lps22hb)
* [mbed-js-lsm6dsl](https://www.github.com/syed-zeeshan/mbed-js-lsm6dsl)
* [mbed-js-lsm303agr](https://www.github.com/syed-zeeshan/mbed-js-lsm303agr)
