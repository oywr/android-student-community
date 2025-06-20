# 华南师范大学滨海校园预约服务平台

华南师范大学滨海校园预约服务平台是一个集空间预约、活动报名、志愿服务报名和通知管理于一体的综合服务平台。该平台旨在为滨海校园的师生提供便捷的预约和报名服务，提高校园资源利用效率。

## 技术栈

- 后端：Spring Boot 3.x、MyBatis-Plus、JWT
- 数据库：MySQL 8.x
- 消息推送：Firebase Cloud Messaging

## 功能特点

### 用户管理
- 用户注册、登录
- 个人信息管理
- 密码修改

### 空间预约
- 空间浏览和搜索
- 预约时间段查询
- 创建和取消预约
- 预约提醒

### 活动管理
- 活动列表和详情查看
- 活动报名和取消
- 活动签到
- 活动评价

### 志愿服务
- 志愿服务浏览
- 服务报名和取消
- 服务签到
- 志愿工时统计

### 通知系统
- 实时推送通知
- 通知列表查看
- 标记通知为已读

## 安装与运行

### 环境要求
- JDK 17+
- Maven 3.6+
- MySQL 8.0+
- Firebase项目（用于消息推送）

### 数据库配置
1. 创建数据库
```sql
CREATE DATABASE student_community DEFAULT CHARACTER SET utf8mb4 COLLATE utf8mb4_unicode_ci;
```

2. 修改配置文件
```
修改 src/main/resources/application.yml 中的数据库连接信息
```

### Firebase配置
1. 从Firebase控制台下载配置文件，放入项目resources目录
2. 更新配置文件中的firebase.config-file值

### 运行项目
```bash
# 克隆项目
git clone https://github.com/yourusername/student-community.git

# 进入项目目录
cd student-community

# 编译
mvn clean package

# 运行
java -jar target/springboot-0.0.1-SNAPSHOT.jar
```

## API文档

详细API文档请参考[API文档](api_documentation.md)

## 贡献指南

1. Fork 本仓库
2. 创建功能分支 (`git checkout -b feature/AmazingFeature`)
3. 提交更改 (`git commit -m 'Add some AmazingFeature'`)
4. 推送到分支 (`git push origin feature/AmazingFeature`)
5. 创建Pull Request

## 许可证

本项目采用 MIT 许可证 - 查看 [LICENSE](LICENSE) 文件了解更多详情。 
