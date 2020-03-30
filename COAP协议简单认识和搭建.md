# COAP协议简单认识和搭建

---

**本篇目标：简单了解coap协议的用途和尝试搭建coap客户端和服务器（基于libcoap）**

**材料准备：**

- linux系统：这里用虚拟机搭建的ubuntu系统
- libcoap库：可以从GitHub下载，或者Linux直接拉取
- 测试环境：火狐浏览器55.0版本与copper插件

****

## coap协议简单介绍



---

## 安装测试环境

测试coap协议的通讯需要安装特定的插件copper，安装环境是火狐浏览器55.0版本，高于该版本插件就不可使用，请确认自己火狐浏览器的版本为55.0版本。

1. 安装火狐浏览器55.0版本

2. 关闭火狐浏览器自动更新功能（选项-高级-更新-不检查更新），若浏览器不小心自动更新成新的版本了，直接用55.0的安装包覆盖安装即可

3. 将copper插件copy到目标文件夹下，路径为：

   C:\Users\username\AppData\Roaming\Mozilla\Firefox\Profiles\1fdcksre.default\

4. 打开火狐浏览器，可以看到右上角有一个图标：![1549809978762](C:\Users\jinhao_tuya\AppData\Roaming\Typora\typora-user-images\1549809978762.png)

5. 点开复制地址coap://californium.eclipse.org/到浏览器并访问，可以看到出现了插件的界面如下：

![1549810198238](C:\Users\jinhao_tuya\AppData\Roaming\Typora\typora-user-images\1549810198238.png)

6. 点击Discover按钮，可以获取到如上图左侧的coap接口，点击create1接口，再点击GET，会发现有数据返回，这就是通过coap协议向服务器请求的数据，浏览器本身为一个客户端用来测试。

---

## 安装libcoap库

可以直接通过git命令获取到libcoap或者复制下载好的库到Ubuntu下：

1. 获取libcoap：git clone  https://github.com/authmillenon/libcoap.git

2. 进入libcoap目录，进行安装：

   (1)autoconf

   (2)./configure

   (3)make

   (4)sudo make install

3. 这样就安装完成了，安装完成后会在example生成两个可执行文件coap-server和coap-client



---

## 搭建coap客户端



---

## 搭建coap服务器



---

