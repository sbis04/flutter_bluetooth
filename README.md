# flutter_bluetooth

This flutter app will help you to connect to Bluetooth Devices (like, HC-05). You can send messages to the bluetooth module and perform various operations. By default, the app has only on and off functionality for any paired bluetooth devices, but you can add as many functionality as you want.

This flutter plugin is very new and contains a few bugs (like, while starting the app for first time it will show a dialog box, written, "Allow flutter_bluetooth to access this device's location?" instead of showing "Allow Bluetooth access", but it will perform the operation of getting bluetooth access. So, don't get afraid). This plugin is made by implementing the "flutter_blue" plugin.

Add this dependency in pubspec.yaml:
```yaml
dependencies:
  flutter_bluetooth_serial: ^0.0.4
 ```
 

## Getting Started

This project is a starting point for a Flutter application.

A few resources to get you started if this is your first Flutter project:

- [Lab: Write your first Flutter app](https://flutter.io/docs/get-started/codelab)
- [Cookbook: Useful Flutter samples](https://flutter.io/docs/cookbook)

For help getting started with Flutter, view our 
[online documentation](https://flutter.io/docs), which offers tutorials, 
samples, guidance on mobile development, and a full API reference.
