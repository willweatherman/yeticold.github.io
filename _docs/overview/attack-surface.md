---
title: Attack surface and failure points
description: Learn about the attack surface for Yeticold, the
  step-by-step protocol for storing bitcoins in a highly secure way
---

This list describes the attack surface and other failure points for Yeticold. We
include only attacks and failures limited in scope to specific coins.
Attacks and failures related to the Bitcoin ecosystem as a whole (newly
discovered cryptographic flaws, critical Bitcoin protocol security or
scalability failures, etc.) are not included as most are equally likely to
impact the value of all Bitcoins whether or not they are secured with Yeticold.

Most attacks require the presence of malware, either in or near the quarantined environment. We'll therefore inventory two layers of Yeticold's attack surface:

* Ways in which a malware infection might occur
* Ways in which a critical failure might happen (possibly, but not necessarily, due to a malware infection)

## Malware infection vectors

* Software
  * OS/App software has malware (i.e. malicious code) built into official distributions. In particular, Yeticold relies on the following packages and their dependencies NOT to distribute malicious code:
    * Ubuntu LTS
    * Bitcoin Core
    * libzbar0: (via pip3 Python Package Manager)
    * opencv-python: (via pip3 Python Package Manager)
    * qrtools: (via pip3 Python Package Manager)
    * qrcode: (via pip3 Python Package Manager)
    * pyzbar: (via pip3 Python Package Manager)
    * pillow: (via pip3 Python Package Manager)
    * zbar-py: (via pip3 Python Package Manager)
  
  * Most of the above packages are used to create the QR code system Yeticold uses and can be refactored to rely on fewer packages.

## Failure scenarios

### Physical failures

* Three seed packets are stolen by an attacker
* Five (of the seven) seed packets are lost or destroyed
* An attacker with physical line-of-sight to the laptop takes a photo of the screen while sensitive data is displayed
* Wifi chip in the USB drives sends seed words to attacker.

### Yeticold protocol failures
* Yeticold hosting (i.e. DNS, Github, website hosting, etc.) is compromised
to inject weaknesses into the protocol documentation or Yeticold software
* Protocol delivery is compromised (e.g. with
a man-in-the-middle attack on the user's network) to deliver
or display a weakened version of the protocol documentation or
software
* Human error during protocol execution
* Design failure in the protocol misses or inadequately addresses a risk
