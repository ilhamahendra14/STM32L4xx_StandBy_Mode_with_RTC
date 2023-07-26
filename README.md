# STM32L4xx_StandBy_Mode_with_RTC

**Impotant:**
+ To get accurate time, set the RTC clock to 32.768KHz.
+ Give a delay at least 3 seconds before entering stand-by mode to avoid looping stand-by mode and can't be debugged/uploaded new firmware.
+ If your STM32 is stuck in stand-by loop, please give jumper BOOT0 pin to 3v3, so you can debug/upload new firmware again.

StandBy mode can be an option if we want to build an embedded system with low power consumption.
Based on [STM32L432KC Datasheet](https://www.st.com/resource/en/datasheet/stm32l432kc.pdf) stand-by mode with RTC using 280 nA current consumption. I tested and got 291nA.
![alt text](https://github.com/ilhamahendra14/STM32L4xx_StandBy_Mode_with_RTC/blob/820ad77c1f564e8b648c1cf5a4da982f8fccebe8/current_consumption.png?raw=true)