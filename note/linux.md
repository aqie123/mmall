一：linxu
	1.rpm -qa | grep jdk
	2.
	3.
二：安装jdk
	a.删除之前jdk : rpm -qa|grep jdk
	b. yum remove
	1. yum -y install lrzsz 	上传文件 rz
	2.解压到指定文件 tar -zxvf ./text.tar.gz -C /home/app/test/
	3.vim /etc/profile
	4.	export JAVA_HOME=/usr/local/jdk-9.0.4
		export PATH=$JAVA_HOME/bin:$PATH 
	5. source /etc/profile

三：tomcat (http://blog.csdn.net/machao0903/article/details/78500816)
	1.wget -c http://mirrors.hust.edu.cn/apache/tomcat/tomcat-9/v9.0.5/bin/apache-tomcat-9.0.5.tar.gz
	2. tar -zxvf apache-tomcat-9.0.5.tar.gz -C /usr/local/
	4.
	5.

四：nginx
	1.用处
		1.直接支持Rails 和 php程序
		2.作为HTTP反向代理服务器
		3.负载均衡服务器
		4.邮件代理服务器
		5.帮助前端实现动静分离
	2.特点
		1.高稳定
		2.高性能
		3.资源占用少
		4.功能丰富
		5.模块化结构
		6.支持热部署
	3.常用命令
		1.查看进程命令 ps -ef|grep nginx
		2.平滑重启 kill -HUP pid
		3. 启动 nginx
		4. 重启 nginx -s reload
	4.指向端口
	5.指向目录
五：mysql

六：maven
	1.下载：wget http://mirrors.shu.edu.cn/apache/maven/maven-3/3.5.2/binaries/apache-maven-3.5.2-bin.tar.gz
	2. 解压：tar -zxvf apache-maven-3.5.2-bin.tar.gz -C /usr/local/
	3. 建立连接 ln -s /usr/local/apache-maven-3.5.2/ maven
	4. 设置环境变量 
		1.export M3_HOME=/usr/local/apache-maven-3.5.2
		2.export PATH=${M3_HOME}/bin:${PATH}

七：基本使用
	1. 查看磁盘空间 df -h
	2.创建新用户
		1. adduser
		2. passwd
	3.centos7 虚拟机 http://192.168.144.128:8080/
	4. rpm -ivh 安装
八：centos 添加源
	1. cd /etc/yum.repos.d
	2. yum makecache
九：查看端口 及防火墙
	1.查看端口 ： netstat -ntlp
	2.linux : lsof -i:81    / 		netstat -tunlp|grep 80
十：安装git
	1.
十一：防火墙
	1. iptables -L -n --line-number
	2. iptables -D INPUT 7
十二：建立软连接
	1. 在 /home/aqie 下
	2. 正确删除 rm -rf  ./test_chk_ln   