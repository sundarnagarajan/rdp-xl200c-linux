# Linux on the RDP XL-200C Mini PC

## Where have we reached?
Apparently the device can boot Linux from my remastered Ubuntu 16.04 and 18.04 ISO
- Wifi does not work (18.04)
- Audio out (18.04) is too loud with a buzzing noise

The OEM vendor has provided a 'driver' for Ubuntu 16.04.

We are currently exploring how to get Wifi (and everything else) working.

## Terminology and short hand
Throughout this repository and in issues and issue responses, I will often use the following terms that are more clearly defined in the table below

| Term | Meaning |
| ---- | ------- |
| My kernel_build repository | [kernel_build](https://github.com/sundarnagarajan/kernel_build) |
| My bootutils repository | [bootutils](https://github.com/sundarnagarajan/bootutils) |
| My RDP Thinbook repository | [rdp-thinbook-linux](https://github.com/sundarnagarajan/rdp-thinbook-linux) |
| Standard Ubuntu ISO | An **unmodified** 64-bit (amd64) Ubuntu ISO download from sites such as the [Official Archive Mirrors for Ubuntu](https://launchpad.net/ubuntu/+archivemirrors) |
| Standard xubuntu ISO | An **unmodified** 64-bit (amd64) ISO from [xubuntu site](https://xubuntu.org/download) |
| Standard Ubuntu Mate ISO | An **unmodified** 64-bit (amd64) ISO from [Ubuntu Mate site](https://ubuntu-mate.org/download/) |
| Remastered Ubuntu ISO | An **unmodified** 64-bit (amd64) Ubuntu ISO download from sites such as the [Official Archive Mirrors for Ubuntu](https://launchpad.net/ubuntu/+archivemirrors) which has been remastered using the ```make_rdp_iso.sh``` script on my [rdp-thinbook-linux](https://github.com/sundarnagarajan/rdp-thinbook-linux) repository |
| Remastered xubuntu ISO | An **unmodified** 64-bit (amd64) ISO from [xubuntu site](https://xubuntu.org/download) which has been remastered using the ```make_rdp_iso.sh``` script on my [rdp-thinbook-linux](https://github.com/sundarnagarajan/rdp-thinbook-linux) repository |
| Remastered Ubuntu Mate ISO | An **unmodified** 64-bit (amd64) ISO from [Ubuntu Mate site](https://ubuntu-mate.org/download/) which has been remastered using the ```make_rdp_iso.sh``` script on my [rdp-thinbook-linux](https://github.com/sundarnagarajan/rdp-thinbook-linux) repository |
| Pre-created Remastered Ubuntu ISO | A remastered Ubuntu ISO from my [rdp-thinbook-linux](https://github.com/sundarnagarajan/rdp-thinbook-linux) repository. Link not here, since link may change |
| Pre-created Remastered xubuntu ISO | A remastered xubuntu ISO from my [rdp-thinbook-linux](https://github.com/sundarnagarajan/rdp-thinbook-linux) repository. Link not here, since link may change |
| Pre-created Remastered Ubuntu Mate ISO | A remastered Ubuntu Mate ISO from my [rdp-thinbook-linux](https://github.com/sundarnagarajan/rdp-thinbook-linux) repository. Link not here, since link may change |

## License, code of conduct, goals and policies
Though this is 'non-technical', please familiarize yourself with the following:
- The [LICENSE (GPLv3)](/LICENSE) used for everything on this repository, unless otherwise explicitly indicated
- [Code of conduct](/CODE_OF_CONDUCT.md)
- Please read the [FAQ](/docs/faq.md) before reporting an issue
- If you are a beginner or are not experienced with operating at the Linux command line, please see: [learning linux](/docs/learning_linux.md)

## Reporting a problem
Raise an issue on github. See the [FAQ](/docs/faq.md) for more details


## About the RDP XL-200C Mini PC
### Links - these worked as of Jul-24-2018
- [RDP XL-200C on www.rdp.in](http://www.rdp.in/thinclients/xl-200c.html)
- [Buy RDP XL-200C on www.rdp.online](https://www.rdp.online/GST%20ready%20Mini%20Desktop)
- [Buy RDP XL-200C on Amazon.in](https://www.amazon.in/RDP-Client-XL-200c-Processor-Storage/dp/B07DKSC5BL)
- [RDP XL-200C specs on www.rdp.in](http://www.rdp.in/techspecs/xl-200c.html)
- [RDP XL-200C Data sheet on www.rdp.in (PDF)](https://rdpdrive.app.box.com/s/1jc0ah5q8c94yoj2erii31e2gmdp8v0r)
### Specs - copied from specs link above

| Parameter | Detail |
| ----- | ----- |
| Model | XL-200C |
| Device Type | Thin Client / Mini PC / VDI Ready |
| CPU | Intel Quad Core Processor up to 1.92 GHz [Intel Atom x5-Z8350 Cherry Trail](https://ark.intel.com/products/93361/Intel-Atom-x5-Z8350-Processor-2M-Cache-up-to-1_92-GHz) |
| RAM | 2GB DDR3L |
| Storage | 32GB eMMC |
| I/O Ports | 1xVGA, 1xHDMI, 1xUSB3.0, 2xUSB2.0, 1xRJ45, 1x TF Card Slot, 1xAudioout |
| Native OS (pre-installed) | Free DOS (probably no OS installed) |
| Supported Local OS | Windows 10 32 bit Home,Windows 10 32 bit Pro & Linux (Ubuntu / Endless OS) |
| Video Resolutions | 16/24/32 bit, Up to 1920X1024 (FHD) |
| Built in Wi-Fi | Yes |
| Audio input/output | Yes |
| Power Consumption | 12.5 watts |
| Dimensions | 25mm(H) x 120mm(W) x 120mm(D) |
| Weight | 220 grams |
| Mounting Option | Desktop / Monitor Back (VESA mount ?) |
