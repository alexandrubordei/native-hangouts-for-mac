# native-hangouts-for-mac

An unoficial google hangouts app for mac that runs in the mac's dock like a regular app but does not require chrome).
It is built using nativefier which uses electron.

[Download binaries DMG](releases/latest)


To build:
```bash
brew install node
npm install nativefier -g
nativefier -i ./Hangouts_Icon.icns --name "Google Hangouts" "https://hangouts.google.com" -p osx
hdiutil create -volname NativeGoogleHangouts -srcfolder ./Google\ Hangouts-darwin-x64 -ov -format UDZO nativegooglehangouts.dmg
```

Note: Google, Hangouts, nativefier, electron are all registered trademarks and belong to their respective owners.
