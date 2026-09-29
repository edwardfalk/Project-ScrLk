# Architecture

The thesis ([Examensarbete-Projekt-ScrLk.pdf](../Examensarbete-Projekt-ScrLk.pdf), in Swedish) points here for an illustrated, up-to-date version of its system overview. That overview now lives in the [README](../README.md), with photos, the system diagram and the full pinout. This page maps the thesis chapters to it.

| Thesis | Where it is now |
| --- | --- |
| 3 System overview | [How it works](../README.md#how-it-works): the system diagram |
| 4.1 Analog board, CRT and safety | [Hardware](../README.md#hardware) |
| 4.2–4.3 Molex connector, level shifter, power | [Connecting the Pi to the analog board](../README.md#connecting-the-pi-to-the-analog-board) |
| 4.4 DPI/KMS and timing | [Driving the CRT from a Raspberry Pi 5](../README.md#driving-the-crt-from-a-raspberry-pi-5), with the oscilloscope capture |
| 4.5–4.6 Ring generator, Ericofon | [The Ericofon](../README.md#the-ericofon) |
| 4.7 ADB keyboard | [The keyboard](../README.md#the-keyboard) |
| 5 Software | [The OS](../README.md#the-os) and [Underneath](../README.md#underneath) |
| 7.2–7.3 Lessons, improvements | [Things that went wrong](../README.md#things-that-went-wrong) and [Known issues and next steps](../README.md#known-issues-and-next-steps) |
| Appendix A, parts list | [Parts](../README.md#parts) |
| Appendix B, DPI overlay | [macintosh-timings](https://github.com/edwardfalk/macintosh-timings) |
| Appendix E, photos and video | Photos are in the README. Video from the build is being collected and will be added here. |

## What has changed since the thesis

- **The two Macs.** The thesis says the Classic's case got the Classic II's insides. It was the other way round: the working Classic's CRT and analog board moved into the less worn Classic II case, which is the badge on the front.
- **The USB over-current warnings.** The thesis blames an undersized level shifter. The best guess now is the power path: the Pi 5 draws its peaks from the analog board's 12 V rail through a small DC-DC module. See [Known issues](../README.md#known-issues-and-next-steps).
