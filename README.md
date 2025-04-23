# STM32-FC Flight Controller

A comprehensive flight controller project based on the STM32F405RG microcontroller, featuring hardware design, firmware, and ground control software.

## Project Structure

- **Firmware/** - STM32F405RG-based flight controller firmware
- **Hardware/** - PCB and schematic design files
- **GroundControl/** - Ground control station software
- **Document/** - Project documentation
- **Data/** - Data logging and configuration files

## Features

- Based on STM32F405RG microcontroller
- USB Device support with CDC (Communication Device Class)
- Hardware Abstraction Layer (HAL) driver support
- Debug and Release build configurations
- ST-Link programming and debugging support

## Development Environment Setup

### Prerequisites

- PlatformIO IDE
- ST-Link V2 programmer
- ARM GCC Toolchain
- STM32CubeMX (for hardware configuration)

### Building the Firmware

1. Clone the repository:

```bash
git clone [repository-url]
cd STM32-FC
```

2. Open the project in PlatformIO IDE

3. Select build configuration:

   - Debug build: Includes debug symbols and optimization level O0
   - Release build: Optimized for performance with O2 level

4. Build the project:
   - For debug: `pio run -e debug`
   - For release: `pio run -e release`

### Flashing the Firmware

Connect your ST-Link programmer to the board and run:

```bash
pio run -t upload
```

## Hardware

The flight controller hardware is designed around the STM32F405RG microcontroller. Detailed hardware documentation and design files can be found in the `Hardware/` directory.

## Ground Control Software

The ground control station software provides a user interface for:

- Flight controller configuration
- Real-time telemetry monitoring
- Flight data logging
- Parameter tuning

See the `GroundControl/` directory for setup and usage instructions.

## Documentation

Detailed documentation including:

- Hardware specifications
- Communication protocols
- Software architecture
- User guides

Can be found in the `Document/` directory.

## Contributing

1. Fork the repository
2. Create your feature branch (`git checkout -b feature/AmazingFeature`)
3. Commit your changes (`git commit -m 'Add some AmazingFeature'`)
4. Push to the branch (`git push origin feature/AmazingFeature`)
5. Open a Pull Request

## License

[Add appropriate license information here]

## Acknowledgments

- STM32 HAL and LL drivers by ST Microelectronics
- STM32 USB Device Library
- [Add other acknowledgments as needed]
