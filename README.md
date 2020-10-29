# STM32CubeH7 MCU Firmware Package

Branch: H7_V1.8
Fork: pavel_a
------------------
This is support branch of monolitic STM32H7 Cube package rebased from ST v. 1.8.0

Examples for various boards and things not relevant for us have been removed for size reduction.
All that is available in the official repo.
Our patches are in _patches dir (some already applied)

## Components:

* STM32H7 HAL     = 1.9.0
  - Patched: Drivers/STM32H7xx_HAL_Driver/Src/stm32h7xx_hal_eth.c
     Our patch from 1.5 (H.T.) - UNTESTED!
* STM32H7xx CMSIS = v1.9.0
* Cortex M7 CMSIS = 5.4.0
* LwIP            = 2.1.2
  - Patched: Removed macro LWIP_PLATFORM_ASSERT(x) via printf()
     in Middlewares/Third_Party/LwIP/system/arch/cc.h
* FreeRTOS        = 10.2.1
