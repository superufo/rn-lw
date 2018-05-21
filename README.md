# rn-lw
reactnative 

forward:  PC->Phone 作为Client客户端,可以任意访问Phone上的 Server 服务器  adb forward tcp:8888 tcp:8888
reverse:反向代理  Phone->PC   adb reverse tcp:8097 tcp:8097  adb reverse tcp:8081 tcp:8081

npm install -g react-devtools
react-devtools

android avd  命令无效，可以重启，使得环境变量彻底生效
adb devices

React-native bundle --platform Android --dev false --entry-file index.
.js --bundle-output android/app/src/main/assets/index.android.bundle --assets-dest android/app/src/main/res

打开模拟器
emulator.exe -netdelay none -netspeed full -avd api23
打开模拟机dev
adb shell input keyevent 82   ( http://192.168.1.60:8097/ )

8081端口的服务就是React Native项目的一个本地服务器，用于提供JSBundle包和一些静态资源
