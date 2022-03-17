# Quality of life: Development tools



## Maven Dependency: JDBC

```HTML
<!-- https://mvnrepository.com/artifact/mysql/mysql-connector-java -->
<dependency>
    <groupId>mysql</groupId>
    <artifactId>mysql-connector-java</artifactId>
    <version>8.0.26</version>
</dependency>
```



## Auto-reload

```HTML
<dependency>
    <groupId>org.springframework.boot</groupId>
    <artifactId>spring-boot-devtools</artifactId>
    <scope>runtime</scope>
    <optional>true</optional>
</dependency>
```

![image-20220317131435292](quality-of-life.assets/image-20220317131435292.png)

## Multi-reference CSS

```html
<!DOCTYPE html>
<html lang="en" xmlns:th="http://www.thymeleaf.org">
<head>
    <meta charset="UTF-8">
    <title>Free money </title>
  	<!-- HERE -->
    <link rel="stylesheet" th:href="@{style.css}" href="../static/style.css">
```

