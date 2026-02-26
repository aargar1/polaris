# Polaris
Polaris is a feature-rich development board built around the Lattice iCE40 FPGA, designed for experimentation and small FPGA-based projects. The board provides a practical set of peripherals for graphics, storage, and USB-based interaction, all in a compact and approachable design. I designed it to implement a custom 32-bit microcontroller.

<img width="634" height="475" alt="image" src="https://github.com/user-attachments/assets/cd815a29-ca89-44a4-9d52-621e1e89f86e" />

## Features

- Lattice iCE40 FPGA
- VGA output with audio support
- SD card interface
- 2× USB Type-A ports
- User-controllable LED
- GPIO and SPI headers

## Tooling

Polaris is plug-and-play compatable with the `yosys` toolchain. The [iCEStudio](https://icestudio.io/) development enviornment provides a great ecosystem for development on Polaris and iCE40-based boards in general.

## Acknowlegments

Thanks to the open-source FPGA and KiCad communities, whose tools and documentation made this project possible.

## BOM (Hack Club Blueprint)
| Comment             | Designator                      | Footprint        | LCSC Part # | Direct Link                                                                                              |
| ------------------- | ------------------------------- | ---------------- | ----------- | -------------------------------------------------------------------------------------------------------- |
| 2150                | R11,R3,R7                       | 0603             | C2960889    | [https://www.lcsc.com/product-detail/C2960889.html](https://www.lcsc.com/product-detail/C2960889.html)   |
| 2.7nF               | C15,C16                         | 0603             | C1609       | [https://www.lcsc.com/product-detail/C1609.html](https://www.lcsc.com/product-detail/C1609.html)         |
| Bus                 | J4                              | 2x14 2.54mm      | C725886     | [https://www.lcsc.com/product-detail/C725886.html](https://www.lcsc.com/product-detail/C725886.html)     |
| VGA                 | J1                              | ICD15S13E4GV00LF | C3121412    | [https://www.lcsc.com/product-detail/C3121412.html](https://www.lcsc.com/product-detail/C3121412.html)   |
| 74CBTLV3126PW,118   | U2                              | TSSOP-14         | C478017     | [https://www.lcsc.com/product-detail/C478017.html](https://www.lcsc.com/product-detail/C478017.html)     |
| 47k                 | R17,R19–R24,R27,R30,R31         | 0603             | C25819      | [https://www.lcsc.com/product-detail/C25819.html](https://www.lcsc.com/product-detail/C25819.html)       |
| WM8524CGEDT         | U3                              | TSSOP-16         | C146242     | [https://www.lcsc.com/product-detail/C146242.html](https://www.lcsc.com/product-detail/C146242.html)     |
| 1Ω                  | R28,R29                         | 0603             | C22936      | [https://www.lcsc.com/product-detail/C22936.html](https://www.lcsc.com/product-detail/C22936.html)       |
| NRS4018T2R2MDGJ     | L1                              | SRN4018          | C92959      | [https://www.lcsc.com/product-detail/C92959.html](https://www.lcsc.com/product-detail/C92959.html)       |
| W25Q16JVSNIQ        | U4                              | SOIC-8           | C115407     | [https://www.lcsc.com/product-detail/C115407.html](https://www.lcsc.com/product-detail/C115407.html)     |
| 330Ω                | R35,R36,R37                     | 0603             | C23138      | [https://www.lcsc.com/product-detail/C23138.html](https://www.lcsc.com/product-detail/C23138.html)       |
| TLV62568DBVR        | U7                              | SOT-23-5         | C163219     | [https://www.lcsc.com/product-detail/C163219.html](https://www.lcsc.com/product-detail/C163219.html)     |
| 100nF               | C1,C2,C3,C4,C5,C10,C14,C27,C30  | 0603             | C14663      | [https://www.lcsc.com/product-detail/C14663.html](https://www.lcsc.com/product-detail/C14663.html)       |
| SW_Push             | SW1                             | 6mm              | C455112     | [https://www.lcsc.com/product-detail/C455112.html](https://www.lcsc.com/product-detail/C455112.html)     |
| 1.5k                | R32,R33                         | 0603             | C22843      | [https://www.lcsc.com/product-detail/C22843.html](https://www.lcsc.com/product-detail/C22843.html)       |
| USB_A               | J5,J6                           | XKB U231-091N    | C2880618    | [https://www.lcsc.com/product-detail/C2880618.html](https://www.lcsc.com/product-detail/C2880618.html)   |
| 4.7uF               | C6,C7,C8,C9,C17,C18,C19         | 0603             | C19666      | [https://www.lcsc.com/product-detail/C19666.html](https://www.lcsc.com/product-detail/C19666.html)       |
| ICE40UP5K-SG48I     | U1                              | QFN-48           | C2678152    | [https://www.lcsc.com/product-detail/C2678152.html](https://www.lcsc.com/product-detail/C2678152.html)   |
| Flashenable         | JP1                             | 1x02 2.54mm      | C5360898    | [https://www.lcsc.com/product-detail/C5360898.html](https://www.lcsc.com/product-detail/C5360898.html)   |
| LED_BGKR            | D1                              | 5mm RGB          | C7117555    | [https://www.lcsc.com/product-detail/C7117555.html](https://www.lcsc.com/product-detail/C7117555.html)   |
| 820Ω                | R13,R14                         | 0603             | C23253      | [https://www.lcsc.com/product-detail/C23253.html](https://www.lcsc.com/product-detail/C23253.html)       |
| 10uF                | C23,C24,C25,C26,C28,C29,C31,C32 | 0805             | C15850      | [https://www.lcsc.com/product-detail/C15850.html](https://www.lcsc.com/product-detail/C15850.html)       |
| 560Ω                | R25,R26                         | 0603             | C23204      | [https://www.lcsc.com/product-detail/C23204.html](https://www.lcsc.com/product-detail/C23204.html)       |
| 536Ω                | R1,R5,R9                        | 0603             | C23201      | [https://www.lcsc.com/product-detail/C23201.html](https://www.lcsc.com/product-detail/C23201.html)       |
| SX5M25.000M20F30TNN | X1                              | 25MHz Osc        | C2901535    | [https://www.lcsc.com/product-detail/C2901535.html](https://www.lcsc.com/product-detail/C2901535.html)   |
| MIC5504-3.3YM5      | U8                              | SOT-23-5         | C41348078   | [https://www.lcsc.com/product-detail/C41348078.html](https://www.lcsc.com/product-detail/C41348078.html) |
| Prog                | J2                              | 1x08 2.54mm      | C5156616    | [https://www.lcsc.com/product-detail/C5156616.html](https://www.lcsc.com/product-detail/C5156616.html)   |
| FerriteBead_Small   | FB1,FB2                         | 0603             | C1027       | [https://www.lcsc.com/product-detail/C1027.html](https://www.lcsc.com/product-detail/C1027.html)         |
| 4300Ω               | R12,R4,R8                       | 0603             | C23159      | [https://www.lcsc.com/product-detail/C23159.html](https://www.lcsc.com/product-detail/C23159.html)       |
| 1uF                 | C12,C13                         | 0603             | C15849      | [https://www.lcsc.com/product-detail/C15849.html](https://www.lcsc.com/product-detail/C15849.html)       |
| 2.2uF               | C11                             | 0603             | C23630      | [https://www.lcsc.com/product-detail/C23630.html](https://www.lcsc.com/product-detail/C23630.html)       |
| 10k                 | R15,R16,R18,R34                 | 0603             | C25804      | [https://www.lcsc.com/product-detail/C25804.html](https://www.lcsc.com/product-detail/C25804.html)       |
| 1070Ω               | R10,R2,R6                       | 0603             | C177957     | [https://www.lcsc.com/product-detail/C177957.html](https://www.lcsc.com/product-detail/C177957.html)     |
| Barrel_Jack         | J7                              | PJ-063AH         | C22434582   | [https://www.lcsc.com/product-detail/C22434582.html](https://www.lcsc.com/product-detail/C22434582.html) |
| SD_Card             | J3                              | 693063010911     | C341097     | [https://www.lcsc.com/product-detail/C341097.html](https://www.lcsc.com/product-detail/C341097.html)     |
| SN74AHC00PWR        | U9                              | TSSOP-14         | C8143       | [https://www.lcsc.com/product-detail/C8143.html](https://www.lcsc.com/product-detail/C8143.html)         |


## License
This project is licensed under the CERN Open Hardware Licence Version 2. If you would like to use Assemblage for a patently non-commercial or educational application, but cannot do so under this license, please contact me via an issue; I would be happy to work something out.
