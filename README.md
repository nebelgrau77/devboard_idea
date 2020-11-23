### Devboard idea - Overview

_This is just a draft of an idea. I don't know anything about PCB design, but I'm trying to gather the ideas, best practices from the boards I own, etc._

Main characteristics:
* fast enough for both motion and sound-based TinyML applications, 
* can be programmed with:
  * with STM32 HAL, 
  * Arduino core (STMDuino)
  * Rust
  * possibly MicroPython/CircuitPython
* has low power modes, e.g. LPUART
* microphone, IMU, RGB LED

[Detailed description](detailed_description.md)
[Bill Of Materials](BOM.md)
[Notes](notes.md)
[To do](todo.md)

