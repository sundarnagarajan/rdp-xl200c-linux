This file contains a variety of links from the Internet that may have some bearing on getting Linux to run on the RDP XL-200C with all hardware working

Avoid removing a link - just add new links (with an informative description) to the **END**


1. [Firmware search paths - from Linux kernel documentation](https://www.kernel.org/doc/html/v4.17/driver-api/firmware/fw_search_path.html)
2. [WiFi on linux-sunxi](https://linux-sunxi.org/Wifi)
3. [Broadcom brcmsmac(PCIe) and brcmfmac(SDIO/USB) drivers - from wireless.wiki.kernel.org](https://wireless.wiki.kernel.org/en/users/drivers/brcm80211)
4. [Broadcom Bluetooth firmware for Linux kernel - github repo by Azamat H. Hackimov (winterheart)](https://github.com/winterheart/broadcom-bt-firmware)
5. [Google search for ```brcm_patchram_plus```](https://www.google.com/search?q=brcm_patchram_plus&oq=brcm_patchram_plus)
6. [Discussion on ```what to do with brcm_patchram_plus``` on spinics.net](https://www.spinics.net/lists/linux-bluetooth/msg70830.html)
7. [Discussion on ubuntuforums.org on getting WiFi working on a Kangaroo mini PC](https://ubuntuforums.org/showthread.php?t=2329846). This starts on Jul-05-2016, and thread ends Aug-05-2016. It gives a good idea of the type of interaction between relatively less experienced device owners and relatively more experienced people on the Internet who want to help. This thread may also be expliclitly useful for the RDP XL-200C, since the thread includes many discussions on getting the right Broadcom firmwar and installing it in the right palce.
8. [Another discussion on ubuntuforums.org about getting Wifi to work on the Asus f205ta](https://ubuntuforums.org/showthread.php?t=2290874). The Asus f205ta [seems to be a Bay Trail laptop](http://www.driversfree.org/en/news/review-and-specs-of-asus-f205ta-budget-notebook-with-a-11-6-inch-display), and owner is finally successful
9. [wireless-info script](https://raw.githubusercontent.com/UbuntuForums/wireless-info/master/wireless-info) to help in gathering information to troubleshoot a wireless connection.
10. Ubuntuforums.org guide on [```How to install a driver for the Broadcom series of PCI wireless cards```](https://ubuntuforums.org/showthread.php?t=2214110). Probably of limited relevance, because the RDP XL-200C Wifi card is probably an SDIO card and not a PCI card
11. [github repo on preparing ISO for Asus-F205TA](https://github.com/Mechazawa/Arch-Linux-Asus-F205TA). It's all about creating ```bootia32.efi```, so it seems to indicate the Asus F20tTA is a Bay Trail laptop with a 32-bit UEFI loader
12. [gentoo discussion on getting Wifi to work on Raspberri Pi 3](https://forums.gentoo.org/viewtopic-p-7949030.html?sid=18a9accf5456dbb752e962749758ce65). This is significant, because the names of the firmware files used to make Wifi finally work are **the same** as the names of the firmware files supplied by the OEM vendor of the RDP XL-200C
