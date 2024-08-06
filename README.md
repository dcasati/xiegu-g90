# Configuring USB-D Mode on Xiegu G90 Using FLRig

This guide provides the steps to configure the Xiegu G90 for **USB-D** mode by entering CI-V commands in the FLRig configuration window.

## Prerequisites

- **FLRig** installed and running on your computer.
- **Xiegu G90** connected via USB or compatible CAT interface.

## Steps to Configure USB-D Mode in FLRig

### 1. Open FLRig

- Launch FLRig on your computer.

### 2. Access Configuration

- Go to `Config` > `Setup`.

### 3. Select Transceiver

- Ensure the **Xiegu G90** is selected as your transceiver.

### 4. Configure Serial Port

- Set up the serial port settings to match your radio configuration:
  - **Port:** The COM port your radio is connected to (e.g., `COM3` or `/dev/ttyUSB0` or `/dev/tty-digirig`).
  - **Baud Rate:** 19200
  - **Data Bits:** 8
  - **Stop Bits:** 1
  - **Parity:** None

### 5. Navigate to the Commands Tab

- Go to the **Start/Exit** tab within the configuration window.

### 6. Enter CI-V Commands

- Under the **Start** section, add the CI-V command for USB-D mode:

  ```plaintext
  USB-D Mode: FE FE 70 E0 26 00 01 01 FD
