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

## License
This project is licensed under the CERN Open Hardware Licence Version 2. If you would like to use Assemblage for a patently non-commercial or educational application, but cannot do so under this license, please contact me via an issue; I would be happy to work something out.
