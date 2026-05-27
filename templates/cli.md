# CLI 工具项目 CLAUDE.md 模板

```markdown
# CLAUDE.md

## 项目概述
[项目名称] - [简短描述]

## 技术栈
- 语言：Rust / Go / Node.js
- CLI 框架：clap / cobra / commander
- 输出格式：JSON / Table / YAML

## 常用命令
- `cargo run` / `go run .` / `node bin/cli.js` - 运行程序
- `cargo test` / `go test ./...` / `npm test` - 运行测试
- `cargo build --release` / `go build` / `npm run build` - 构建

## 项目结构
src/
├── main.rs / main.go / index.js  # 入口文件
├── cli.rs / cli.go / cli.js      # CLI 定义
├── commands/                      # 命令实现
├── config/                        # 配置管理
└── utils/                         # 工具函数

## CLI 设计规范
- 使用子命令模式：`tool command [args] [flags]`
- 支持 --help 和 --version
- 输出支持 JSON 格式：--json
- 退出码：0 成功，1 错误，2 用法错误

## 配置文件
- 位置：~/.config/tool/config.toml
- 环境变量：TOOL_*
- 命令行参数优先级最高

## 注意事项
- 处理好信号中断 (SIGINT)
- 大数据输出使用分页
- 错误信息要有帮助性
- 支持管道输入输出
```
