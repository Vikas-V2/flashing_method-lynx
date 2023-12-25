---
Device name: Google pixel 7a
Device codename: lynx
Device maintainer: Vikas Yaduvanshi 
---

### Declaration ###

---
 I am not responsible for bricked devices, dead SD cards,caused by you following
  these directions. YOU are choosing to make these modifications, and if
 you point your finger at me for messing up your device, .

---

# Method: #1 

---
If you already on superiorOS then follow this Method , IF NOT THEN FOLLOW # Method2
---

1. Download the Recovery flashing zip   from Here [Download](https://sourceforge.net/projects/superioros/files/lynx/gapps/)
2. Boot into Recovery.
3. Go to Apply Update.
4. Sideload the ROM.
5. Wipe data.(*if you want to clean flash this rom *) 
6. Reboot.

 
---
# Method: #2 flash all files manually 
* always use latest platform tools From here [Download]((https://developer.android.com/tools/releases/platform-tools/)


```
boot.img
dtbo.img
vendor_kernel_boot.img
vendor_boot.img
```




*Reboot to bootloader keep in mind bootloader should be unlocked
* connect your devive to pc  then open cmd 
# FLASH the downloaded image files to your device by typing 

```
fastboot flash boot boot.img
fastboot flash dtbo dtbo.img
fastboot flash vendor_kernel_boot vendor_kernel_boot.img
fastboot flash vendor_boot vendor_boot.img

```

## reboot to Crdroid recovery
*  If you are not in recovery, reboot into recovery:
*  in bootloder menu choose boot to recovery option.


once Crdroid recovery up choose Factory Reset option under advanced settings 
 then Format data / factory reset and continue with the formatting process. 
This will remove encryption and delete all files stored in the internal storage, as well as format your cache partition (if you have one).
 Return to the main menu.
 
 ```
Sideload the Crdroid .zip package but do not reboot before you read/followed the rest of the instructions!
On the device, select “Apply Update”, then “Apply from ADB” to begin sideload.
 On the host machine, sideload the package using: adb sideload filename.zip
```
