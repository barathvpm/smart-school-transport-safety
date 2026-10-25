
# ESP32 Firmware

## Purpose

This directory contains the firmware for the Smart School Transport Safety and Monitoring System.

The firmware is intended to run on an ESP32 development board and support BLE beacon monitoring and configured safety-event processing.

## Firmware Status

Update this section to match the current project:

- [ ] Firmware source code added.
- [ ] Firmware compiles successfully.
- [ ] Firmware uploaded to the ESP32.
- [ ] BLE beacon detection tested.
- [ ] Event output checked using the Serial Monitor.
- [ ] Alert communication tested, if implemented.

## Requirements

- ESP32 development board.
- USB data cable.
- Arduino IDE or another compatible development environment.
- ESP32 board support package.
- BLE library compatible with the selected framework.
- BLE beacon or BLE-capable test device.

Add any other hardware or libraries required by the actual source code.

## Installation

1. Install the development environment.
2. Install the ESP32 board support package.
3. Open the firmware source file in this directory.
4. Install the libraries imported by the source file.
5. Connect the ESP32 to the computer.
6. Select the correct board and port.
7. Compile the firmware.
8. Correct any compilation errors.
9. Upload the firmware.
10. Open the Serial Monitor and use the baud rate configured in the code.

## Configuration

Document the settings that your firmware actually supports, such as:

- BLE beacon identifier.
- Beacon scan interval.
- Beacon timeout.
- Event-detection conditions.
- Serial Monitor baud rate.
- Alert destination and communication method, if implemented.

Do not publish passwords, API keys, phone numbers, or other secrets.

## Verification

After uploading, record:

- Whether compilation succeeded.
- Whether the board started correctly.
- Whether the BLE beacon was detected.
- What output appeared in the Serial Monitor.
- Whether configured events were reported correctly.
- Whether communication failures were handled as expected.

Record actual results in `../tests/test_cases.md`.

## Troubleshooting

### ESP32 is not detected
Check the USB data cable, board connection, driver, and selected serial port.

### Compilation fails
Check the board package, required libraries, source code, and selected board.

### BLE beacon is not detected
Check that the beacon is powered on, advertising, within range, and configured as expected. Confirm that the firmware scans for the correct advertisement data.

### Alerts are not received
Confirm that the relevant alert feature has actually been implemented. Then check network connectivity, module wiring, configuration, and service requirements.

## Important

The instructions must be updated if the actual firmware uses a different board, framework, library, or communication method.
