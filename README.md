# LBM Nucleo-WL55JC port

This repository contains an initial port of the LBM v4.4.0 for the STM32 Nucleo-WL55JC development board.

The relevant board HAL and CMSIS libraries were obtained from the STM32CubeWL software package. Core file templates were relocated to the core folder within the template structure.
However, further work is required to connect these drivers with the Semtech modem library.

## LoRa Basic Modem library
LBM proposes an full implementation of the [TS001-LoRaWAN L2 1.0.4](https://resources.lora-alliance.org/technical-specifications/ts001-1-0-4-lorawan-l2-1-0-4-specification) and [Regional Parameters RP2-1.0.3](https://resources.lora-alliance.org/technical-specifications/rp2-1-0-3-lorawan-regional-parameters) specifications.

Please refer to [README.md](lbm_lib/README.md) to get all information related to LoRa Basics Modem library