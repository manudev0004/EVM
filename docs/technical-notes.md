# Technical Notes

[Overview](../README.md) · [Original report](../EVM%20Report.pdf)

These notes describe the archived report and files, rather than a new hardware validation.

## Controller and interfaces

The report lists a Raspberry Pi 4, Raspberry Pi camera, R307 fingerprint scanner, L1602 display, speaker, buttons, jumper wires and breadboard. Its Python appendix imports `RPi.GPIO`, `gpiozero`, `serial`, `adafruit_fingerprint`, `Adafruit_CharLCD`, JSON support and a local `Face_Recog` module.

Fingerprint communication is shown over UART. GPIO buttons represent candidate choices and other interactions. The LCD displays prompts, confirmation and results. Vote counts are read from and written to `votes.json` in the appendix.

## Verification flow

The code excerpt checks the fingerprint sensor and then calls `Face_Recog.detect_face(...)`. The results section illustrates rejecting a repeat vote. The local face-recognition module, enrollment data and complete persistence logic are absent, so their implementation should not be inferred from a function call or screenshot.

## Evidence boundaries

| Material | What it supports |
|---|---|
| Device photographs | A physical prototype with LCD, fingerprint scanner and buttons |
| Report result screens | Examples of verification and voting interactions |
| Python appendix | Illustrative GPIO, serial, LCD and JSON integration |
| Tamper-alert photograph | The prototype displaying a tamper message |

The report contains broader security and online-voting claims. This archive does not provide a deployed online service, cryptographic audit, tamper-resistance evaluation or biometric test dataset. A restricted results-display interaction is also not the same as a complete authorization system.
