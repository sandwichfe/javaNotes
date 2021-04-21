### 1.vmware 安装 centos7

打开:http://mirrors.aliyun.com/centos/7/isos/x86_64/       centos7的阿里下载库，在这里我下的是，minimal精简版。

用vmware将centos安装完成后，首先开启网卡，onboot=yes。

如果没有ifconfig命令  就 yum一个。 参考：https://jingyan.baidu.com/article/eb9f7b6d42636d869364e8c9.html



然后xshell连接 vaware : 参考:https://blog.csdn.net/xzy950605/article/details/50929761?utm_medium=distribute.pc_relevant.none-task-blog-2%7Edefault%7EBlogCommendFromMachineLearnPai2%7Edefault-1.control&dist_request_id=&depth_1-utm_source=distribute.pc_relevant.none-task-blog-2%7Edefault%7EBlogCommendFromMachineLearnPai2%7Edefault-1.control

以及  https://blog.csdn.net/qq_33521184/article/details/105489692?utm_medium=distribute.pc_relevant.none-task-blog-baidujs_baidulandingword-0&spm=1001.2101.3001.4242



记得虚拟机自定义ip地址时 要与 外界主机 ip在同一个域也就是在前面三个值要相等，在同一范围。



同时 网关  子网掩码  都要设置好   很重要！！！！！

https://www.cnblogs.com/yhongji/p/9336247.html





阿里云  配置 docker仓库https://developer.aliyun.com/article/521649