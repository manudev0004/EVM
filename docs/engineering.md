# Prototype Engineering

[Back to the project](../README.md) · [Original report PDF](../EVM%20Report.pdf)

## Technical Summary

The prototype coordinates fingerprint input, a camera-based identity-checking flow, physical candidate buttons and LCD feedback through Raspberry Pi and Python.

## Hardware and software

| Part | Role |
|---|---|
| Raspberry Pi 4 | Coordinates the prototype and GPIO devices |
| R307 fingerprint scanner | Fingerprint capture and matching |
| Raspberry Pi camera | Input for the face-verification flow |
| L1602 / 16×2 LCD | Prompts, confirmation and results |
| Five candidate buttons | Physical selection inputs |
| Speaker/buzzer and wiring | User feedback and connections |
| Python, GPIO and serial libraries | Application logic and device interfaces |

The code appendix uses JSON for vote counts and references a separate `Face_Recog` module.

## Interaction Sequence

The report describes fingerprint matching and a camera-based face check before a candidate selection is accepted. The application checks prior voting state, records the selection and displays confirmation. A separate interaction exposes candidate counts on the LCD.

Each step connects software state with a physical action: a scanner result, camera input, button press or display update. This makes sequencing and feedback important parts of the embedded application.

## Evidence and Scope

The report dated 2 May 2023 includes flow diagrams, result screens, equipment and an illustrative Python appendix. The supplied photographs show the enclosure, buttons, fingerprint scanner and LCD messages.

The full face-recognition module and a complete executable source tree are not included in this portfolio. The tamper-alert photograph documents a displayed message; it does not establish encrypted storage or a validated security property. The material should be read as an academic voting-machine prototype rather than an independently certified election system.
