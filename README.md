# CMStorm-Backlight-MacOS
Backlight enable/disable instructions and script for Mac OS X High Sierra or older.

  1. Download the led-backlight-osx file from this repo and place it on your Application folder
  2. Launch the OS X "Automator" program
  3. Choose "Service" document type
  4. Under "Library", click "Utilities", and drag "Run Shell Script" to the blank area / workflow pane.
  5. For "selected service receives" choose "no input" in "any application" (important)
  6. For "pass input" choose "as arguments" (important)
  7. For "shell" choose "/bin/bash"
  8. Paste in this script:
    /Applications/led-backlight-osx
  9. Click "run" to test. After 3 seconds, your keyboard should remain in a state with num lock and scroll lock enabled, and all the keys should be lit up.
  10. Click "File" > "Save", "Save service as" : "CMStorm ON"
  11. Go to System Preferences > Keyboard > Shortcuts > Services > General > "CMStorm ON"
  12. Assign a shortcut.s
  13. Do make a disable script, repeat the process and in step 8 replace the script with the following:
    /Applications/led-backlight-osx off\

Thanks to pykler for the script: https://github.com/pykler/led-backlight-osx

Reference: http://community.coolermaster.com/topic/11765-cm-storm-devastator-support-guide/

This instructions have been produced for people like me that didn't find any working instructions. I found that this is the best way to solve the backlight problem on Mac OS X.
