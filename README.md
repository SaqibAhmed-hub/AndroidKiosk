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

~ To uninstall the app:\
```adb uninstall com.example.kioskandroid```



