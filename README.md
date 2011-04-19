This tests statically registered BroadcastReceiver to see if it can receive broadcast intents without a running process (such as Activity or Service).

To run this program, don't hit the "Run As..." or "Debug As..." button on Eclipse, because this project doesn't have any Activity or Service class.

To test this program, build and enter the following command on the console window of the machine connected to the target device.

# cd <project dir>/bin
# adb install StaticBroadcastReceiver.apk
# adb shell am broadcast -a my.broadcast.intent