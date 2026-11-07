# WiFiEverywhere

A small jailbreak preference bundle with one switch labelled **WiFi Everywhere**.

## Compatibility

The project is configured with an iOS 5.0 deployment target and armv7/arm64 build architectures. Actual support depends on the installed Theos toolchain, jailbreak, and device architecture; it has not yet been tested across every iOS release.

## Build

On a Mac or Linux system with Theos installed:

```sh
make package
```

The resulting Debian package is written to the Theos packages output directory.

## Current behaviour

The switch saves a Boolean preference named `enabled` in the `com.macwithgentoo.wifieverywhere` preferences domain. It does not change Wi-Fi connectivity or restart/crash SpringBoard yet.
