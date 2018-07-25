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

### Are the broadcom drivers in the (recent) kernels that we use?
[This link from wireless.wiki.kernel.org](https://wireless.wiki.kernel.org/en/users/drivers/brcm80211) says that brcmsmac is for PCIe and brcmfmac is for SDIO/USB.

On the most recent kernel (4.17.9):

```grep BRCM /boot/config-4.17.9```
gives
```
CONFIG_NET_DSA_TAG_BRCM=y
CONFIG_NET_DSA_TAG_BRCM_PREPEND=y
CONFIG_BRCMUTIL=m
CONFIG_BRCMSMAC=m
CONFIG_BRCMFMAC=m
CONFIG_BRCMFMAC_PROTO_BCDC=y
CONFIG_BRCMFMAC_PROTO_MSGBUF=y
CONFIG_BRCMFMAC_SDIO=y
CONFIG_BRCMFMAC_USB=y
CONFIG_BRCMFMAC_PCIE=y
CONFIG_BRCM_TRACING=y
# CONFIG_BRCMDBG is not set
```

In particular, see:

**CONFIG_BRCMSMAC=m**

**CONFIG_BRCMFMAC=m**


The file ```/lib/firmware/brcm/brcmfmac43430-sdio.txt``` is not in /lib/firmware in the standard Ubuntu distribution, nor is it part of the [linux firmware git repo](https://git.kernel.org/pub/scm/linux/kernel/git/firmware/linux-firmware.git). So this is an initial clue.
