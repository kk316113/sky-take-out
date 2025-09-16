# Sky Take Out

一个基于 **Spring Boot** 开发的外卖点餐系统，支持用户点餐、商家管理、订单处理等功能。后端提供完整的 API 接口，并集成了 **Redis** 作为缓存提升性能。

## 📌 功能特性

* 用户端

  * 待开发
* 管理端

  * 菜品管理
  * 分类管理
  * 订单管理
  * 员工管理
  * 套餐管理
* 系统支持

  * Redis 缓存优化
  * MyBatis 数据持久层
  * 全局异常处理
  * 日志管理等

## 🛠️ 技术栈

* **后端框架**: Spring Boot, Spring MVC
* **数据库**: MySQL 8.0.41
* **ORM**: MyBatis
* **缓存**: Redis
* **接口文档**: Swagger
* **构建工具**: Maven

## 📂 部分项目结构

```
sky-take-out
│── sky-server           // 后端服务
│   ├── src/main/java    // 业务代码
│   ├── src/main/resources
│   │    ├── application.yml // 配置文件
│   └── ...
```

## 🚀 快速启动

### 1. 克隆项目

```bash
git clone https://github.com/你的用户名/sky-take-out.git
cd sky-take-out/sky-server
```

### 2. 配置数据库

在 `application.yml` 中修改 MySQL 和 Redis 配置：

```yaml
spring:
  datasource:
    url: jdbc:mysql://localhost:3306/sky_take_out?serverTimezone=UTC&useUnicode=true&characterEncoding=UTF-8
    username: root
    password: 123456
  redis:
    host: localhost
    port: 6379
```

### 3. 初始化数据库

执行 `resources/db` 目录下的 SQL 脚本，创建数据表。

### 4. 启动项目

```bash
mvn spring-boot:run
```

访问接口文档：

```
http://localhost:8080/doc.html
```

## 📖 API 文档示例

* **用户登录**: `POST /user/login`
