# swagger的使用

swagger在前后端联调开发中，启动非常重要的作用，如下：

1. 保持接口和文档的一致性
2. 使注释更为丰富



1、框架依赖中已包含swagger接口组件。
```xml
<dependency>
    <groupId>io.springfox</groupId>
    <artifactId>springfox-swagger2</artifactId>
    <version>2.7.0</version>
</dependency>
<dependency>
    <groupId>io.springfox</groupId>
    <artifactId>springfox-swagger-ui</artifactId>
    <version>2.7.0</version>
</dependency>
```

## 网页地址

你可以通过http://localhost:8080/swagger-ui.html这个地址获得接口信息。

## 生产环境、测试环境、开发环境配置

在生产环境中需要把swagger去掉，请参考配置类Swagger2Config中的@Profile({"dev", "test"})注解。（当前配置表示加载在dev和test文件使用,只在开发环境和测试环境的时候加载该类）