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

### RP2040-Zero Pin Diagram

| Func. |  Pin |  -  | Pin | Func.     |
| ----: | ---: | :-: | :-- | :-------- |
|       |   5V |     | GP0 |           |
|       |  GND |     | GP1 |           |
|       |  3V3 |     | GP2 | SWD SWDIO |
|       | GP29 |     | GP3 | SWD SWCLK |
|       | GP28 |     | GP4 | UART TXD  |
|       | GP27 |     | GP5 | UART RXD  |
|       | GP26 |     | GP6 |           |
|       | GP15 |     | GP7 |           |
|       | GP14 |     | GP8 |           |

GP9-13 are ommited above diagram.

### UART

| DebugProbe | PIN |  -  | PIN | Device |
| ---------: | --: | :-: | :-- | :----- |
|        TXD | GP4 |     | GP1 | RXD    |
|        RXD | GP5 |     | GP0 | TXD    |
|        GBD | GND |     | GND | GND    |

### SWD

| DebugProbe | PIN |  -  | Device PIN |
| ---------: | --: | :-: | :--------- |
|      SWDIO | GP2 |     | SWDIO      |
|        GND | GND |     | GND        |
|      SWCLK | GP3 |     | SWCLK      |
