# Project Deep Clean
#### Originally for Samsung Galaxy S8 G950FD AQL5 
##### And probably other variants as well as future TW releases.

------------


Since Samsungs TouchWiz ROM is extremely bloated with features. Project Deep Clean is aimed to provide a comprehensive removable list with descriptions so that we can completely remove useless ~~features~~ and files that we don't need without breaking the functionalities that we actually want to use.

## Disclaimer
*This is **not** noob-friendly.* I do expect things to break so that you can tell us what's wrong and we will improve this script together.

This script can break things in an unexpected, possibly horrible way. Please do a **full backup** of your current setup before attempting. If anything goes terribly wrong, I won't laugh at you but you will be on your own.
If that disclaimer doesn't scare you, let's proceed.

> Qui Audet Adipiscitur

## Usage
**Debloat script:**
- Comment out anything you do NOT want to remove from the script using #
- Save the script
- Grab a flashable zip and repalce the updater-script inside
- Flash and voilà

**Rescue Zip:**
If you need anything back to the system, a rescue flashable zip is provided for you to put anything you need inside the system folder and flash.

If your system failed to boot and you want to see what happened, you will need to add these lines to build.prop and flash for you to logcat during boot:

```shell
ro.secure=0
ro.debuggable=1
persist.service.adb.enable=1
persist.sys.usb.config=mtp,adb
ro.adb.secure=0
```

## Feedback
I need your input so that this list can be as complete as possible. If anything other than the removed ones breaks unexpectedly, please check/provide `logcat | grep <some app>`so that we can find out what's wrong. You can do so via [XDA thread](https://forum.xda-developers.com/galaxy-s8/samsung-galaxy-s8--s8-cross-device-development/zip-project-deep-clean-actually-t3743184 "XDA thread") or submit commits or fork this source and submit a pull request.

## Credit
- [SoLdieR9312](https://forum.xda-developers.com/member.php?u=4860093 "SoLdieR9312") for his OREO BETA6 Debloat script template.
- [foobar66](https://forum.xda-developers.com/member.php?u=3463514 "foobar66") for his debloat shell script as a reference.
- Google as well as several posts in XDA Developers forum
