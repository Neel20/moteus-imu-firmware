# Moteus IMU Firmware

Custom firmware for the Moteus C1 motor controller with integrated LSM6DSV16X IMU support.

## Overview

This firmware extends the Moteus C1 to provide real-time 6-axis motion data (accelerometer and gyroscope) from the LSM6DSV16X IMU. It enables simultaneous motor control and inertial measurement in a single device.

## Features

- Raw accelerometer and gyroscope data access from LSM6DSV16X IMU
- Custom "Type 5" firmware mode for stable 6-DOF operation
- I2C communication interface
- Python-based data acquisition tools
- Sub-0.1 degree position accuracy maintained

## Usage

Run the provided Python script to read IMU data:
```bash
python readIMUma6.py
```

## Technical Details

This implementation includes:
- LSM6DSV16X IMU integration with cascaded communication protocols
- Custom C++ firmware modifications across multiple system files
- Real-time data streaming without system freezing issues
- Compatible with existing Moteus motor control functionality

## Credits

This project builds upon:
- Original Moteus firmware by [mjbots](https://github.com/mjbots/moteus)
- Extended firmware customizations by [Otavio Good](https://github.com/otaviogood/moteus)

## License

This project is licensed under the Apache License 2.0 - see the [LICENSE](LICENSE) file for details.

Based on the original [Moteus firmware](https://github.com/mjbots/moteus) by mjbots.
