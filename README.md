# DebugProbe-RP2040-Zero

- [Official Repository of the Firmwares and source codes is raspberrypi/debugprobe](https://github.com/raspberrypi/debugprobe)

## Firmware Instration

- Copy the latest DebugProbe Firmware for RP2040 (released with the name as
  debugprobe_on_pico.uf2) to RP2040-Zero

## Pin Assign

| GPIO | Connection | Function |
| :--- | :--------- | :------- |
| GP2  | SWD        | SWDIO    |
| GP3  |            | SWCLK    |
| GP4  | UART       | TXD      |
| GP5  |            | RXD      |

## Wiring

### UART

| DebugProbe | PIN |  -  | PIN | Device |
| ---------: | --: | :-: | :-- | :----- |
|        TXD | GP4 |     | GP1 | RXD    |
|        RXD | GP5 |     | GP0 | TXD    |

### SWD

| DebugProbe | PIN |  -  | Device PIN |
| ---------: | --: | :-: | :--------- |
|      SWDIO | GP2 |     | SWDIO      |
|        GND | GND |     | GND        |
|      SWCLK | GP3 |     | SWCLK      |
