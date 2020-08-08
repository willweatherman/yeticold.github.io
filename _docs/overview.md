---
title: About Yeticold
description: Yeticold is a step-by-step protocol for long-term storage of
  Bitcoins, in an offline and secure way.
redirect_from:
  - /docs/
---

Yeticold is a step-by-step protocol for storing bitcoins in a highly secure
manner. It is intended for:

* **Personal storage**: Yeticold does not address institutional security
needs such as internal controls, transparent auditing, and preventing access
to funds by a single individual.
* **Large amounts of money ($100,000+)**: Yeticold thoroughly considers corner
cases such as obscure vectors for malware infection, personal estate
planning, human error resulting in loss of funds, and so on.
Even if your Bitcoin holdings are more modest, it's worth considering using
Yeticold. If Bitcoin proves successful as a global currency, it will appreciate
10x (or much more) in the coming years. Security will become increasingly
important if your holdings appreciate and Bitcoin becomes a more attractive
target for thieves.
The "Protocol Overview" section also describes some lower-security, lower-cost
approaches to self-managed storage that may be more appropriate for smaller
amounts of funds.
* **Long-term storage**: Yeticold not only considers the Bitcoin security
landscape today, but also a future world where Bitcoin is much more valuable
and attracts many more security threats.
* **Infrequently-accessed funds**: Accessing highly secure bitcoins is
cumbersome and introduces security risk through the possibility of human
error, so it is best done infrequently.
* **Technically unskilled users**: Although the Yeticold protocol is long, it is
clear and straightforward to follow. No technical expertise is required.

The Yeticold protocol covers bitcoin storage, not procurement. It assumes you
already possess bitcoins and wish to store them more securely.

If you are already familiar with Bitcoin security concepts and are certain that
you want high security cold storage, you may prefer to read
[Trusting This Protocol](#trusting-this-protocol) and then skip to the section
[Choosing a Multisignature Withdrawal Policy](/docs/overview/multi-signature-security#choosing-a-multisignature-withdrawal-policy).

## Trusting this protocol

Funds secured using Yeticold can only be as secure as its design.
Here's what you can trust about this protocol:
* **Open source**: Yeticold software, is open
source. The code is straightforward and well-commented to facilitate easy review
for flaws or vulnerabilities. [View it on Github](https://github.com/JWWeatherman/yeticold).

If you like, you may review the [design document](/docs/design-doc/overview)
for details on the technical design.

## Background

### Self-Managed Storage vs. Online

Let's start by assessing whether Yeticold is right for you.

There is no such thing as perfect security. There are only degrees of security,
and those degrees come at a cost (in time, money, convenience, etc.) So the
first question is: How much security are you willing to invest in?
For most people, most of the time, the authors recommend storing Bitcoin using YetiWarm which is a single laptop setup allowing much more ease of access. The pros and cons of the various yeti software branches can be found in the [design document](/docs/design-doc/overview).

### Yeticold vs. Hardware Wallets

Many people who choose
self-managed storage (as opposed to an online storage service) use "hardware
wallets" such as the
[Trezor](https://trezor.io/),
[Ledger](https://www.ledgerwallet.com/),
and [KeepKey](https://www.keepkey.com/)
to store their bitcoins. These can be almost as unsecure as the online storage sercives due to specialized hardware.

The primary security consideration is that all hardware wallets today operate inside of specialized hardware. 
This specialized hardware is manufactured in known locations with employes working on the supliy lines.
This allows for easy human error and the ability to insert malware before it ever goes online.

For details on this and other security considerations, see the
"No Hardware Wallets" section of the [design document](/docs/design-doc/overview)
As with online multisig
vaults, many people do use hardware wallets to store sizeable amounts of
money. We personally recommend Yeticold for all investments, but ultimately
it's a personal decision based on your risk tolerance and costs you're
willing to pay (in money and time) for security.
