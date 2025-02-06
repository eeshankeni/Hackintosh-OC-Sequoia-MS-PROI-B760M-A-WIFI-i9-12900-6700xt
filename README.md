# Hackintosh-Sequoia-MSI-B760M-i9-12900-6700XT
And EFI to help you get Opencore 1.0.3 running. Tested on Sequoia 15.2。

![Screenshot 2025-02-06 at 7 38 11 AM](https://github.com/user-attachments/assets/b4a4e803-e9fd-4ac8-8e52-671089661d38)


## Specs

| Accessory         | Model                                   |
| ----------------- | --------------------------------------- |
| CPU               | Intel® Core™ i9-12900                   |
| GPU               | ROG Strix AMD Radeon RX6700XT           |
| Motherboard       | MSI PRO B760M-A WIFI                    |
| RAM               | 16GB*4 DDR4 3600 Corsair                |
| HDD               | WD 2TB NVME                             |
| Audio             | Realtek ALC897 (alcid=13)               |
| Wi-Fi & Bluetooth | Intel® Wi-Fi6E AX211                    |

## What does NOT work?
- Bluetooth, Airdrop
- iMessage, Facetime

## Whats special?
- USB ports mapped via usbtoolbox.
- CPU topology rebuild and CPU Friend should provide decent alder lake thread management.
- Debugging disabled by default. Enabled with -v bootarg

### Tips
- ctrsmt bootarg added to recognise the E cores as additional threads. Disable if it helps.
- Use [beta itlwm kext](https://github.com/Lorys89/itlwm/releases/tag/v2.4.0-alpha) and [this thread](https://github.com/OpenIntelWireless/itlwm/issues/983) to find the Heliport app.
- I've used alcid=13 for Realtek, try other ids for 897 if it fails.
- If you get a blank screen post kernel right before installation, Disable NootRX and enable it once in userland post account creation.
- Follow this [helpful guide](https://chriswayg.gitbook.io/opencore-visual-beginners-guide/advanced-topics/using-alder-lake).
- Enable Above 4G decoding, disable ftpm, disable secure boot.
