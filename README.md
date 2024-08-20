# xtensa-alire-index

> Alire index for xtensa LX7 toolchain

This repo contains the Alire index for the xtensa LX7 toolchain. 
It allows you installing xtensa LX7 toolchain for ESP32 boards such as

* [ESP32-S2](https://www.espressif.com/en/products/socs/esp32-s2)
* [ESP32-S3](https://www.espressif.com/en/products/socs/esp32-s3)

NOTE: **No GNAT runtime is provided!**

## Install

```sh
alr index --reset-community
alr index --add git+https://github.com/reznikmm/xtensa-alire-index.git --name xtensa
alr toolchain --select gnat_xtensa_elf gprbuild
```

After installing you will have GCC with `xtensa-esp32-elf` target:

```sh
$ gprconfig --show-targets
List of targets supported by a compiler:
xtensa-esp32-elf
```

## Related resources

* [Telegram group "Ada Xtensa"](https://t.me/+8W6Y75pkslU1ZDgx)
* [Experiments with ESP32-H2](https://forum.ada-lang.io/t/experiments-with-risc-v/930)
* [Ada & FreeRTOS on ESP32 H2](https://forward-in-code.blogspot.com/2024/07/ada-freertos-on-esp32-h2.html)
* [ESP-IDF Ada Binding](https://github.com/jklmnn/esp-idf-ada-bindings)
* [A baremetal, single C header ESP32 SDK](https://github.com/cpq/mdk)
* [HiRTOS on ESP32-C3](https://github.com/jgrivera67/HiRTOS)
