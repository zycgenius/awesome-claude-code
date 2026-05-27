# 后端 API 项目 CLAUDE.md 模板

```markdown
# CLAUDE.md

## 项目概述
[项目名称] - [简短描述]

## 技术栈
- 运行时：Node.js 20 / Python 3.12 / Go 1.22
- 框架：Express / FastAPI / Gin
- 数据库：PostgreSQL / MySQL
- 缓存：Redis
- ORM：Prisma / SQLAlchemy / GORM

## 常用命令
- `npm run dev` / `python manage.py runserver` / `go run .` - 启动开发服务器
- `npm test` / `pytest` / `go test ./...` - 运行测试
- `npm run migrate` / `alembic upgrade head` / 运行数据库迁移
- `npm run seed` / 填充测试数据

## API 规范
- RESTful 风格
- 基础路径：/api/v1
- 认证：JWT Bearer Token
- 分页：?page=1&limit=20
- 错误响应：{ error: { code: string, message: string } }

## 项目结构
src/
├── controllers/    # 请求处理
├── services/       # 业务逻辑
├── models/         # 数据模型
├── routes/         # 路由定义
├── middleware/      # 中间件
├── utils/          # 工具函数
├── config/         # 配置文件
└── migrations/     # 数据库迁移

## 数据库规范
- 表名使用复数形式（users, orders）
- 字段名使用 snake_case
- 必须有 id, created_at, updated_at 字段
- 外键命名：{table}_id

## 注意事项
- 不要直接修改已有迁移文件
- 敏感配置使用环境变量
- 所有 API 需要输入验证
- 数据库操作使用事务
```
