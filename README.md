# adb_cmd
1. recived call ==== adb shell input keyevent KEYCODE_CALL
2. make a call ===== adb shell am start -a android.intent.action.CALL -d tel:8777564598
3. send a sms ====== adb shell am start -a android.intent.action.SENDTO -d sms:8777564598 --es sms_body HELLO --ez exit_on_sent true && adb shell input keyevent 22 && adb shell input keyevent 22 && adb shell input keyevent 66

