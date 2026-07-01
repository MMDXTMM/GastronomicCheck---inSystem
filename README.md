# GastronomicCheck---inSystem

基于 Spring Boot 的点评类后端项目，包含店铺、博客、优惠券秒杀、关注等常见业务模块，并集成 Redis 缓存与分布式锁。

## 技术栈

- Java 8
- Spring Boot 2.3
- MyBatis-Plus
- MySQL
- Redis / Redisson

## 项目结构

```
GastronomicCheck---inSystem/   # Maven 主工程
  src/main/java/               # 业务代码
  src/main/resources/          # 配置与 SQL 脚本
```

## 本地运行

1. 创建 MySQL 数据库，并执行 `GastronomicCheck---inSystem/src/main/resources/db/hmdp.sql`
2. 修改 `GastronomicCheck---inSystem/src/main/resources/application.yaml` 中的数据库与 Redis 连接信息
3. 进入 `GastronomicCheck---inSystem` 目录后执行：

```bash
mvn spring-boot:run
```

默认服务端口：`8081`

## 注意事项

- 请勿将真实数据库密码、Redis 密码提交到公开仓库
- `.idea/` 等 IDE 配置文件已被忽略，不应纳入版本控制
