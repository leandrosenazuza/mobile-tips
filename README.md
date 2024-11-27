#Connect phone in android studio  
  1. First, conect your phone to the pc.
  2. In your phone, allow USB debuging.
  3. Type "adb devices", on the android studio terminal. It will show you the device conected.
  4. After, type "adb tcpip 5555".
  5. Look in your phone, in Wi-fi option, the number of the wifi's ip.
  6. With the ip: adb connect 192.168.12.16:5555
End
