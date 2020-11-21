### devboard idea

A pretty nice devboard would be this:

* STM32L4 MCU (CortexM4, low power, 80MHz)
* Arduino Nano form factor (Adafruit ItsyBitsy is probably too small to fit the sensors), breadboard friendly
* IMU for accelerometer/gyroscope based TinyML 
* PDM microphone for keyword spotting
* NeoPixel for user communication, e.g. green light for "yes", red for "no", etc.
* simple LED for blinking
* serial over USB
* main interfaces printed by their pins like on ItsyBitsy

Such board:
* is fast enough for both motion and sound-based TinyML applications, 
* can be programmed with:
  * with STM32 HAL, 
  * Arduino core (STMDuino)
  * Rust
  * possibly MicroPython/Circuitpython


