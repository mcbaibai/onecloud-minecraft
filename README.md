在玩客云安装我的世界1.14服务端教程
首先你需要你的玩客云刷了armbian否则这个教程不适合你
进入首页，输入
         root@onecloud:~# apt install openjdk17 vim -y
然后去下载个服务端:https://fabricmc.net/use/server/
然后在home创建叫server的文件夹
然后cd /home/server
这里推荐使用1.14，1.20.1容易崩溃
在命令行输入curl -OJ https://meta.fabricmc.net/v2/versions/loader/1.14/0.15.11/1.0.1/server/jar
          root@onecloud:~# curl -OJ https://meta.fabricmc.net/v2/versions/loader/1.14/0.15.11/1.0.1/server/jar
然后在里面创建文件叫start.sh
在里面输入java -Xmx2G -jar fabric-server-mc.1.14-loader.0.15.11-launcher.1.0.1.jar nogui
跟我启动输入
          root@onecloud:~# bash start.sh
如果卡住返回至root@onecloud:~#
在文件夹 里找到eula.txt
在最后面的false改成true然后再启动就成功了
Done!
