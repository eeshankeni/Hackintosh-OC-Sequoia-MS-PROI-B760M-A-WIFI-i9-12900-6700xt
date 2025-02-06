# Hackintosh-Sequoia-MSI-B760M-i9-12900-6700XT

And EFI to help you get Opencore 1.0.3 running. Tested on Sequoia 15.2。

## Hardware Specs

| Accessory         | Model                                   |
| ----------------- | --------------------------------------- |
| CPU               | Intel® Core™ i9-12900                   |
| GPU               | ROG Strix AMD Radeon RX7000XT           |
| Motherboard       | MSI PRO B760M-A WIFI                    |
| RAM               | 16GB*4 DDR4 3600 Corsair                |
| HDD               | WD 2TB NVME                             |
| Wi-Fi & Bluetooth | Intel® Wi-Fi6E AX211                    |

## What does NOT work?
- Bluetooth, Airdrop
- iMessage
- Realtek ALC897 Audio Stopped working with Alcid=13 after updating from Sonoma to Sequoia.

### Tips
- ctrsmt bootarg added to recognise the E cores as additional threads.
- Use [beta itlwm kext](https://github.com/Lorys89/itlwm/releases/tag/v2.4.0-alpha) and [this thread](https://github.com/OpenIntelWireless/itlwm/issues/983) to find the Heliport app.
- If you get a blank screen post kernel right before installation, Disable NootRX and enable it once in userland post account creation.
- Follow this [helpful guide](https://chriswayg.gitbook.io/opencore-visual-beginners-guide/advanced-topics/using-alder-lake).
