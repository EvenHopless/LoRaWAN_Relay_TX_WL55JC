# LoRaWAN Soil moisture sensor

This repository contains an example application utilizing the LBM modem v.4.4.0. The code is based on Semtech's periodic uplink example application.
The application is configured to collect a soil moisture sample every 30 minutes and transmit this data to the network server.

The LoRaWAN credentials must be provided in example_options.h

## LoRa Basic Modem library
LBM proposes an full implementation of the [TS001-LoRaWAN L2 1.0.4](https://resources.lora-alliance.org/technical-specifications/ts001-1-0-4-lorawan-l2-1-0-4-specification) and [Regional Parameters RP2-1.0.3](https://resources.lora-alliance.org/technical-specifications/rp2-1-0-3-lorawan-regional-parameters) specifications.

Please refer to [README.md](lbm_lib/README.md) to get all information related to LoRa Basics Modem library

## Resources

In addition to copying this library, you will need an analogue moisture sensor connected to a Nucleo-L476RG development board and a SX1261MB2BAS radio module.
To hook up the sensor to the develoopment board, please follow the connection diagram below.

![Connection Diagram](assets/connection_diag.png)

## Build

To build the example application the following should be executed on the command line:

```bash
make -C lbm_examples full_sx1261 MODEM_APP=RELAY_TX
```