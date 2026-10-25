
# Hardware Documentation

## 1. Overview

The proposed system uses an ESP32 development board as the main controller and a BLE beacon as the source of wireless beacon advertisements.

Additional sensors and communication modules may be included depending on the final prototype.

## 2. Main Components

| Component | Purpose |
|---|---|
| ESP32 development board | Main controller and BLE scanning |
| BLE beacon | Broadcasts BLE advertisements |
| USB cable | Programming and initial power |
| IR sensor (optional) | Provides an additional input if included in the design |
| GSM module (optional) | Cellular communication, if implemented |
| Wi-Fi connection (optional) | Network communication, if implemented |
| Jumper wires and breadboard | Prototyping connections, if required |

## 3. Connections

Document the actual wiring used in your prototype.

| Component | ESP32 connection | Status |
|---|---|---|
| BLE beacon | Wireless; no direct signal wire required for normal BLE advertisements | Verify |
| IR sensor | Record the actual GPIO and power connections | Update |
| GSM module | Record the actual UART and power connections | Update |
| Other sensor | Record the actual GPIO and power connections | Update |

Do not copy pin numbers from an example without checking your circuit.

## 4. Power Supply

Use a power source appropriate for the ESP32 board and any connected modules. GSM modules may require a power supply capable of handling their current peaks.

Check the voltage and current requirements of each component before connecting it. Do not assume that every module can be powered directly from the ESP32's 3.3 V output.

## 5. Assembly Procedure

1. Identify the ESP32 board and other components.
2. Check each component's operating voltage.
3. Connect the components according to the verified circuit diagram.
4. Check wiring and polarity before powering the circuit.
5. Upload and test the firmware.
6. Verify BLE detection and any configured sensor inputs.
7. Test communication modules separately before integrating them.
8. Record photographs of the actual prototype, if available.

## 6. Hardware Verification

Record the following information:

- ESP32 board model.
- BLE beacon model or test-device type.
- Sensor models and GPIO assignments.
- Communication module model, if used.
- Power-supply specifications.
- Successful tests and known issues.

## 7. Safety Note

Disconnect power before changing wiring. Verify voltage levels, polarity, and module power requirements. Test the prototype on a workbench before considering any installation in a vehicle.
