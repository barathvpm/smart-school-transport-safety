
# Test Cases

## 1. Purpose

This document defines test cases for evaluating the Smart School Transport Safety and Monitoring System.

The tests cover BLE beacon detection, event processing, restart behaviour, and optional alert communication.

**Important:** These are test procedures, not evidence that the tests have passed. Update the result and evidence columns after running each test on the actual prototype.

## 2. Result Definitions

- **Pass:** The observed result matches the expected result.
- **Fail:** The observed result does not match the expected result.
- **Not Tested:** The test has not yet been performed.
- **Blocked:** The test could not be performed because a required component or feature is unavailable.

## 3. Test Cases

| Test ID | Test | Procedure | Expected Result | Result |
|---|---|---|---|---|
| TC-01 | ESP32 startup | Power on or reset the ESP32 | Firmware starts and produces the expected startup output | Not Tested |
| TC-02 | Beacon detected | Switch on the configured test beacon within the test range | Firmware identifies the configured beacon | Not Tested |
| TC-03 | Beacon missing | Switch off or move the test beacon out of range | Firmware follows its configured missing-beacon rule, if implemented | Not Tested |
| TC-04 | Beacon returns | Restore the beacon after a missing-beacon event | Firmware detects it again and reports the expected state | Not Tested |
| TC-05 | Repeated advertisements | Keep the beacon advertising continuously | Firmware handles repeated advertisements without unexpected behaviour | Not Tested |
| TC-06 | ESP32 restart | Restart the controller during testing | Firmware starts again and resumes its configured monitoring behaviour | Not Tested |
| TC-07 | Communication unavailable | Disable the network or disconnect the optional communication module | Failure is handled and reported as designed | Not Tested |
| TC-08 | Alert delivery | Trigger a test event with the alert channel configured | The intended test recipient receives the alert, if alerting is implemented | Not Tested |
| TC-09 | Invalid beacon data | Use a beacon or test advertisement that does not match the configured identifier | Firmware handles the unmatched data as expected | Not Tested |
| TC-10 | Event logging | Trigger a supported test event | The event is logged or displayed with the expected information | Not Tested |

## 4. Test Record Template

For every test, record:

- Test ID:
- Date and time:
- Hardware configuration:
- Firmware version or commit:
- Procedure followed:
- Expected result:
- Actual result:
- Pass / Fail / Not Tested / Blocked:
- Evidence filename or screenshot:
- Notes or corrective action:

## 5. Testing Notes

1. Begin with the ESP32 and BLE beacon before adding optional modules.
2. Use a controlled test environment.
3. Repeat tests where necessary to check consistency.
4. Record actual observations rather than assuming the expected result occurred.
5. Keep simulated results separate from hardware test results.
6. Do not test by placing an unvalidated prototype into operational school transport.

## 6. Current Test Summary

Total tests: 10

Passed: Update after testing.

Failed: Update after testing.

Not tested: Update after testing.

Blocked: Update after testing.

## 7. Limitations

Successful bench testing does not establish that the system is reliable enough for real school transport operations. Additional validation, privacy safeguards, and appropriate approvals would be required before real-world use.
