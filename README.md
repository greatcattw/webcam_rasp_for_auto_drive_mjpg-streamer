# webcam_rasp_for_auto_drive
Making a webcam for toy card auto drive by rasp3B with low_latency  
用樹莓3B建立webam, 用於玩具車的自動駕駛. 具有低延時,低CPU負載.  

樹莓硬體為  
rasp3B  

樹莓作業系統為  
2022-04-04-raspios-buster-armhf.img  
9d2d2db345e9e7d511bad6493031b8f3  

USB攝影機為  
Logi C270  

影像預設的尺寸為1280x720  


這個版本使用JPEG格式,找到這個版本是個意外.  
相較YUV & MJPG,對樹莓CPU的負載較低.  
原因待查.  

## 安裝
一鍵安裝的版本  
下載後放到U盤,插上樹莓,執行
set_as_ap.sh  
安裝後重啟樹莓  

## 測試  
使用其它電腦/手機的WiFi掃瞄,可以看到webcam這個AP  
無帳密登入,取得IP為192.168.100.x
使用瀏覽器
192.168.100.1:8080/?action=snapshot
可以看到攝影機的影像

# In progress