# 全栈项目 CLAUDE.md 模板

```markdown
# CLAUDE.md

## 项目概述
[项目名称] - [简短描述]

## 技术栈
- 框架：Next.js 14 / Nuxt 3 / SvelteKit
- 语言：TypeScript
- 数据库：PostgreSQL / MongoDB
- ORM：Prisma / Drizzle
- 认证：NextAuth.js / Lucia
- 样式：Tailwind CSS

## 常用命令
- `npm run dev` - 启动开发服务器
- `npm run build` - 构建生产版本
- `npm run db:push` - 推送数据库 schema
- `npm run db:studio` - 打开数据库管理界面
- `npm test` - 运行测试

## 项目结构
src/
├── app/              # App Router 页面
│   ├── (auth)/       # 认证相关页面
│   ├── (dashboard)/  # 仪表盘页面
│   └── api/          # API 路由
├── components/       # React 组件
├── lib/              # 工具库
│   ├── db.ts         # 数据库客户端
│   ├── auth.ts       # 认证配置
│   └── utils.ts      # 工具函数
├── hooks/            # 自定义 Hooks
└── types/            # 类型定义

prisma/
├── schema.prisma     # 数据库 schema
└── migrations/       # 迁移文件

## 数据库
- 使用 Prisma ORM
- Schema 文件：prisma/schema.prisma
- 迁移命令：npx prisma migrate dev

## API 约定
- 使用 Next.js Route Handlers
- API 路由在 app/api/ 目录
- 使用 Zod 进行输入验证

## 注意事项
- 服务端组件默认，需要交互时才用客户端组件
- 敏感操作需要验证用户身份
- 数据库查询注意 N+1 问题
```
