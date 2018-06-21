
mosquitto安装和使用
----------------------------------------------------

mosquitto官网：http://mosquitto.org

# 1.安装Cygwin
    官网下载相应版本： http://www.cygwin.com/

    安装过程：省略

    安装过程中需要注意的地方：
    * 如果是64bits系统，选择源时使用http://mirrors.163.com/cygwin/x86_64
    * 选择安装组件时必须包括：
        binutils 
        gcc (core, g++)
        gcc-mingw (core, g++)
        gdb

# 2.安装mosquitto
    省略

# 3.测试
    cmd进入mosquitto安装目录，
    输入mosquitto -c mosquitto.conf将启动broker

    保持broker启动，另开cmd，启动客户端，
    
    订阅主题：
    mosquitto_sub -v -t topicTest01

    发布主题：
    mosquitto_pub -t topicTest01 -m TestMessage 

    --help可查看命令参数

参考：

https://www.cnblogs.com/yudar/p/4615703.html

https://blog.csdn.net/pgpanda/article/details/51800865

