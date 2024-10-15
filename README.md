# Network Power Quality Monitoring

## Project Overview

The Network Power Quality Monitoring project is designed to collect, analyze, and visualize key metrics related to the quality of an electrical power network. 
It continuously monitors the critical parameters of the power supply to ensure stability and detect deviations that could indicate potential issues. 
The system provides real-time data on frequency, voltage, and their deviations, allowing for proactive maintenance and issue resolution.

## Key Features

- Frequency Monitoring: Tracks the real-time frequency of the power network and ensures it stays within acceptable limits.
- Frequency Deviation: Calculates the deviation from the nominal frequency to detect abnormal fluctuations that may affect connected devices.
- Voltage Monitoring: Continuously measures the voltage supplied to the network and ensures compliance with predefined thresholds.
- Voltage Deviation: Identifies any deviation from the expected voltage levels, which may signal underlying issues such as overvoltage or undervoltage.

## Metrics Collected

- Frequency (Hz): The rate at which the alternating current (AC) power is oscillating. Nominal frequency is typically 50 Hz or 60 Hz, depending on the region.
- Frequency Deviation (Hz): The difference between the actual frequency and the nominal frequency. Frequency stability is critical for power-sensitive equipment.
- Voltage (V): The magnitude of electrical potential delivered to the network. Monitoring ensures the voltage remains stable and within the allowed operational range.
- Voltage Deviation (V): The deviation from the expected voltage level. Sudden deviations can cause equipment malfunction or damage.

## Project Structure

- `service1/`: Handles real-time frequency and voltage data collection.
- `service2/`: Provides statistical analysis and deviation detection for the collected data.
- `shared-libraries/`: Common libraries and utilities shared across services.
- `scripts/`: Deployment scripts and CI/CD configurations.

## Usage

The monitoring tool collects data in real-time and outputs the following metrics:
- Current Frequency
- Frequency Deviation
- Current Voltage
- Voltage Deviation

You can also configure the system to trigger alerts when the deviation exceeds the allowed thresholds.

## How to Clone the Project

1. Clone the main repository:
   ```bash
   git clone https://github.com/username/main-project.git
   ```
2. Initialize and update submodules:
   ```bash
   git submodule update --init --recursive
   ```

## Building the Project

Each service has its own `go.mod` and can be built independently. For example, to build `service1`:
   ```bash
   cd service1
   make build
   ```
3. To build the entire project and its dependencies:
   ```bash
   ./scripts/build-all.sh
   ```

## Future Enhancements

- Data Visualization: Implement graphical representation of the collected data (e.g., using Grafana or a similar tool).
- Alerting System: Integration with an email or SMS notification service to alert users when critical deviations occur.
- Historical Analysis: Enable the storage of long-term historical data for trend analysis and reporting.

## Contributing

Please refer to each service's individual `README.md` file for more details on contributing. The main repository handles overall project coordination and documentation.

## License
This project is licensed under the MIT License – see the [LICENSE](/LICENSE) file for details.

