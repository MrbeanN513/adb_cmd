# adb_cmd
1. recived call ==== adb shell input keyevent KEYCODE_CALL
2. make a call ===== adb shell am start -a android.intent.action.CALL -d tel:8777564598
3. send a sms ====== adb shell am start -a android.intent.action.SENDTO -d sms:8777564598 --es sms_body HELLO --ez exit_on_sent true && adb shell input keyevent 22 && adb shell input keyevent 22 && adb shell input keyevent 66
4. end a call ==== adb shell input keyevent KEYCODE_ENDCALL
5. send notification ===== adb shell "cmd notification post -S bigtext -t 'you are hacked' 'Tag' 'hahahahahhahahahahahhah'"
6. list all notification === adb shell dumpsys notification | egrep NotificationRecord | awk -F\| '{print $2}'


