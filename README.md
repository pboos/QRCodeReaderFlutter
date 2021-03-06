# QRCode Reader plugin for Flutter

> This is a copy of [qrcode_reader](https://pub.dartlang.org/packages/qrcode_reader) with build fix 

> The original repo is archived so publishing as a new plugin

Flutter plugin for reading QR Codes with the camera.

### Example

``` dart
import 'package:qrcode_reader/QRCodeReader.dart';
```

``` dart
Future<String> futureString = new QRCodeReader()
               .setAutoFocusIntervalInMs(200) // default 5000
               .setForceAutoFocus(true) // default false
               .setTorchEnabled(true) // default false
               .setHandlePermissions(true) // default true
               .setExecuteAfterPermissionGranted(true) // default true
               .scan();
```

These options are Android only, this is the simplest way of plugin usage:
``` dart
Future<String> futureString = new QRCodeReader().scan();
```