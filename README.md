# Simple-Termux-Xfce4

​This repository offers a straightforward method for installing and utilizing a lightweight desktop on your smartphone or tablet.

## Installation

To install, execute the following command in Termux:

```bash
curl -sL https://github.com/carwinx05/Simple-Termux-Xfce4/releases/download/script/setup-desktop.sh -o install.sh && bash install.sh
```

## Key Features
- **User-Friendly Setup**: Just run a single command and everything configures automatically, no manual configuration required.
- **Firefox and Synaptic**: Navigate the internet and manage packages/updates on your mobile as if you were on a desktop.
- **Full Desktop Hardware Support**: Connect your hardware to your mobile and use it as a real desktop PC.

## Troubleshooting

### Process Completed (Signal 9) - Press Enter

1. Install LADB from the Play Store or download it from [here](https://github.com/hyperio546/ladb-builds/releases).
2. Connect to Wi-Fi.
3. Enable wireless debugging in Developer Settings and note the port number and pairing code.
4. Enter these values in LADB.
5. Once connected, run the following command:

```bash
adb shell "/system/bin/device_config put activity_manager max_phantom_processes 2147483647"
```

### How aceess my device files?

To access your device's files, simply run the following command in the Termux shell and accept the permission prompt.

```bash
termux-setup-storage
```
