# raspbian

开启SSH：
      在TF卡的跟目录（boost）下创建ssh文件

设置WiFi连接：
      1、创建名为wpa_supplicant.conf的文件
      2、添加内容如下
      country=CN
        ctrl_interface=DIR=/var/run/wpa_supplicant GROUP=netdev
        update_config=1
        network={
          ssid="WiFi名"
          psk="密码"
          priority=10
        }
