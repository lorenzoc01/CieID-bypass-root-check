# CieID - Bypass Root Check
Lucky Patcher custom patch to bypass the root check in CieID android app.

## Usage
1. Insert the txt file inside `/storage/emulated/0/Android/data/[luckypatcher package name]/files/LuckyPatcher/CustomPatches`
2. In LuckyPatcher, apply the custom patch to CieID app (or "Create Modified APK File" with the patch applied and install the rebuilt apk)

## Compatibility
The patch was tested on version `1.7.25` of the app. It could work in future versions too, but that's not guaranteed.

## Explanation
The patch replaces a byte in the classes.dex file, forcing an if condition to be false and bypassing the code responsible for the root check.
