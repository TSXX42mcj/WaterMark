右键管理员身份运行cmd

adb devices
显示已连接设备

adb shell
进入adb命令行

mount -o remount -o rw /
  使用这条命令可以临时挂载上/system文件夹，直到下一次重启。
  
不能挂载/system且提示“’/dev/root’ is read-only”：

重新运行cmd

adb root
adb disable-verity
adb remount

adb push setup.conf /system/etc/
把setup.conf 文件push到 /system/etc/

adb reboot
重启
