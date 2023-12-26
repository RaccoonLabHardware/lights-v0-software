# RaccoonLab UAV LIGHTS v2 node

This is a repository for [RaccoonLab UAV Lights v2](https://docs.raccoonlab.co/guide/ui_leds/) node.

| View | Top view | Bot view |
| ---- | --- | ------ |
| <img src="https://docs.raccoonlab.co/assets/img/t-view.42a0bfba.png" alt="drawing" width="225"> | <img src="https://docs.raccoonlab.co/assets/img/t-view-top.39aeaa81.png" alt="drawing" width="225"> | <img src="https://docs.raccoonlab.co/assets/img/t-view-bottom.e9a28e7d.png" alt="drawing" width="225">|

The core of this repository is the .ioc file that defines the stm32 peripherals with respect to what a real device has.

The peripheral configuration is shown below:

| | |
|-|-|
| <img src="Assets/stm32cubemx.png" alt="drawing"> | <img src="Assets/adc1_settings.png" alt="drawing"> |

Additionally, the reposity has a source code generated with STM32CubeMX v6.6.0 using STM32Cube FW_G0 V1.6.1 for STM32CubeIDE usage.

Feel free to write your own custom firmware to test some features or suggest something.

The entry point is Core/Src/main.c. This file initializes all the peripherals and then goes to application_entry_point(). This is where a custom user logic is expected to be implemented.

Reference:
- Hardware: https://docs.raccoonlab.co/guide/ui_leds/hardware.html
- Docs: https://docs.raccoonlab.co/guide/ui_leds/
- Usage example: https://github.com/RaccoonlabDev/lights-node
