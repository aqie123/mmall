一：web 容器
	1.nginx  80
	2.tomcat 8080
	3.apache 80
二：Nginx
	1. 启动 D:\Program Files\nginx-1.13.8>nginx -c conf/nginx.conf
	2. 验证 nginx -t
	3. 重载配置 nginx -s reload
	4. 细节 autoindex off   403
三：Tomcat
	1.启动 net start tomcat9
四：info
	1.img.forward.com 实现转发目录
	2.tomcat.forward.com 转发tomcat服务器
五：Mysql

六: 项目初始化
	1.maven archetype 创建web空项目
	2.Mybatis
		1.Mybatis-generator : 自动生成数据库交互代码
		2.Mybatis-plugin :mybatis接口实现和xml自动跳转
		3.Mybatis-pagehelper : 分页插件
	3.tomcat web.xml
	4.spring applicationContext.xml
	5.SpringMVC dispatcher-servlet.xml
	6.日志管理 Logback 初始化
	7.IDEA
		1.开启Problem，实时编译
		2.IDE 使用mybatis及Spring scan时，autowried注入时报错处理
七：website
	1.http://learning.happymmall.com/
	2.img.forward.com  nginx
八：思维导图
	1.http://www.imooc.com/article/20193#child_3_3
	2.www.happymmall.com
	3.
九：使用intellij idea搭建MAVEN+SSM(Spring+SpringMVC+MyBatis)框架
	1.https://www.cnblogs.com/jingpeipei/p/6291071.html
	2.123456@
十：腾讯云
	1.140.143.238.151

	2.	线上前台地址：http://www.happymmall.com
		线上后台地址：http://admin.happymmall.com
十一：maven
	1.清除命令 ： mvn clean
	2.编译命令 ：mvn compile
	3.打包命令：mvn package
	4.跳过单元测试：mvn clean package -Dmaven.test.skip=true
十二：软件环境配置
	1.http://learning.happymmall.com/env.html
	2.
十三：windows 查看端口
	1.netstat -ano
	2.netstat -aon|findstr "8080"  端口号
	3.tasklist|findstr "2720"       pid

