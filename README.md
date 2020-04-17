# hello-spring-boot

使用 SpringBoot 提供一个输出 hello 的 controller

使用 MockMvc 测试


1. 添加 SpringBoot parent 依赖

```xml
<parent>
    <groupId>org.springframework.boot</groupId>
    <artifactId>spring-boot-starter-parent</artifactId>
    <version>1.5.8.RELEASE</version>
</parent>
```

2. 添加 spring-boot-starter-web 依赖

```xml
<dependency>
    <groupId>org.springframework.boot</groupId>
    <artifactId>spring-boot-starter-web</artifactId>
</dependency>
```

3. 打包
```shell script
mvn install -Dmaven.test.skip=true
```

4. 启动
```shell script
java -jar target/hello-spring-boot.jar
```

在浏览器 访问 http://127.0.0.1:8080/hello