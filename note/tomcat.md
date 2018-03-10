1.配置多站点
	1. server.xml 修改 host/COntext
		http://localhost:8080/test1 跟 http://localhost:8080/test2 来分别访问
	2.使用不同ip/域名访问
		<!-- 新建站点 -->
      <Host name="www.aqiejava.com"  appBase="E:\aqiejava"
            unpackWARs="true" autoDeploy="true">

      </Host>
	3.使用不同端口访问
		配置：service
2.tomcat 相关
	1.站点默认根目录 
		a.D:\Program Files\apache-tomcat-8.5.24\webapps
		b./usr/local/apache-tomcat-9.0.5/webapps
	2.查看tomcat 是否启动
		a.netstat -tunlp|grep 8080
		b.ps -ef |grep tomcat
		c.杀死进程 kill -9 pid
	3. 远程访问 manager/html
		1.https://www.cnblogs.com/davidgu/p/6064731.html
		2./webapps/manager/META-INF/context.xml