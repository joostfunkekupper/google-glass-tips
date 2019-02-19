# Google Glass Tips

## ADB Tips
Since Glass doesn't allow you to easily manage your apps via the UI, you will rely heavily on ADB to manage the installed apps.

### View connected devices
`adb devices -l`

### View installed apps
`adb shell pm list packages`

### Uninstall an app
`adb uninstall <package name>`

## Screen mirroring
1. Download [Android Screen Mirror](https://code.google.com/archive/p/android-screen-monitor/) java jar.
2. Unzip in desired directory.
3. Connect the device and ensure debugging is enabled, see [here](http://neatocode.tumblr.com/post/49566072064/mirroring-google-glass).
3. Run `java -jar asm.jar`
4. ...
5. Profit

### Download files from device
`adb pull <device name>:<directory>` for example `adb pull glass-2:/sdcard/DCIM/Camera`
