# 리눅스 jdk 재설치



### jdk 버전 확인

```bash
java -version
```



### 기존 링크파일 삭제

```bash
rm /usr/bin/java
```



### tar 파일 풀기

```bash
tar xvf jdk-8u221-linux-x64.tar.gz
```

> 파일 이름 변경
>
> ```bash
> mv jdk1.8.0_221 jdk1.8.0
> ```



### jdk 파일 복사

```bash
cp -r jdk1.8.0 /etc
```



### 심볼릭 링크 파일 만들기

```bash
[root@server2 bin]# -> 경로 : /usr/bin
ln -s /etc/jdk1.8.0/bin/java java
```



### 확인

```bash
ls -l java
```

