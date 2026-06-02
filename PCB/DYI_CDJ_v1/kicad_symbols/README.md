# CDJ v1 KiCad Module Library

This project-local library contains schematic symbols and through-hole module footprints for the breakout boards shown in the project notes:

- `PCF8575_Module_HW331`
- `CD74HC4067_Module_Generic`
- `Arduino_Pro_Micro_USB_C`

KiCad should load them through the project-local `sym-lib-table` and `fp-lib-table` files.

The Arduino Pro Micro USB-C library was imported from:

https://github.com/jueta/Arduino_Pro_Micro_USB_C-Kicad-Library

The two module footprints were rebuilt from the linked product photos and corroborating supplier dimensions. They are drawn as component-side views: when the module is face-up, the silkscreen labels match the real board labels. Before ordering a PCB, print the footprints at 1:1 scale and place the physical boards over them.

Measurement references:

- Linked PCF8575 product photos and `21 mm x 32 mm` dimension image: https://www.aliexpress.com/item/1005009340294771.html
- Equivalent Open-Smart PCF8575 module listed as `33 mm x 21 mm`: https://www.tinytronics.nl/en/communication-and-signals/io-converters/open-smart-pcf8575-io-expander-module-16-extra-io-pins
- Linked HW-178 CD74HC4067 product photos: https://www.aliexpress.com/item/1005006309366590.html
- HW-178 supplier dimensions listed as `17 mm x 40 mm`: https://besomi.com/jo_en/hw-178-cd74hc4067-besomi-mux-module.html
- Equivalent standard 74HC4067 module dimensions listed as `40 mm x 18 mm`: https://protosupplies.com/product/16-ch-analog-digital-mux-module/

- Header pitch is 2.54 mm.
- PCF8575 board outline is nominally `21 mm x 32 mm`.
- PCF8575 left row, top to bottom: `P10`, `P11`, `P12`, `P13`, `P14`, `P15`, `P16`, `P17`, `VDD`, `GND`.
- PCF8575 right row, top to bottom: `P07`, `P06`, `P05`, `P04`, `P03`, `P02`, `P01`, `P00`, `VDD`, `GND`.
- PCF8575 bottom row, left to right: `GND`, `VCC`, `SDA`, `SCL`, `INT`.
- CD74HC4067 HW-178 board outline is nominally `40 mm x 18 mm`. Some suppliers report the width as `17 mm`; the header geometry is the same.
- CD74HC4067 left row, top to bottom: `C15` through `C0`.
- CD74HC4067 right row, top to bottom: `SIG`, `S3`, `S2`, `S1`, `S0`, `EN`, `VCC`, `GND`.
- Arduino Pro Micro USB-C board body is assumed to be `36.80 mm x 17.70 mm`.
- Arduino Pro Micro USB-C top row, USB-C on the left, left to right: `RAW`, `GND`, `RST`, `VCC`, `A3`, `A2`, `A1`, `A0`, `15`, `14`, `16`, `10`.
- Arduino Pro Micro USB-C bottom row, USB-C on the left, left to right: `TX0`, `RX1`, `GND`, `GND`, `2`, `3`, `4`, `5`, `6`, `7`, `8`, `9`.
- Board outlines match your exact modules. Daughterboard mounting holes are shown on `F.Fab` as reference marks only; they are intentionally not drilled into the carrier PCB.

The symbols use named pad numbers such as `SDA`, `P00`, and `C15`, so symbol pins and footprint pads map by signal name instead of fragile numeric pin order.
