# jenkins
- 长期支持版本【V2.164】
- docker镜像安装：
- 便捷安装：
docker run --name jenkins -p 18080:8080 -v /var/jenkins:/var/jenkins_home --restart=always registry.cn-hangzhou.aliyuncs.com/masilong/jenkins

- 完整安装：
docker run --name jenkins -p 18080:8080 -p 50000:50000 -v /var/jenkins:/var/jenkins_home -v /usr/java/jdk7:/usr/local/jdk7 -v /opt/apache-maven-3.2.5:/usr/local/maven -v /opt/scripts/:/opt/scripts/ --restart=always --env MAVEN_HOME=/usr/local/maven --env JENKINS_HOME=/var/jenkins_home registry.cn-hangzhou.aliyuncs.com/masilong/jenkins

- 访问地址：http://127.0.0.1:18080/jenkins
