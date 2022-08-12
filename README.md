# Firmware for LED Thermometer

The repository contains source code of firmware for LED Thermometer.  
IDE IAR is used for building and debugging purposes.  
To get information regarding hardware go to a repository [led_thermometer-hw](https://github.com/JavaLandau/led_thermometer-hw).

Structure of the firmware:

<pre>
- Project                   - project files of IDE IAR
- Src                       - source code of main files  
    - AlcoholColumn.c       - HL-driver of alcohol column (column of LEDs)  
    - main.c                - main file, including initialization and main logic of the device  
    - ...  
- Inc                       - headers of main files in Src  
- STM32CubeF0               - submodule of CMSIS and HAL drivers from STMicroelectronics  
- Devices                   - library of drivers for chips presented on the board of the device  
    - DS18B20               - driver for digital temperature sensor DS18B20  
    - MBI5039               - driver for SPI LED driver MBI5039  
- GPIOfun                   - service library to refer to GPIO as string  
- TIMDelay                  - library to make time delay based on hardware timer
</pre>