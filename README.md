# GOJIRA-01: Rugged Modular Cyberdeck

**GOJIRA-01** is a modular, armored cyberdeck featuring a Japanese industrial sci-fi design inspired by mecha aesthetics and field seismic/radiation monitoring instruments.

## Key Features
- **Compute Core**: Raspberry Pi 5 (8GB/16GB) with PCIe NVMe 1TB SSD HAT.
- **Dual Display System**: 8.8" Ultrawide IPS (1920x480) + 1.3" Monochrome I2C OLED telemetry monitor.
- **Industrial Connectivity**: Panel-mount Neutrik etherCON RJ45 (D-Series) with internal 802.3at PoE+ splitter and dual SMA RF bulkheads for RTL-SDR.
- **Hybrid Power**: 4x 18650 LiFePO4 UPS with Ideal Diode OR-ing for seamless switching between battery, USB-C PD, and PoE+.
- **Reactive Dorsal Cooling**: CNC-milled aluminum heatsink fins with 12x WS2812B addressable LEDs reacting to network link and CPU thermal load.

## Repository Structure
- `firmware/gojira_core.py`: Unified Python controller for the I2C OLED display and SPI WS2812B LEDs.
- `firmware/gojira-core.service`: Systemd service unit for auto-start on boot.
- `hardware/WIRING_AND_SPECS.md`: Electrical schematic, GPIO pinout, and Neutrik D-Series cutout dimensions.
- `cad/`: Placeholder folder for PA12-CF 3D printable STL/STEP chassis files.
