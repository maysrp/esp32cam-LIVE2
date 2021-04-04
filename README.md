# esp32cam-LIVE2
ESP32cam 局域网视频监控  带web配网


ESP32-cam刷入micropython固件   

固件地址：https://github.com/lemariva/micropython-camera-driver

使用Thonny打开你的ESP32-CAM 
联网  
```
import network
sta_if = network.WLAN(network.STA_IF)
sta_if.active(True)
sta_if.connect("wifi名称","wifi密码")

sta_if.ifconfig()


import upip

upip.install("picoweb")

upip.install("micropython-ulogging")

```
将main.py 上传到你的ESP32CAM上。

按住RST按钮重启esp32cam 手机搜索camera_1的热点 默认密码为12345678  


192.168.4.1/set 设置  
193.
设置完成后请务必按RST按钮重启
