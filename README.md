# Lolipa

### 环境说明

* Java 8
* Gradle 3.0
* MySQL 5.7
* npm 3.10.3
* Node 6.5.0

编译通过

其他环境暂未测试

### 编译部署

1.环境配置

修改 application.properties 与 env.properties

2.安装依赖并编译

执行
```
gradle build
```

运行
```
java -jar Lolipa.jar
```

3.导入数据库结构 database.sql

4.前端构建

在 view 目录执行

```
npm install
```

```
npm run build
```

将 dist 目录下的文件放到 nginx 所指定的项目目录

5.配置 nginx

nginx.conf 为默认配置文件，请根据自己的环境修改为适合的配置

### 其他配置

后台地址 /admin

默认用户名 Admin

默认密码 admin