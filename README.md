# AndroidKiosk
a sample app to demonstrate using the android with kiosk mode Enterprise Mobility Management (EMM)


## ADB Command:
~ To uninstall the app:\
```adb uninstall com.example.kioskandroid```

~ How to setup the device owner:\
```adb shell dpm set-device-owner com.example.dpc/.MyDeviceAdminReceiver```

~ How to remove the device admin owner:\
```adb shell dpm remove-active-admin com.example.dpc/.MyDeviceAdminReceiver```



