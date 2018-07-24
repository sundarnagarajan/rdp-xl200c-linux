Collecting information here.

## EFI questions
### Does the device support non-EFI (MBR) boot?

### When booting in EFI mode, does the device support booting a **standard** (unmodified, 64-bit amd64)  Ubuntu ISO?

## Wifi questions
### Does WiFi work when using Ubuntu 16.04 - without using any OEM-provided 'driver'?

### Does Wifi work when booting a **standard** (unmodified, 64-bit amd64) Ubuntu ISO after installing the OEM-provided 'driver'?

### Does Wifi work when booting a **pre-created remastered standard** Ubuntu ISO after installing the OEM-provided 'driver'?

#### If the OEM-provided driver does not work at all, can you run ```/etc/rc.local``` manually after installing the OEM-provided ```driver```?
#### What were the errors?
#### What is the output of ```dmesg``` command
#### What is the output of ```journalctl -k``` command

### What is the exact meaning of 'Wifi does not work'?
#### Are Wifi interfaces detected and shown in the desktop GUI?
#### What is the output of the config ```sudo ifconfig -a```?
#### If Wifi interfaces are detected and shown, can you try to connect using Wifi? Are local access points shown?
#### Does the connection appear to 'succeed'?
#### Is the connection unstable, or does the connection drop after a while?

### Answer [Wifi questions above](/docs/initial_analysis.md#wifi-questions) for Ubuntu 18.04 also
