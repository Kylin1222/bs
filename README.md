# bs
Network Countermeasures Technology Training Platform  
## biaoqian.html是初始页面  
## 开启服务命令  
### Windows开启noVNC：
    node websockify.js路径 --web noVNC-master路径 9000 localhost:5900
#### 浏览器连接网址：http://172.16.227.131:9000(win10) http://172.16.227.128:9000(win7)
### kali开启noVNC：
    x11vnc -display :0 -autoport -localhost -nopw -bg -xkb -ncache -ncache_cr -quiet -forever
	ss -antp | grep vnc
	/usr/share/novnc/utils/novnc_proxy --listen 8081 --vnc localhost:5900
#### 浏览器连接网址：http://172.16.227.130:8081/vnc.html（kali ip）
### kali开启shellinabox
	sudo /etc/init.d/shellinabox start
#### 浏览器连接网址：https://172.16.227.130:4200  
### 实验手册显示：  
电脑需安装nodejs  
  
	cd webserver
	node index.js
