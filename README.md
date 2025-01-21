#Connect phone in android studio  
  1. First, conect your phone to the pc.
  2. In your phone, allow USB debuging.
  3. Type "adb devices", on the android studio terminal. It will show you the device conected.
  4. After, type "adb tcpip 5555".
  5. Look in your phone, in Wi-fi option, the number of the wifi's ip.
  6. With the ip: adb connect 192.168.12.16:5555
End

#To consume local endpoint:
  1. It's necessary run this command: "adb reverse tcp:2242 tcp:2242". In this case, 2242 is the API port. If you are using a diferent one, change it.
  2. Ensure to use the complet path in your string. In the URI, don't forget to put "http://".

#To publish the project
  1. Ensure your project are up to date: "flutter upgrade" and "flutter pub upgrade"
  2. To generate the archive to deploy a project, you must execute "flutter build appbundle --release"  
