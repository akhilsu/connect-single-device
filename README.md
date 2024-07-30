# connect-single-device

This is a sample python to test the device connectivity

# Netmiko Device Connection Example

This repository contains a simple example of how to connect to a Cisco IOS device using the Netmiko library in Python.

## Table of Contents

- [Introduction](#introduction)
- [Installation](#installation)
- [Usage](#usage)
- [License](#license)

## Introduction

Netmiko is a multi-vendor library that simplifies the process of connecting to network devices via SSH. This example demonstrates how to connect to a Cisco IOS device using Netmiko.

## Installation

To run this example, you need to have Python installed on your system. You can install the required dependencies using `pip`.

1. Clone the repository:

    ```sh
    git clone https://github.com/akhilsu/connect-single-device.git
    cd connect-single-device
    ```

2. Create a virtual environment (optional but recommended):

    ```sh
    python -m venv venv
    source venv/bin/activate  # On Windows use `venv\Scripts\activate`
    ```

3. Install the required packages:

    ```sh
    pip install -r requirements.txt
    ```

## Usage

1. Update the `device` dictionary in `connect.py` with the appropriate details for your Cisco IOS device:

    ```python
    device = {
        "device_type" : "cisco_ios",
        "ip" : "10.10.10.10",
        "username" : "admin",
        "password" : "admin@123",
        "port" : 22
    }
    ```

2. Run the script:

    ```sh
    python connect.py
    ```

    If the connection is successful, you will see the message "Device connected successfully" in the console.

## License

This project is licensed under the MIT License. See the [LICENSE](LICENSE) file for details.
