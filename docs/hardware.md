# Hardware Selection

## Main Computational Module

For this project, the [`Orange Pi Zero 2W`]() with **4GB LPDDR4** has been selected as the main computational module. This single-board computer, based on the [`Allwinner H618 (ARM Cortex-A53)`]() processor, is an optimal choice due to its performance and energy efficiency. The module supports both wireless and wired communication interfaces, making it versatile for a variety of applications.

## Wired Ethernet Connection

To ensure wired Ethernet connectivity, the [`Orange Pi Expansion Board`]() is used, providing speeds of up to **100Mbps**. This expansion also offers additional ports to enhance the system’s functionality.

## Analog Signal Digitization

For acquiring data from analog sensors, the [`ADS1115 16-Bit 4-Channel IIC ADC Converter with PGA`]() is used. This module supports 4 channels, allowing multiple sensors to be connected simultaneously, and provides accurate analog signal measurements with **16-bit** resolution.

## Sensors for Measuring AC Current

For measuring alternating current, **inductive sensors** are planned to be used. The specific models have not yet been selected, but for measuring currents in **220-260V** networks at **50-60 Hz**, the following models are suitable:

- [`SCT-013-000`](): A current sensor for up to **100A**, supporting non-invasive measurement. It is easy to use, with a 3.5 mm interface.
- [`YHDC SCT-013-050`](): A model designed for measuring currents up to **50A**, also supporting measurements in the specified voltage and frequency ranges.
- [`PZEM-004T`](): A module for monitoring AC current, voltage, power, and frequency, with the ability to connect to microcontrollers via UART.

These models can be tested to determine the best compatibility with the project, depending on the required accuracy and the range of current to be measured.
