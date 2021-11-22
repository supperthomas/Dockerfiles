# Dockerfiles

本项目主要为了让大家更方便的搭建各种编译环境，并且能够快速搭建好编译环境做出的一个小工具。

大家都知道各种git上面的代码，编译环境过于复杂，搭建起来费时费力，而且顺着user guide 经常会出错。

而且环境各种出错。

处于这个痛点，

学习了下docker 觉得docker能够很方便的解决这个痛点。

而且dockerfile的文件很小，可以放到github上面，大家一起维护。

可能要考虑以下几点：

1. 前期境外服务器需要用到的dockerfile，这个可以放到测试环境中进行测试，快速搭建，和修改
2. 如果放到本地机器的话，有些软件包下载过于慢，或者从github下载也很慢。  这个我会放另外一个dockerfile维护
    需要1. 修改软件源为阿里源，
    \2. 需要修改github源为gitee源
3. 另外一种方式是docker pull直接下载做好的镜像。







## DOCKER 测试环境：

境外：



- https://katacoda.com/    这个空间比较大，缺点就是有可能随时断线

- https://labs.play-with-docker.com/    这个空间只有4G，适合小型化的docker， 可以用putty  使用时间4个小时

  
