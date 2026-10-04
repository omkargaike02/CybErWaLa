# CybErWaLa

Grab cam shots and live GPS location from a target's phone camera or PC webcam just by sending a link.

![CybErWaLa]

## What is CybErWaLa?

CybErWaLa is a social engineering tool that hosts a convincing fake webpage on a local PHP server and exposes it to the internet using ngrok or CloudFlare Tunnel. When the generated link is opened by a target and camera/location permission is granted, the tool captures a snapshot from the device camera and/or the device's GPS location.

## Features

- Multiple ready-made webpage templates to keep the target engaged long enough to capture a shot:
  - Festival Wishing
  - Live YouTube TV
  - Online Meeting [Beta]
- GPS Location Tracking with Google Maps integration
- Built-in cleanup script to wipe captured files and logs in one command

## Tested On

- Kali Linux
- Termux
- MacOS
- Ubuntu
- Parrot Sec OS
- Windows (WSL)

## Requirements

\`\`\`
apt-get -y install php wget unzip
\`\`\`

## Installation


git clone https://github.com/omkargaike02/CybErWaLa

cd CybErWaLa

bash cyberwala.sh


## Cleanup

bash cleanup.sh


This removes all captured camera files, saved locations, and log files.

## Change Log

**v2.0** — Added GPS location tracking with Google Maps integration and accuracy reporting

**v1.9** — Improved architecture detection (ARM, ARM64, x86, x86_64, Apple Silicon)

**v1.8** — Added CloudFlare Tunnel support, removed deprecated Serveo

**v1.7** — Fixed Termux home directory detection, added Apple Silicon / Raspberry Pi support

**v1.6** — Fixed ngrok direct link generation

## Disclaimer

CybErWaLa is built strictly for authorized penetration testing and security awareness/education. The author is not responsible for any misuse or illegal use of this tool. Use it only on systems and people you have explicit permission to test.

---

### Author
**Omkar Gaike**
GitHub: https://github.com/omkargaike02

---
<sub>Built on the GPL-3.0 licensed CamPhish engine by TechChip — license requires this notice to remain. Original project: https://github.com/techchipnet/CamPhish</sub>
