# Raspberry Pi Voting Prototype

<p><img src="assets/readme/overview.svg" width="100%" alt="Raspberry Pi voting prototype combines identity checks, candidate buttons and LCD feedback"></p>

A physical voting-machine prototype combining fingerprint verification, a camera-based identity check, button inputs and a local results display.

![Technology: Raspberry Pi and Python](https://skillicons.dev/icons?i=raspberrypi,python&theme=light)

<p align="center">
<a href="#voting-flow"><img src="assets/readme/nav-voting-flow.svg" width="328" height="88" alt="Click to open Voting Flow"></a>
<a href="#prototype-gallery"><img src="assets/readme/nav-prototype-photos.svg" width="328" height="88" alt="Click to open Prototype Photos"></a>
<br>
<a href="docs/engineering.md"><img src="assets/readme/nav-technical-guide.svg" width="328" height="88" alt="Click to open Technical Guide"></a>
<a href="EVM%20Report.pdf"><img src="assets/readme/nav-project-report.svg" width="328" height="88" alt="Click to open Project Report (PDF)"></a>
</p>

## Contents

- [Project Summary](#project-summary)
- [Voting Flow](#voting-flow)
- [Prototype Gallery](#prototype-gallery)
- [Engineering Work](#engineering-work-shown)

<table>
<tr><td width="50%"><img src="evm_image1.jpg" width="350" alt="Voting prototype with candidate buttons, fingerprint scanner and LCD confirmation"></td><td width="50%"><img src="evm_image2.jpg" width="350" alt="LCD displaying the recorded count for candidate four"></td></tr>
<tr><td>Vote confirmation on the assembled prototype</td><td>Candidate count on the local display</td></tr>
</table>

## Project Summary

The prototype brings sensor input, identity checks and a physical voting interface into one Raspberry Pi application. The voting flow combines a fingerprint check with camera-based face verification before accepting a candidate-button input. An LCD guides the user through the process and displays confirmation.

The work connects identity-checking steps to a physical interaction: the person verifies their identity, chooses a candidate and receives confirmation on the display. The report and photographs make the assembled hardware and its feedback screens visible.

## Voting Flow

<p><img src="assets/readme/voting-flow.svg" width="840" alt="Voting flow: verify identity, check prior voting state, select a candidate, record the vote and confirm on the LCD; rejected checks do not record a vote"></p>

1. Start the identity-checking sequence.
2. Match the fingerprint and perform the camera-based face check.
3. Check whether the person has already voted.
4. Accept a candidate-button selection and record the vote.
5. Show confirmation, with a separate interaction for displaying results.

The report illustrates the repeat-vote check in its results section. The [technical guide](docs/engineering.md) explains the hardware interfaces, storage approach and supporting evidence.

## Prototype gallery

| Fingerprint prompt | Tamper-alert screen |
|---|---|
| ![LCD asking the user to place a finger on the scanner](evm_image3.jpg) | ![LCD displaying the tamper-alert message](photo_2024-04-01_02-46-06.jpg) |

| Enclosure and side profile |
|---|
| ![Existing photograph showing the voting-machine enclosure from the side](evm_image4.jpg) |

These photographs show the constructed enclosure, LCD, buttons and fingerprint scanner. The report explains the associated interaction and application logic.

## Engineering work shown

- Coordinating physical inputs, a serial sensor and an LCD through Python on Raspberry Pi.
- Connecting identity-checking steps to a device interaction sequence.
- Recording selections and displaying local results in an academic prototype.
- Documenting hardware work with a report, code excerpt and photographs.

## Read the evidence

The [original report](EVM%20Report.pdf), dated **2 May 2023**, contains design context, flow diagrams, result screens, equipment and the code appendix. It also discusses wider online-voting ideas; these should be distinguished from the physical prototype preserved here.

[**Open the technical guide for components, interaction sequencing and report context →**](docs/engineering.md)


