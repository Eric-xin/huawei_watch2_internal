# wearos-converter -- 转换你的 wearos 到国际版

## 第一步：解锁bootloader
把手表adb调试打开
输入adb命令adb shell
手表提示调试点确定
输入`adb reboot bootloader`手表将进入bootloader
进入后输入
`fastboot oem unlock`
长按上面的表冠确认（ps：长按确认 短按选择）
注意 解除bl锁将清空手表数据
之后等手表重启重新配置之后，记得再开发者里重新开启adb调试 /doge

## 第二：刷入rec
重新输入adb reboot bootloader进入bootloader
输入
`fastboot boot X:\xxxx\recovery.img`
刷入rec 待手表重启后
就到了我们熟悉的twrp界面#haha
点击第一个按钮进入twrp
**ps：手表重启后rec将会被还原，如果想再次进入twrp必须重新刷一遍#(流汗滑稽)#(流汗滑稽)#(流汗滑稽)**

##第三：安装wearos-converter
先`adb pull WAY/TO/YOUR/FILE/wearos-converter.zip /sdcard`
在sd卡根目录找到我们刚刚导入的wearos-converter.zip卡刷 
**注意卡刷完成后不要双清，直接点重启进入系统**

---------------------------------------------------------------------------

## Step 1: Unlock bootloader

Turn on the watch ADB debugging

Enter the ADB command ADB shell

Watch prompt debugging point determination

Enter 'ADB reboot bootloader' to enter the bootloader

Enter after entering

`fastboot oem unlock`

Long press the crown to confirm (PS: long press to confirm, short press to select)

Note that releasing BL lock will clear watch data

After that, after the watch is restarted and reconfigured, remember to restart ADB debugging in the developer setting



## Second, Flash in REC

Re enter ADB reboot bootloader to enter the bootloader

input

`fastboot boot X:\xxxx\ recovery.img `

Brush in rec and wait for the watch to restart

We are now familiar with the twrp interface

Click the first button to enter twrp

**PS: after the watch is restarted, REC will be restored. If you want to enter twrp again, you must brush it again (funny) **



## Third: install the wearos converter

First ` ADB pull way / to / your / file / wearos- converter.zip /sdcard`

Find the wearos- we just imported in the SD Kagan directory. converter.zip and FLASH