# AndroidKiosk
a sample app to demonstrate using the android with kiosk mode Enterprise Mobility Management (EMM).

## Lock Task Mode:
Lock Task Mode https://developer.android.com/work/dpc/dedicated-devices/lock-task-mode


## ADB Command:(Android Debug Bridge)
~ Show the adb version:\
```adb --version```

~ Show the list of devices:\
```adb devices -l```

~ How to restart the adb:\
```adb kill-server``` <br />
```adb start-server```

~ How to setup the device owner:\
```adb shell dpm set-device-owner com.example.dpc/.receiver.MyDeviceAdminReceiver```

~ How to remove the device admin owner:\
```adb shell dpm remove-active-admin com.example.dpc/.receiver.MyDeviceAdminReceiver```

~ To install the app:\
```adb install app/build/outputs/apk/debug/app-debug.apk```

~ To uninstall the app:\
```adb uninstall com.example.kioskandroid```

<b>Note </b> If you want to keep the attribute android:testOnly as true you can use pm install command with -t option,
but you may need to push the apk to device first.
```
$ adb push app/build/outputs/apk/debug/app-debug.apk /tmp/
5210 KB/s (825660 bytes in 0.154s)

$ adb shell pm install /tmp/app-debug.apk 
    pkg: /tmp/hello.apk
Failure [INSTALL_FAILED_TEST_ONLY]

$ adb shell pm install -t /tmp/app-debug.apk 
    pkg: /tmp/hello.apk
Success
```


##Emulator Command:
~ Shows the list of emulators:\
 ```emulator -list-avds```

~ run the emulators: \
 ```emulator -avd Pixel_4_API_32```









