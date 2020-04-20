# Flutter Bluetooth 
[![Codemagic build status](https://api.codemagic.io/apps/5e675f714ce63c22e5aeb47f/5e675f714ce63c22e5aeb47e/status_badge.svg)](https://codemagic.io/apps/5e675f714ce63c22e5aeb47f/5e675f714ce63c22e5aeb47e/latest_build) 

### *NOTE:* This is the updated version of the app (using flutter_bluetooth_serial 0.2.2). This version has much fewer bugs and provides a lot of functionality.

This flutter app will help you to connect to Bluetooth Devices (like, HC-05). You can send messages to the bluetooth module and perform various operations. By default, the app has only **on and off functionality** for any paired bluetooth devices, but you can add as many functionality as you want.

Initially, you will have to give **location permission** to the app. As for discovering as well as for connecting to the paired devices, location permission is required as Bluetooth transmission shares some location data.  

<p align="center">
  <img width="300" src="https://github.com/sbis04/flutter_bluetooth/blob/master/screenshots/bluetooth_device_location.png">
</p>

Add this dependency in pubspec.yaml:
```yaml
dependencies:
  flutter_bluetooth_serial: ^0.2.2
 ```
 
## How to run the app
You should have flutter installed and up running properly to use this application.
To check if there is any problem, use the command:
```bash
flutter doctor
```
Now, navigate to the project folder and run this command:
```bash
flutter run
```
If you get any error like this : 
<p align="center">
  <img width=max src="https://github.com/sbis04/flutter_bluetooth/blob/master/screenshots/error_screenshot.png">
</p>
Then navigate to your project folder (like, flutter_bluetooth) after opening the project folder follow these steps:
android -> app -> src -> main -> AndroidManifest.xml

Now, add these two lines of code :

```xml
<manifest ......
          
    <!-- this line -->
    xmlns:tools="http://schemas.android.com/tools">

    <!-- and this line -->
    <uses-sdk tools:overrideLibrary="io.github.edufolly.flutterbluetoothserial"/>
    ...
</manifest>
```


# Screenshots
<p align="center">
  <img width="250" src="https://github.com/sbis04/flutter_bluetooth/blob/master/screenshots/bluetooth_turn_on.png">
  <img width="250" src="https://github.com/sbis04/flutter_bluetooth/blob/master/screenshots/connecting.png">
  <img width="250" src="https://github.com/sbis04/flutter_bluetooth/blob/master/screenshots/device_connected.png">
</p>

<p align="center">
  <img width="250" src="https://github.com/sbis04/flutter_bluetooth/blob/master/screenshots/device_on.png">
  <img width="250" src="https://github.com/sbis04/flutter_bluetooth/blob/master/screenshots/device_off.png">
  <img width="250" src="https://github.com/sbis04/flutter_bluetooth/blob/master/screenshots/device_disconnected.png">
</p>

# License

Copyright (c) 2019 Souvik Biswas

Permission is hereby granted, free of charge, to any person obtaining a copy
of this software and associated documentation files (the "Software"), to deal
in the Software without restriction, including without limitation the rights
to use, copy, modify, merge, publish, distribute, sublicense, and/or sell
copies of the Software, and to permit persons to whom the Software is
furnished to do so, subject to the following conditions:

The above copyright notice and this permission notice shall be included in all
copies or substantial portions of the Software.

THE SOFTWARE IS PROVIDED "AS IS", WITHOUT WARRANTY OF ANY KIND, EXPRESS OR
IMPLIED, INCLUDING BUT NOT LIMITED TO THE WARRANTIES OF MERCHANTABILITY,
FITNESS FOR A PARTICULAR PURPOSE AND NONINFRINGEMENT. IN NO EVENT SHALL THE
AUTHORS OR COPYRIGHT HOLDERS BE LIABLE FOR ANY CLAIM, DAMAGES OR OTHER
LIABILITY, WHETHER IN AN ACTION OF CONTRACT, TORT OR OTHERWISE, ARISING FROM,
OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER DEALINGS IN THE
SOFTWARE.
