Solution
--------

1.  Make sure your device is connected to your computer and is set to **USB debugging** mode
2.  Download passwordstorer-signed.apk to your device
  - In a terminal pointing to where the .apk is located, run **adb install passwordstorer-signed.apk**
  - If you get a message saying "adb is not a recognized command", make sure your system's PATH variable is pointing to the Android\sdk\platform-tools folder. Should be somewhere in C:\Users\<username>\AppData\Local\Android\sdk\platform-tools
3.  The app should have been downloaded and installed onto your device.
4.  Open the app in your device. Should be called **TonysPasswordStorer**
5.  Once you open the app and see the "Hello World!" message, we're ready to do a backup.
  - Do this to save the password to your device
6.  On the terminal, run **adb backup man.the.is.tonygreer.tonyspasswordstorer**
  - Follow the instructions "Now unlock your device and confirm the backup operation."
  - On your device, press the **Back up my data** button
    - This may timeout if you take too long, just run the command again
7.  Now you should have a file called **backup.ab** saved to wherever your terminal was pointing to.
8.  To make things easier, copy backup.ab from this folder to the **tools folder** where **abe.bat** is located
9.  Open a new terminal window pointing to the tools folder where abe.bat is located
10. Run the command **abe backup.ab backup.tar**
11. Inside the tools folder, you should see a new file called **backup.tar**
12. Open backup.tar and go to **apps->man.the.is.tonygreer.tonyspasswordstorer->sp**
13. You should see a file called **default.xml**
14. Open default.xml with any text editor and you should see the password!
  - \<string name="password">**traincarbuttwagon**\</string>
