# Reproducing the Prototype

[Overview](../README.md)

This checkout contains the report and five photographs, with code embedded in the report appendix. It has no runnable entry point, dependency manifest or complete face-recognition module, so a clone-and-run command would be misleading.

## Files needed to restore a runnable project

1. Original Python application files, including `Face_Recog` and enrollment utilities.
2. The tested Raspberry Pi OS/Python versions and dependency versions.
3. A reviewed wiring/pin diagram, power requirements and peripheral configuration.
4. A sample vote-state file and reset procedure using demonstration identities.
5. Tests for identity rejection, repeated voting, candidate input, result access and alert behaviour.

The report's code helps recover the structure, but copying a formatted PDF appendix is not equivalent to recovering tested source. Restore and verify the original files before adding installation instructions.

## Useful portfolio additions

A short video can show the fingerprint prompt, candidate selection, confirmation, repeat-vote handling and results display in sequence. Label simulated or incomplete steps. If source files are recovered, add a setup guide and record hardware tests before describing the project as reproducible.
