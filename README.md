<div align="center">

# Awesome Claude Code

[![Awesome](https://awesome.re/badge.svg)](https://awesome.re)
[![GitHub Stars](https://img.shields.io/github/stars/zycgenius/awesome-claude-code?style=flat-square&logo=github)](https://github.com/zycgenius/awesome-claude-code)
[![GitHub Forks](https://img.shields.io/github/forks/zycgenius/awesome-claude-code?style=flat-square&logo=github)](https://github.com/zycgenius/awesome-claude-code)
[![License: CC0-1.0](https://img.shields.io/badge/License-CC0_1.0-lightgrey.svg?style=flat-square)](https://creativecommons.org/publicdomain/zero/1.0/)

**精心策划的 Claude Code 资源合集**

Claude Code 是 Anthropic 推出的 AI 编程 CLI 工具，本项目收集了最优质的扩展、工具、教程和最佳实践。

[English](#english) | [中文](#目录)

</div>

---

## 为什么收藏这个项目？

- 🔥 Claude Code 正在改变开发者的工作方式
- 📦 一站式找到所有 MCP 服务器、Hooks、技能扩展
- 🇨🇳 中文社区最全的 Claude Code 资源
- 🔄 持续更新，欢迎贡献

## 目录

- [官方资源](#官方资源)
- [MCP 服务器](#mcp-服务器)
- [Hooks 钩子](#hooks-钩子)
- [Skills 技能扩展](#skills-技能扩展)
- [CLAUDE.md 模板](#claudemd-模板)
- [Agent SDK 项目](#agent-sdk-项目)
- [实用工具](#实用工具)
- [教程与文章](#教程与文章)
- [视频教程](#视频教程)
- [最佳实践](#最佳实践)
- [社区](#社区)
- [贡献指南](#贡献指南)

---

## 官方资源

> Anthropic 官方发布的 Claude Code 相关资源

| 资源 | 描述 | 链接 |
|------|------|------|
| Claude Code 官方文档 | 官方文档，最权威的参考资料 | [docs](https://docs.anthropic.com/en/docs/claude-code) |
| Claude Code GitHub | 官方仓库，反馈问题和功能请求 | [GitHub](https://github.com/anthropics/claude-code) |
| Claude Code SDK | 构建自定义 Agent 的官方 SDK | [GitHub](https://github.com/anthropics/claude-code-sdk) |
| MCP 协议规范 | Model Context Protocol 官方规范 | [GitHub](https://github.com/modelcontextprotocol) |
| Anthropic API 文档 | API 参考文档 | [docs](https://docs.anthropic.com/en/api) |

---

## MCP 服务器

> Model Context Protocol (MCP) 服务器扩展，让 Claude Code 连接外部工具和数据源

### 数据库

| 名称 | 描述 | 语言 |
|------|------|------|
| [mcp-server-postgres](https://github.com/modelcontextprotocol/servers/tree/main/src/postgres) | PostgreSQL 数据库连接 | TypeScript |
| [mcp-server-sqlite](https://github.com/modelcontextprotocol/servers/tree/main/src/sqlite) | SQLite 数据库操作 | Python |
| [mcp-server-mysql](https://github.com/benborla29/mcp-server-mysql) | MySQL 数据库连接 | TypeScript |
| [mcp-server-redis](https://github.com/modelcontextprotocol/servers/tree/main/src/redis) | Redis 缓存操作 | TypeScript |

### 开发工具

| 名称 | 描述 | 语言 |
|------|------|------|
| [mcp-server-github](https://github.com/modelcontextprotocol/servers/tree/main/src/github) | GitHub API 集成 | TypeScript |
| [mcp-server-gitlab](https://github.com/modelcontextprotocol/servers/tree/main/src/gitlab) | GitLab API 集成 | TypeScript |
| [mcp-server-git](https://github.com/modelcontextprotocol/servers/tree/main/src/git) | Git 操作 | Python |
| [mcp-server-docker](https://github.com/modelcontextprotocol/servers/tree/main/src/docker) | Docker 容器管理 | TypeScript |

### 搜索与爬虫

| 名称 | 描述 | 语言 |
|------|------|------|
| [mcp-server-brave-search](https://github.com/modelcontextprotocol/servers/tree/main/src/brave-search) | Brave 搜索引擎 | TypeScript |
| [mcp-server-fetch](https://github.com/modelcontextprotocol/servers/tree/main/src/fetch) | 网页内容抓取 | Python |
| [mcp-server-firecrawl](https://github.com/mendableai/firecrawl-mcp-server) | 网页爬取与提取 | TypeScript |

### 文件与系统

| 名称 | 描述 | 语言 |
|------|------|------|
| [mcp-server-filesystem](https://github.com/modelcontextprotocol/servers/tree/main/src/filesystem) | 文件系统操作 | TypeScript |
| [mcp-server-memory](https://github.com/modelcontextprotocol/servers/tree/main/src/memory) | 知识图谱记忆 | TypeScript |

### 云服务

| 名称 | 描述 | 语言 |
|------|------|------|
| [mcp-server-aws](https://github.com/modelcontextprotocol/servers/tree/main/src/aws) | AWS 服务集成 | TypeScript |
| [mcp-server-gcp](https://github.com/nicholasoxford/gcp-mcp-server) | Google Cloud 服务 | TypeScript |

### 生活与效率

| 名称 | 描述 | 语言 |
|------|------|------|
| [mcp-server-slack](https://github.com/modelcontextprotocol/servers/tree/main/src/slack) | Slack 消息集成 | TypeScript |
| [mcp-server-notion](https://github.com/suekou/mcp-notion) | Notion 笔记集成 | TypeScript |
| [mcp-server-google-maps](https://github.com/modelcontextprotocol/servers/tree/main/src/google-maps) | Google 地图 | TypeScript |

> 💡 更多 MCP 服务器请访问 [MCP Servers 官方仓库](https://github.com/modelcontextprotocol/servers)

---

## Hooks 钩子

> Claude Code Hooks 让你在特定事件触发时自动执行操作

### 实用 Hooks 示例

| 名称 | 描述 | 链接 |
|------|------|------|
| 自动格式化 | 文件保存后自动运行 Prettier/ESLint | [示例](#hooks-示例) |
| 提交检查 | 提交前自动运行测试 | [示例](#hooks-示例) |
| 通知推送 | 任务完成时发送通知 | [示例](#hooks-示例) |
| 自定义斜杠命令 | 通过 hooks 扩展斜杠命令 | [示例](#hooks-示例) |

### Hooks 配置示例

```json
// .claude/settings.json
{
  "hooks": {
    "PostToolUse": [
      {
        "matcher": "Write|Edit",
        "hooks": [
          {
            "type": "command",
            "command": "npx prettier --write $CLAUDE_FILE_PATH"
          }
        ]
      }
    ],
    "Notification": [
      {
        "hooks": [
          {
            "type": "command",
            "command": "osascript -e 'display notification \"Claude Code 任务完成\" with title \"通知\"'"
          }
        ]
      }
    ]
  }
}
```

> 💡 更多 Hooks 用法请参考 [官方文档](https://docs.anthropic.com/en/docs/claude-code/hooks)

---

## Skills 技能扩展

> Claude Code 技能（Skills）是可复用的提示词模板，通过 `/` 斜杠命令调用

### 热门技能

| 名称 | 描述 | 用途 |
|------|------|------|
| `/review` | 代码审查 | 审查 PR 变更 |
| `/security-review` | 安全审查 | 检查安全漏洞 |
| `/init` | 项目初始化 | 生成 CLAUDE.md |
| `/verify` | 验证变更 | 确认修改生效 |
| `/loop` | 循环执行 | 定时轮询任务 |

### 自定义技能

你可以在 `.claude/skills/` 目录下创建自定义技能：

```markdown
<!-- .claude/skills/deploy.md -->
---
name: deploy
description: 部署项目到生产环境
---

部署检查清单：
1. 运行所有测试
2. 检查环境变量
3. 构建生产版本
4. 部署到服务器
5. 验证部署状态
```

---

## CLAUDE.md 模板

> 项目级 Claude Code 配置文件模板

### 基础模板

```markdown
# CLAUDE.md

## 项目概述
简短描述项目

## 技术栈
- 语言：TypeScript
- 框架：Next.js
- 数据库：PostgreSQL

## 常用命令
- `npm run dev` - 启动开发服务器
- `npm test` - 运行测试
- `npm run build` - 构建生产版本

## 代码规范
- 使用 TypeScript 严格模式
- 组件使用 PascalCase
- 工具函数使用 camelCase

## 项目结构
src/
├── components/   # React 组件
├── hooks/        # 自定义 Hooks
├── utils/        # 工具函数
└── pages/        # 页面
```

### 高级模板

> 更多模板请查看 [templates/](./templates/) 目录

| 模板 | 适用场景 |
|------|----------|
| [前端项目模板](./templates/frontend.md) | React/Vue/Angular 项目 |
| [后端 API 模板](./templates/backend.md) | Node.js/Python API 项目 |
| [全栈项目模板](./templates/fullstack.md) | Next.js/Nuxt.js 全栈项目 |
| [CLI 工具模板](./templates/cli.md) | 命令行工具项目 |
| [Python 项目模板](./templates/python.md) | Python 项目 |

---

## Agent SDK 项目

> 使用 Claude Code SDK 构建的自定义 Agent

| 名称 | 描述 | 语言 |
|------|------|------|
| [claude-code-sdk-python](https://github.com/anthropics/claude-code-sdk-python) | Python SDK | Python |
| [claude-code-sdk-js](https://github.com/anthropics/claude-code-sdk-js) | JavaScript/TypeScript SDK | TypeScript |

### Agent 示例项目

```python
# 使用 Python SDK 的简单示例
from claude_code_sdk import query, ClaudeCodeOptions

result = query(
    prompt="分析这个项目的代码结构",
    options=ClaudeCodeOptions(
        max_turns=3,
        system_prompt="你是一个代码分析专家"
    )
)
print(result)
```

---

## 实用工具

> 围绕 Claude Code 生态的实用工具

| 名称 | 描述 | 类型 |
|------|------|------|
| [Claude Code Status Bar](https://github.com/anthropics/claude-code#status-line) | 状态栏配置 | 配置 |
| [cc-usage](https://github.com/anthropics/claude-code#costs) | 费用统计 | 工具 |
| [MCP Inspector](https://github.com/modelcontextprotocol/inspector) | MCP 调试工具 | 调试 |

---

## 教程与文章

> 精选的 Claude Code 教程和深度文章

### 入门教程

- 📝 [Claude Code 官方快速入门](https://docs.anthropic.com/en/docs/claude-code/quickstart)
- 📝 [Claude Code 概述](https://docs.anthropic.com/en/docs/claude-code/overview)
- 📝 [MCP 协议入门指南](https://modelcontextprotocol.io/introduction)

### 进阶教程

- 📝 [Claude Code Hooks 详解](https://docs.anthropic.com/en/docs/claude-code/hooks)
- 📝 [构建自定义 MCP 服务器](https://modelcontextprotocol.io/quickstart/server)
- 📝 [Claude Code Agent SDK 开发指南](https://docs.anthropic.com/en/docs/claude-code/sdk)

### 最佳实践

- 📝 [CLAUDE.md 配置最佳实践](https://docs.anthropic.com/en/docs/claude-code/memory)
- 📝 [MCP 服务器安全指南](https://modelcontextprotocol.io/docs/concepts/security)

---

## 视频教程

> YouTube 和 B 站上的优质视频教程

- 🎬 [Claude Code 官方演示](https://www.youtube.com/@anthropic) - Anthropic 官方频道
- 🎬 [Claude Code 入门教程](https://www.youtube.com/results?search_query=claude+code+tutorial) - 社区教程

---

## 最佳实践

> 使用 Claude Code 的经验和技巧

### 1. CLAUDE.md 编写技巧

```markdown
# 好的 CLAUDE.md
## 常用命令
- `npm test` - 运行测试（单个测试用 `npm test -- --grep "测试名"`）

## 注意事项
- 不要修改 migrations/ 目录下的已有文件
- API 路由在 src/app/api/ 目录下
```

### 2. 提示词技巧

```
✅ 好的提示：修复 src/auth.ts 中的登录验证 bug，用户输入空密码时应该返回 400 错误

❌ 差的提示：修复登录
```

### 3. 使用 Plan 模式

对于复杂任务，先用 Plan 模式规划再执行：
```
> 实现用户认证系统，支持 JWT 和 OAuth2
```

### 4. MCP 服务器选择

| 需求 | 推荐 MCP 服务器 |
|------|-----------------|
| 操作数据库 | postgres / sqlite / mysql |
| 搜索网页 | brave-search / fetch |
| 操作 GitHub | github |
| 管理文件 | filesystem |

---

## 社区

> 加入 Claude Code 社区，交流经验和问题

- 💬 [GitHub Discussions](https://github.com/anthropics/claude-code/discussions)
- 🐛 [Issue Tracker](https://github.com/anthropics/claude-code/issues)
- 📢 [Anthropic 官网](https://www.anthropic.com/claude-code)

---

## 贡献指南

欢迎贡献！请阅读 [CONTRIBUTING.md](./CONTRIBUTING.md) 了解如何参与。

### 如何贡献

1. Fork 本仓库
2. 创建你的分支 (`git checkout -b add-cool-resource`)
3. 提交你的更改 (`git commit -m 'Add cool resource'`)
4. 推送到分支 (`git push origin add-cool-resource`)
5. 创建 Pull Request

### 贡献类型

- ✅ 添加新的 MCP 服务器
- ✅ 添加新的 Hooks 示例
- ✅ 添加新的教程或文章
- ✅ 修复错误或改进现有内容
- ✅ 添加新的 CLAUDE.md 模板

---

## 致谢

感谢所有贡献者让这个项目变得更好！

[![Contributors](https://contrib.rocks/image?repo=zycgenius/awesome-claude-code)](https://github.com/zycgenius/awesome-claude-code/graphs/contributors)

---

## Star History

[![Star History Chart](https://api.star-history.com/svg?repos=zycgenius/awesome-claude-code&type=Date)](https://star-history.com/#zycgenius/awesome-claude-code&Date)

---

## License

[![CC0](https://licensebuttons.net/p/zero/1.0/88x31.png)](https://creativecommons.org/publicdomain/zero/1.0/)

本项目采用 [CC0 1.0](https://creativecommons.org/publicdomain/zero/1.0/) 许可证。

---

<div align="center">

**如果觉得有用，请给个 ⭐ Star 支持一下！**

</div>
