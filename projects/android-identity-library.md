# Project Name
Android Identity Library.

# Project Description
Libraries and reference applications for working with real-world identity.

The initial focus for this work was mdoc/mDL according to [ISO/IEC 18013-5:2021](https://www.iso.org/standard/69084.html)
and related standards (mainly ISO 23220 series and ISO 18013-7) on Android. Current focus
includes other credential formats and operating environments.

## Libraries

The project includes two libraries written in Java and Kotlin. The
first is `identity` which provides the core building blocks and which
can also be used on server-side environments. The other is `identity-android`
which provides Android-specific extensions to the former. It is designed to
run on Android (API 24 or later) and will take advantage of  Android-specific
features including hardware-backed Keystore, NFC, Bluetooth
Low Energy, and so on.

The libraries are intended to be used by Wallet Applications (mobile
applications on the credential holder's device), Reader Applications (applications
operated on device controlled by the verifier), and Issuance Systems (applications
operated by the credential issuer or their agent). They provide the following
building blocks

- A light-weight _Secure Area_ abstraction for hardware-backed keystore
    - Applications can create hardware-backed Elliptic Curve Cryptography
      keys which can be used for creating Signatures or performing Key Agreement.
      Each key will have an attestation which can be used to prove to Relying Parties
      (such as a credential issuer) that the private part of the key only exists
      in a Secure Area.
    - The `identity-android` library includes an implementation based on
      [Android Keystore](https://developer.android.com/training/articles/keystore)
      with support for requiring user authentication (biometric or lock-screen knowledge
      factor, e.g. system PIN) for unlocking the key and also can use
      [StrongBox](https://source.android.com/docs/compatibility/13/android-13-cdd#9112_strongbox)
      if available on the device. This is appropriate to use in Android applications
      implementing ISO/IEC 18013-5:2021 for storing `DeviceKey`.
    - The `identity` library includes an implementation backed by BouncyCastle
      with support for passphrase-protected keys. This isn't suitable for use
      in Mobile Applications as its not backed by Secure Hardware.
    - Applications can supply their own _Secure Area_ implementations for e.g.
      externally attached dongles, cloud based HSMs, or whatever the issuer
      deems appropriate to protect key material associated with their credential.
- A _Credential Store_ for storage of one or more _Credentials_
    - Each Credential has a _Credential Key_ which can be used by the issuer
      to bind a credential to a specific device which is useful when
      issuing updates or refreshing a credential.
    - Additionally, each Credential has one or more _Authentication Keys_ which
      can be endorsed by the issuer and used at presentation time.
    - Finally, namespaced data and arbitrary key/value pairs can be stored
      in a _Credential_ which can be used for credential data and claims. This
      data is stored encrypted at rest.
- Data structures and code for provisioning of mdoc/mDLs
    - This code can can be used both on the device and issuer side. No networking
      protocol is defined, the application has to define its own.
- Parsers and generators for all data structures used in ISO/IEC 18013-5:2021
  presentations, including `DeviceResponse`, `DeviceRequest`,  `MobileSecurityObject`
  and many other CBOR data structures.
- An implementation of the ISO/IEC 18013-5:2021 presentation flows including
  QR engagement, NFC engagement (both static and negotiated), device retrieval
  (BLE, Wifi Aware, and NFC)

## Wallet and Reader Android applications

This repository also contains two Android applications using this library
in the `appholder` and `appverifier` modules. The Wallet application is a simple
self-contained application which allows  creating a number of mdoc credentials
using four different mdoc Document Types:

- `org.iso.18013.5.1.mDL`: Mobile Driving License
- `org.micov.1`: mdoc for eHealth ([link](https://github.com/18013-5/micov))
- `nl.rdw.mekb.1`: mdoc for Vehicle Registration ([link](https://github.com/18013-5/mVR))
- `eu.europa.ec.eudiw.pid.1`: mdoc for Personal Identification

and their associated mdoc name spaces. The first one is defined in
ISO/IEC 18013-5:2021 and the other three have been used at mdoc/mDL
test events organized by participants of the ISO/IEC JTC1 SC17 WG10
working group.

## ISO 18013-7 Reader Website

The `wwwverifier` module contains the source code for a website acting as an
mdoc reader according to the latest ISO 18013-7 working draft (as of Sep 2023)
and it's implementing  the so-called REST API. There is currently a test instance
of this application available at https://mdoc-reader-external.uc.r.appspot.com/.
The Wallet Android  application also has support for the REST API and registers
on Android for the `mdoc://` URI scheme. This can be tested end-to-end by going
to the reader  website (URL above) and clicking on one of the "Request" buttons,
and then  hitting the `mdoc://` link presented on the site. This will cause the
browser  to invoke the Wallet app which will then connect to the reader and send
the credential after user consent.

# Alignment with the OpenWallet Foundation Mission

The project is already open-source and operating as such. It implements an important
standard for digital wallets on a widely used mobile platform and is already
in use in production applications, including Google Wallet.

# Current Code of Conduct

The project is currently using the [Google Code of Conduct](https://github.com/google/identity-credential/blob/master/docs/code-of-conduct.md).

# TAC Sponsor
--

# Project License
Apache 2.0

# Source Control
https://github.com/google/identity-credential

# Issue Tracker
https://github.com/google/identity-credential/issues

# External Dependencies
--

# Release Methodology
Releases are made on Google Maven.

# Initial Maintainers
David Zeuthen.

# Proposed Project Governance
--

# Links to Documented Governance Practices
--

# Preferred Maturity Level
--

# Communication Channels
--

# Project Website
--

# Social Media
--

# Financial Sponsorship
--

# Infrastructure
--
