# learn-docker
# [自己动手写docker](https://item.jd.com/12109237.html)　学习笔记
## 间杂几篇博客
- [A Practical Introduction to Container Terminology](https://developers.redhat.com/blog/2018/02/22/container-terminology-practical-introduction/)
## 目录
- 前言
	
- 第一章 容器与开发语言
	- Docker
	- Golang

- 第二章 基础技术
    - Linux Namespace
  		- 概念
  		- UTS Namespace
  		- IPC Namespace
  		- PID Namespace
  		- Mount Namespace
  		- User Namespace
  		- Network Namespace	
  		
  		- [Docker基础技术：Linux Namespace（上）](https://coolshell.cn/articles/17010.html)	
        - [Docker基础技术：Linux Namespace（下）](https://coolshell.cn/articles/17029.html)
        		  
	- Linux Cgroups
  		- 什么是Linux Cgroups
  		- Docker是如何使用Cgroups的
  		- 用go语言实现通过cgroup限制容器的资源
  		
  		- [DOCKER基础技术：LINUX CGROUP](https://coolshell.cn/articles/17049.html)

  	- Union File System
  		- 什么是Union File System
  		- Docker是如何使用Union File System的
  		- 自己动手写Union File System 例子
  		
  		- [DOCKER基础技术：AUFS](https://coolshell.cn/articles/17061.html)
        - [DOCKER基础技术：DEVICEMAPPER](https://coolshell.cn/articles/17200.html)
- 第三章  构造容器
	-  构造实现run命令版本的容器
		- Linux proc 文件系统介绍
		- 实现 run 命令
	- 使用Cgroups 限制容器资源使用
		- 定义Cgroups的数据结构
		- 在启动容器的时候增加资源限制的配置 
	- 增加管道以及环境变量识别
		- 管道
		- PATH识别	
		
- 第四章 构造镜像 
	- 使用busybox创建容器
		- busybox
		- pivot_root
	- 使用 AUFS 包装busybox
	- 实现volume数据卷
	- 实现简单镜像打包
	
- 第五章 构建容器进阶
	- 实现容器的后台运行
	- 实现查看运行中容器
	- 实现查看容器日志
	- 实现进入容器Namespace
	- 实现停止容器
	- 实现删除容器
	- 实现通过容器制作镜像
	- 实现容器指定环境变量运行

- 第六章 容器网络
	- 容器虚拟化网络基础技术介绍
	- 构建容器网络模型
	- 容器地址分配
	- 创建Bridge网络
 	- 在Bridge网络创建容器
 	- 容器跨主机网络

- 第七章 高级实践	
	- 使用mydocker创建一个可访问nginx容器
	- 使用mydocker 创建一个flask + redis的计数器
	- runC介绍
	- runC创建容器流程
	- containerd介绍
	- kunernets CRI 容器引擎
