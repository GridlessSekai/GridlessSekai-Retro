# Getting Logs for Bug Reports
Bugs happen. We have logs for that!

Unsure how to do something? Google it.

# Android
1. Connect your Android phone to a PC (or use Termux without PC - see INSTALL.md)
2. Enable Developer Mode on your Android Phone
3. Enable USB debugging (wireless too if Termux)
4. Install ADB (https://developer.android.com/tools/releases/platform-tools) on your PC and unzip it
5. Navigate to the platform-tools folder and open CMD
6. Close the game on your phone
7. Run `adb logcat -s "OfflineSekaiR"`
8. Launch the game on your phone. Navigate to where the issue is occuring in game
9. Copy the logs printed!

# iOS
1. Connect your iOS device to a PC
2. Trust the PC on your device
3. Install libimobiledevice (windows: https://github.com/jrjr/libimobiledevice-windows, there are other versions you can find on Google) and unzip it
4. Navigate to the suite path and open POWERSHELL
5. Close the game on your phone
6. Run `./idevicesyslog | Select-String -Pattern "OfflineSekaiR"` (use grep for Mac/Linux: `idevicesyslog | grep "OfflineSekaiR"`)
7. Launch the game on your phone. Navigate to where the issue is occuring in game
8. Copy the logs printed!
