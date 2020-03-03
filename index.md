---
# Feel free to add content and custom Front Matter to this file.
# To modify the layout, see https://jekyllrb.com/docs/themes/#overriding-theme-defaults

layout: content
title: About
---

## Q: What is it?

A: A tool to prove that a file existed before a particular time.

* FreeTSA.org service and OpenTimestamps.org calendars made easily available to any end-user
* Cross-platform Linux/Mac/Win
* Entirely based on free sw, strong cryptography, open standards

## Q: Wait... But, Why Timestamping?

A: Because attesting that a file existed before a particular time can be useful to.

* prove when an agreement was signed, if it is disputed
* validate a signature after a revocation occurred
* prove the ownership for copyright
* grant record Integrity

## Q: Wait... But, Why Also on the Blockchain?

A: A classical timestamp provided by a trusted third party - like FreeTSA.org - is very precise (it proves the existence at a particular second), it replies instantly and is a legal standard.

However it can be validated for a limited time (usually no more than 20 years), for technical and economic reasons.

On the other hand, a Blockchain attestation - like that of an OpenTimestamps.org calendar - relies on the Bitcoin’s blockchain, a resilient distributed system, designed to survive perpetually, secured by the thermodynamic value of more than 50 TWh per year (~ 3 bln of $).

However it is less precise (it proves the existence at a particular day), requires time to be confirmed, and is not yet a legal standard.

For all these reasons TimeBags uses both - to have all the benefits of both.

## Q: Ok, Where Is The Package?

A: Well... it's still in Alpha version.

But if you are a python developer and you are interested to contribute, the repo is [here](https://github.com/TimeBags/timebags).

## Q: How Is It Made?

A: Combining a bunch of components.

* [freeTSA.org](https://freetsa.org) service and [rfc3161ng](https://github.com/trbs/rfc3161ng/) library
* [opentimestamps.org](https://opentimestamps.org) calendars service and CLI (modified to be used as a library)
* [ASiC-S](https://www.etsi.org/deliver/etsi_ts/102900_102999/102918/01.03.01_60/ts_102918v010301p.pdf) open standard defined by ETSI and based simply on zip archives
* [PyQt5](https://www.riverbankcomputing.com/software/pyqt/intro) cross-platform GUI library
* [fman](https://build-system.fman.io/) build system

