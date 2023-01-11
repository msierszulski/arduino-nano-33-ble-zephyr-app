# Arduino nano 33 BLE Zephyr app
Copyright (c) 2022-2023 [Mateusz Sierszulski](https://github.com/msierszulski), [Robert Szczepański](https://github.com/robertszczepanski)

## Getting started
Before getting started, make sure you have a proper Zephyr development
environment.
Please refer to Zephyr's official
[getting started guide](https://docs.zephyrproject.org/latest/getting_started/index.html)
for detailed setup instructions.

The application was created to run on [Arduino Nano 33 BLE sense board](https://store.arduino.cc/products/arduino-nano-33-ble-sense).

### Initialization

The first step is to initialize the workspace folder (``workspace``) where
the ``arduino-nano-33-ble-zephyr-app`` and all Zephyr modules will be cloned. You can do
that by running:

```shell
west init -m https://github.com/msierszulski/arduino-nano-33-ble-zephyr-app --mr main workspace
cd workspace
west update
```

### Build & Run
The application can be built by running:

```shell
cd video-overlays-zephyr-app
west build -p -b arduino_nano_33_ble_sense -s app
```