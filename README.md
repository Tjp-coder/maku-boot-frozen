# Maku Boot - 测试目标系统（冻结快照）

> 这是 Maku Boot 后端系统的一个**老版本快照**（2022 年版本），
> 仅作为 [ReqMakuTest 接口自动化测试框架](https://github.com/Tjp-coder/ReqMakuTest)
> 的被测目标使用，**不接收上游更新，不修复 bug**。
>
> 完整官方版本请见：[Maku 官方](https://gitee.com/makunet/maku-boot)

## 用途

为 ReqMakuTest 测试框架提供稳定的被测系统，
保证测试用例（如错误文案断言、字段定义）与系统行为长期一致。

## 技术栈

Spring Boot 2.x / MySQL 8 / Redis / MyBatis Plus / Spring Security

## 启动方式

```bash
# 1. 导入数据库脚本
#    db/mysql/maku.sql

# 2. 修改 application-dev.yml 中的数据库连接信息

# 3. 启动
mvn spring-boot:run -pl maku-server
```

服务起在 http://localhost:8080，默认账号 admin / admin123

## 关联项目

- 接口自动化测试框架：[ReqMakuTest](https://github.com/Tjp-coder/ReqMakuTest)
- 在线测试报告：[Allure Report](https://tjp-coder.github.io/ReqMakuTest/)

## 致谢

感谢 [Maku 团队](https://gitee.com/makunet) 提供的优秀开源项目，
本仓库仅用于个人学习和测试框架演示，版权归原作者所有，遵循 MIT 协议。
