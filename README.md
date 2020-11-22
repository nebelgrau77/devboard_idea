### devboard idea

A pretty nice devboard would be this:

* STM32L4 MCU (CortexM4, low power, 80MHz)
* Arduino Nano form factor (Adafruit ItsyBitsy is probably too small to fit the sensors), breadboard friendly
* IMU for accelerometer/gyroscope based TinyML 
* PDM microphone for keyword spotting
* NeoPixel for user communication, e.g. green light for "yes", red for "no", etc.
* simple LED for blinking
* serial over USB
* DFU bootloader
* main interfaces printed by their pins like on ItsyBitsy
* needs SWD pins broken out

Such board:
* is fast enough for both motion and sound-based TinyML applications, 
* can be programmed with:
  * with STM32 HAL, 
  * Arduino core (STMDuino)
  * Rust
  * possibly MicroPython/CircuitPython
* has low power modes, e.g. LPUART

![SMT32L4 small packages](data/small_package_STM32L4.png)


BOM:
* 1 x MCU
* 1 x Xtal (8 MHz? 32kHz? check Nucleo32 L4)
* 1 x NeoPixel APA102 (SPI)
* 1 x LED (power/uploading/general LED)
* 2 x button switch
* 1 x USB Type-C (or B, which is has a smaller connector?)
* 1 x PDM microphone (STM MP34DT06J)
* 1 x IMU sensor (LIS3DH/LSM6DS3/LSM9DS1)
* 1 x Flash memory (2MB QSPI)

