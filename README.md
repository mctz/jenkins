# Jenkins 2.332.3
- docker镜像安装：
- 便捷安装：
- linux安装： docker run --name jenkins -p 18080:8080 -v /etc/localtime:/etc/localtime:ro --restart=always registry.cn-hangzhou.aliyuncs.com/masilong/jenkins
- windows安装：docker run --name jenkins -p 18080:8080 -v /etc/localtime:/etc/localtime:ro -v E:/dockerData/jenkins:/var/jenkins_home --restart=always --env JENKINS_HOME=/var/jenkins_home registry.cn-hangzhou.aliyuncs.com/masilong/jenkins


- 完整安装：
docker run --name jenkins -p 18080:8080 -p 50000:50000 -v /etc/localtime:/etc/localtime:ro -v /var/jenkins:/var/jenkins_home -v /usr/java/jdk7:/usr/local/jdk7 -v /opt/apache-maven-3.2.5:/usr/local/maven -v /opt/scripts/:/opt/scripts/ --restart=always --env MAVEN_HOME=/usr/local/maven --env JENKINS_HOME=/var/jenkins_home registry.cn-hangzhou.aliyuncs.com/masilong/jenkins

- 访问地址：http://127.0.0.1:18080/jenkins
