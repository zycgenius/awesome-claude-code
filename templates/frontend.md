# 前端项目 CLAUDE.md 模板

```markdown
# CLAUDE.md

## 项目概述
[项目名称] - [简短描述]

## 技术栈
- 框架：React 18 / Vue 3 / Angular 17
- 语言：TypeScript
- 样式：Tailwind CSS / CSS Modules
- 构建：Vite / Webpack
- 测试：Vitest / Jest + Testing Library

## 常用命令
- `npm run dev` - 启动开发服务器
- `npm run build` - 构建生产版本
- `npm run preview` - 预览生产构建
- `npm test` - 运行测试
- `npm run lint` - 代码检查
- `npm run format` - 代码格式化

## 代码规范
- 使用 TypeScript 严格模式
- 组件使用 PascalCase 命名
- 工具函数使用 camelCase 命名
- 常量使用 UPPER_SNAKE_CASE
- CSS 类名使用 kebab-case

## 项目结构
src/
├── components/     # 可复用组件
│   ├── ui/        # 基础 UI 组件
│   └── layout/    # 布局组件
├── pages/         # 页面组件
├── hooks/         # 自定义 Hooks
├── utils/         # 工具函数
├── services/      # API 服务
├── stores/        # 状态管理
├── types/         # TypeScript 类型定义
├── styles/        # 全局样式
└── assets/        # 静态资源

## 组件编写规范
- 使用函数式组件
- Props 使用 interface 定义
- 复杂逻辑抽取为自定义 Hook
- 避免内联样式

## API 约定
- 基础路径：/api/v1
- 认证方式：Bearer Token
- 错误格式：{ code: number, message: string }

## 注意事项
- 不要修改 vite.config.ts 除非必要
- 环境变量以 VITE_ 开头
- 公共组件放在 components/ui/ 目录
```
