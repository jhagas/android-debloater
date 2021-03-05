# android-debloater
Semi-Automated NON-ROOT android debloater script build in BASH. What is it mean semi-automated? 
This is a very dangerous task to do and can broke your phone, semi-automated means that this script helps you a lot but you still have a control over what do you want to do. 
This script can also automatically install an APK Inspector to your phone, so you can carefully get the apps package name in your phone then remove it!

> Check out my other android-linux integration CLI script, [wireless-scrcpy](https://github.com/jhagas/wireless-scrcpy) and [gsconnect-cli](https://github.com/jhagas/gsconnect-cli)

## :penguin: Download
For download, just copy these commands into your terminal and press ENTER
```bash
git clone https://github.com/jhagas/android-debloater
mkdir ~/.local/bin/
chmod 777 ~/android-debloater/android-debloater
cp ~/android-debloater/android-debloater ~/.local/bin/
```

## Usage
TO RESTORE, YOU NEED TO DO A FACTORY RESET, 
SO DO THIS CAREFULLY OR YOUR PHONE WILL BROKEN!!

1. Find an app to Uninstall 
```bash
android-debloater find [APP-NAME]
```
for example
```bash
android-debloater find whatsapp
```
You shall get an output tike this
```bash
com.whatsapp
```

2. Uninstall Bloat Apps
```bash
android-debloater remove [APP-PACKAGE-NAME]
```
It remove the apps,  [APP-PACKAGE-NAME] must be precisely typed in order to remove it. For example
```bash
android-debloater remove whatsapp
```
If Whatsapp successfully removed, you will get an output like this
```bash
Success
```

3. Install Helper to your phone
```bash
android-debloater install-helper
```
It install 'App Inspector' app to your phone, so you can easily get the package name of the bloat. And you don't have to instally manually from Google play store.

## Support App Inspector in Google Play Store
App Inspector by Projectoria : https://play.google.com/store/apps/details?id=bg.projectoria.appinspector
