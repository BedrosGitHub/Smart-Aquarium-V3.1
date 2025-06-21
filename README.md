# Smart Aquarium V3.1 🐠🌊

Welcome to the Smart Aquarium V3.1 repository! This project aims to enhance your aquarium experience by providing a robust controller based on the ESP8266. With web-based management, you can easily control various aspects of your aquarium from anywhere. 

[![Download Releases](https://img.shields.io/badge/Download%20Releases-Click%20Here-brightgreen)](https://github.com/BedrosGitHub/Smart-Aquarium-V3.1/releases)

## Table of Contents

1. [Overview](#overview)
2. [Features](#features)
3. [Installation](#installation)
4. [Usage](#usage)
5. [Control Modes](#control-modes)
6. [Web UI](#web-ui)
7. [API Documentation](#api-documentation)
8. [OTA Updates](#ota-updates)
9. [Time Synchronization](#time-synchronization)
10. [Persistent Settings Storage](#persistent-settings-storage)
11. [Contributing](#contributing)
12. [License](#license)
13. [Contact](#contact)

## Overview

The Smart Aquarium V3.1 is designed to make aquarium management easier and more efficient. It leverages the power of the ESP8266 microcontroller to offer various control modes and features that enhance user experience. Whether you want to manage your aquarium manually or through automated schedules, this controller provides the flexibility you need.

## Features

- **Web-based Management**: Control your aquarium from any device with a web browser.
- **Four Relay Outputs**: Manage lights, pumps, and other devices.
- **Multiple Control Modes**: Choose from manual, scheduled, timer, or toggle modes.
- **OTA Updates**: Easily update your firmware over-the-air.
- **Time Synchronization**: Sync your aquarium's clock with NTP servers.
- **Persistent Settings Storage**: Save your settings even after power loss.
- **Responsive Web UI**: Enjoy a user-friendly interface for easy control.
- **RESTful API**: Integrate with other applications or control your aquarium remotely.

## Installation

To get started with Smart Aquarium V3.1, follow these steps:

1. **Clone the Repository**:
   ```bash
   git clone https://github.com/BedrosGitHub/Smart-Aquarium-V3.1.git
   ```

2. **Install Required Libraries**:
   You will need the following libraries to compile the project:
   - ESP8266WiFi
   - AsyncWebServer
   - LittleFS
   - NTPClient
   - ArduinoJson

   You can install these libraries through the Arduino Library Manager.

3. **Upload the Code**:
   Open the project in the Arduino IDE and upload it to your ESP8266.

4. **Configure Wi-Fi**:
   Edit the `config.h` file to enter your Wi-Fi credentials.

5. **Compile and Upload**:
   After configuring, compile and upload the code to your ESP8266.

## Usage

Once the installation is complete, you can access the web interface by entering the IP address of your ESP8266 in your web browser. The default IP address is usually `192.168.1.1`, but it may vary depending on your network configuration.

## Control Modes

Smart Aquarium V3.1 offers four control modes to suit your needs:

1. **Manual Mode**: Control the relays directly from the web interface.
2. **Scheduled Mode**: Set specific times for the relays to turn on or off.
3. **Timer Mode**: Use a timer to control the relays for a set duration.
4. **Toggle Mode**: Switch the relays on and off at regular intervals.

## Web UI

The web UI is designed to be intuitive and user-friendly. You can easily navigate through different sections to manage your aquarium settings. The interface displays the current status of each relay, along with options to change settings.

![Web UI Screenshot](https://via.placeholder.com/800x400?text=Web+UI+Screenshot)

## API Documentation

Smart Aquarium V3.1 provides a RESTful API for remote control. Below are some of the key endpoints:

- **GET /status**: Retrieve the current status of the aquarium.
- **POST /control**: Send commands to control the relays.
- **GET /settings**: Fetch current settings.
- **POST /settings**: Update settings.

Refer to the API documentation in the repository for more details on each endpoint.

## OTA Updates

Over-the-air (OTA) updates allow you to update the firmware without needing to connect your ESP8266 to a computer. To perform an OTA update:

1. Ensure your ESP8266 is connected to the internet.
2. Upload the new firmware version using the web interface.

You can download the latest releases from the [Releases section](https://github.com/BedrosGitHub/Smart-Aquarium-V3.1/releases).

## Time Synchronization

Smart Aquarium V3.1 uses the Network Time Protocol (NTP) to keep the time synchronized. This feature is essential for scheduled operations and ensures that your aquarium operates on a consistent schedule.

## Persistent Settings Storage

The settings are stored in LittleFS, allowing you to retain your configurations even after a power outage. This feature ensures that your aquarium operates according to your preferences without needing to reconfigure every time.

## Contributing

We welcome contributions to improve Smart Aquarium V3.1. If you have ideas or enhancements, please fork the repository and submit a pull request. Make sure to follow the coding standards and include tests for new features.

## License

This project is licensed under the MIT License. See the [LICENSE](LICENSE) file for details.

## Contact

For any questions or feedback, feel free to reach out:

- **GitHub**: [BedrosGitHub](https://github.com/BedrosGitHub)
- **Email**: bedros@example.com

Thank you for checking out Smart Aquarium V3.1! We hope you enjoy managing your aquarium with ease and efficiency. For more updates and releases, visit the [Releases section](https://github.com/BedrosGitHub/Smart-Aquarium-V3.1/releases).