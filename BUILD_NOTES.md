# Build/Packaging Notes

This package is the phone-friendly PWA release candidate source. It is deliberately offline-first. The browser build itself does not contain fake billing, fake ads, or fake account servers.

For a Google Play release, package the hosted PWA as an Android App Bundle using a production web-to-Android wrapper. Do not publish an unhosted local HTML file: the final PWA must be served from HTTPS so the service worker, installability and Trusted Web Activity workflow work correctly.

For iOS, the same web codebase can later be wrapped/distributed through an appropriate iOS app wrapper, but App Store submission requires Apple's developer account and review process.


## Android release target
Minimum supported Android version: Android 13 (API 33). Target/compile SDK: Android 16 (API 36).
