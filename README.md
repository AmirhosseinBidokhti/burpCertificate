# burpCertificate
System-level trusted BurpSuite Certificate for Android 7+

https://blog.ropnop.com/configuring-burp-suite-with-android-nougat/

```
# Remount and copy cert to device
adb root
adb remount
adb push 9a5ba575.0 /sdcard/
adb shell
vbox86p:/ # mv /sdcard/9a5ba575.0 /system/etc/security/cacerts/
vbox86p:/ # chmod 644 /system/etc/security/cacerts/9a5ba575.0
vbox86p:/ # reboot
```
