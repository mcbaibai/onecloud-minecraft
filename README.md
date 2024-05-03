在玩客云安装我的世界1.14服务端教程<br>
首先你需要你的玩客云刷了armbian否则这个教程不适合你<br>
进入首页，输入<br>
<h3>apt install openjdk17 vim -y</h3><br>
然后去下载个服务端:https://fabricmc.net/use/server/<br>
然后在<h4>home</h4>创建叫<h4>server</h4>的文件夹<br>
然后cd /home/server<br>
这里推荐使用1.14，1.20.1容易崩溃<br>
在命令行输入<h3>curl -OJ https://meta.fabricmc.net/v2/versions/loader/1.14/0.15.11/1.0.1/server/jar</h3><br>
然后在里面创建文件叫<h4>start.sh></h4><br>
在里面输入<h3>java -Xmx2G -jar fabric-server-mc.1.14-loader.0.15.11-launcher.1.0.1.jar nogui</h3><br>
跟我启动输入<br>
<h3>bash start.sh</h3><br>
如果卡住返回至<h4>root@onecloud</h4><br>
在文件夹 里找到<h4>eula.txt</h4><br>
在最后面的<h4>false</h4>改成<h4>true</h4>然后再启动就成功了<br>
Done!<br>
