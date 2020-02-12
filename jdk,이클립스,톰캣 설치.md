### JDK

```BASH
tar xvf jdk-8u221-linux-x64.tar.gz
mv jdk1.8.0_221 jdk1.8.0
cp -r jdk1.8.0 /etc
cd /usr/bin/
ln -s /etc/jdk1.8.0/bin/java java
ls -l java
```



### 이클립스

```bash
tar xvf eclipse-jee-oxygen-3a-linux-gtk-x86_64.tar.gz
cp -r eclipse /etc
cd /usr/bin/
ln -s /etc/eclipse/eclipse eclipse 
ls -l eclipse
```



### 톰캣

```bash
tar xvf apache-tomcat-9.0.22.tar.gz 
cp -r apache-tomcat-9.0.22 /etc
cd /etc/apache-tomcat-9.0.22/conf/
vi server.xml
포트번호 : 8080 -> 80
firewall-config
http 방화벽 풀기
cd /usr/bin/
ln -s /etc/apache-tomcat-9.0.22/bin/startup.sh starttomcat
ln -s /etc/apache-tomcat-9.0.22/bin/shutdown.sh shutdowntomcat
ls -l starttomcat
ls -l shutdowntomcat 
```

