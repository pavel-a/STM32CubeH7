# STM32CubeH7 MCU Firmware Package

Branch: H7_V1.9
Fork: pavel_a
------------------
This is support branch of monolithic STM32H7 Cube package rebased from ST v. 1.9.0

Examples for various boards and things not relevant for us have been removed for size reduction.
All that is available in the official repo.
Our patches are in _patches dir (some already applied)

## Components:

* STM32H7 HAL     = 1.10.0
- Patched:
  - ETH: ... TODO
* STM32H7xx CMSIS = v1.10.0
* Cortex M7 CMSIS = 5.6.0
* LwIP            = 2.1.2
  - Patched: Removed macro LWIP_PLATFORM_ASSERT(x) via printf()
     in Middlewares/Third_Party/LwIP/system/arch/cc.h
* FreeRTOS        = 10.3.1 (MPU)

See release notes in the official ST repo for more info.
https://github.com/STMicroelectronics/STM32CubeH7
