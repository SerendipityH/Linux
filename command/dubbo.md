1.从官网下载源码
https://github.com/alibaba/dubbo 

2.解压
tar -zxvf dubbo-master.tar.gz

3.打包生成war包
cd dubbo-master
mvn install -DskipTests
然后(这边要确保maven安装了)
cd dubbo-admin
mvn package -Dmaven.skip.test=true

接下来ls看一下发现有
dubbo-admin-2.5.10.war

4.复制到Tomcat的webapps目录下
cp dubbo-admin-2.5.10.war /usr/local/apache-tomcat-8.5.37/webapps

5.进入解压war包
jar -xvf dubbo-admin-2.5.10.war


![...]{https://github.com/SerendipityH/Linux/blob/master/command/photo/dubbo.jpg}






问题：
现在git上已经没有dubbo-admin 需要切换下分支，嘤嘤嘤
