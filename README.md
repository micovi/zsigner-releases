# zsigner releases

Signed builds of the zsigner companion app, and the update feed the app reads.

The app checks `https://github.com/micovi/zsigner-releases/releases/latest/download/appcast.xml`
for new versions. The feed, its release notes and every archive are signed with the project's
update key (EdDSA, Sparkle); the app refuses anything that does not verify, and installs nothing
without the user's click. The macOS builds are also signed with Developer ID and notarized by
Apple.

This repository holds release files only; there is no source code here.
