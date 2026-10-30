# Android-RAT

Requirements
Python 3
apktool
zipalign
apksigner
msfvenom
Metasploit Framework
Linux recommended (tested on Debian 12)
Signing Keys
A folder named .android must exist in the root of your project (or in your home directory as ~/.android) containing the debug keystore file (debug.keystore) so APK signing works out-of-the-box.

If you don't have one, you can generate it using:

keytool -genkey -v -keystore ~/.android/debug.keystore -storepass android -alias androiddebugkey -keypass android -keyalg RSA -keysize 2048 -validity 10000
How to use
Clone this repository




Ensure the .android directory exists in your project root (or your home directory) with the debug keystore inside.

Start the tool

python3 cli.py
Follow the on-screen menu:


```==============================
   AndroidRAT Main Menu
==============================
[1] Build Android Payload (APK)
[2] Start Metasploit Listener
[3] Sign APK
[4] Patch APK for Visible UI
[5] Show Help & Exit

