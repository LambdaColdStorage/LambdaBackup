LambdaBackup
============

A Backup Tool for Google Glass (for Mac OS X)

Creates lifestreams like this:

<img src="http://www.stephenbalaban.com/wp-content/uploads/2013/06/out.gif" />

The secret is that the entire app is a shell script wrapped as an app.

Tools used:

- Platypus – for wrapping the shell script up as an app.
- `CocoaDialog` – bash bindings for Cocoa.
- `adb` – for moving files back and forth between the Glass without having to implement a PTP client, this is why we need the Glass to be in debug mode.
- ImageMagick (`convert`) – for creating the optional GIF image stream at the end.
- GNU `parallel` – for downsizing the images in parallel using ImageMagick.
