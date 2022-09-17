# 声明：

一切基于Yunzai-bot更改，本人不负责更新、回答问题，Yunzai-Bot及本修改版属于开源项目，禁止贩卖！！！

####想使用docker版Yunzai-Botv2版本的请参考https://github.com/Le-niao/Yunzai-Bot/issues/80

```
Yunzai-bot原版：

https://github.com/Le-niao/Yunzai-Bot

https://gitee.com/Le-niao/Yunzai-Bot

```

##

#### 安装docker

已经安装docker的直接跳过，但是注意确保已经安装docker-compose

```
不知道有没有安装可以直接输入下面指令，看看有没有反应
docker-compose --help
软路由openwrt系统可以直接在软件包查看，没有就直接安装
```

# Linux
使用一键脚本安装（荐）
```
curl -fsSL get.docker.com -o get-docker.sh
sudo sh get-docker.sh --mirror Aliyun
```
# Windows 和 Mac

请参考以下文档进行安装：

Docker一从入门到实践：https://yeasy.gitbook.io/docker_practice/install/windows

官方文档 https://docs.docker.com/desktop/windows/install/

官方文档 https://docs.docker.com/desktop/mac/install/

##

# 配置文件

#下载文件
要运行Yunzai-bot文件夹输入以下指令进行clone
```
国内机器:git clone https://gitee.com/hbj2457/Yunzai-Bot.git
国外机器:git clone https://github.com/hbj2457/Yunzai-Bot.git
```

##

# 启动

```
# 先cd Yunzai-Bot文件夹
cd Yunzai-Bot

# -------------------------
# 启动容器
docker-compose up -d

# -------------------------
#容器名字查看(注意是数字和英文的组合)
docker ps -a

# -------------------------
# 启动完成后进入 yunzai-bot 的容器(把yunzai-bot替换成你的容器名字)
docker exec -it yunzai-bot /bin/sh

# -------------------------
# 在容器内部运行项目，进行登录验证
node app

# -------------------------
# 验证完成后，按快捷键 Ctrl+D 退出容器，然后重启容器
docker-compose restart

# -------------------------
#查看最后的100行日志并持续输出日志
docker-compose logs -f --tail=100
```
##

# 注意事项：

Linux快捷键：

Ctrl+D是退出容器

Ctrl+C是结束进程

关闭ssh(终端)窗口不会结束docker容器的进程，所以确保是正常运行后可以直接关掉ssh(终端)窗口

可以正常使用后请先在QQ给Yunzai—bot发送“#更新”，以此保持最新版本

##

# 安装指令插件以及插件依赖

#### 指令安装(需要依赖请用这个方法)

进入 yunzai-bot 的容器(把yunzai-bot替换成你的容器名字)


```
docker exec -it yunzai-bot /bin/sh

```

然后就可以用指令安装插件和插件依赖了

#### 安装普通js插件

回到下载要运行时候的文件夹

直接丢Yunzai-Bot\plugins\example文件夹就行

（注意：确保是适用于V3版本的js插件）

##

# 插件

## 插件索引：

https://gitee.com/yhArcadia/Yunzai-Bot-plugins-index

## 插件推荐：

Miao-Plugin(https://gitee.com/yoimiya-kokomi/miao-plugin)

xiaoyao-cvs-plugin(https://gitee.com/Ctrlcvs/xiaoyao-cvs-plugin)

suiyue(https://gitee.com/Acceleratorsky/suiyue)

py-plugin(https://gitee.com/realhuhu/py-plugin)

Guoba-Yunzai / Guoba-Plugin(https://gitee.com/guoba-yunzai/guoba-plugin)
