# Python 项目 CLAUDE.md 模板

```markdown
# CLAUDE.md

## 项目概述
[项目名称] - [简短描述]

## 技术栈
- Python 3.10+
- 包管理：uv / pip / poetry
- 测试：pytest
- 代码风格：ruff / black
- 类型检查：mypy

## 常用命令
- `uv run python main.py` - 运行程序
- `uv run pytest` - 运行测试
- `uv run ruff check .` - 代码检查
- `uv run ruff format .` - 代码格式化
- `uv run mypy .` - 类型检查

## 项目结构
src/
├── __init__.py
├── main.py         # 入口文件
├── config.py       # 配置管理
├── models/         # 数据模型
├── services/       # 业务逻辑
├── utils/          # 工具函数
├── api/            # API 路由
└── db/             # 数据库相关

tests/
├── conftest.py     # 测试配置
├── test_models/
├── test_services/
└── test_api/

## 代码规范
- 遵循 PEP 8
- 使用 type hints
- 函数和类必须有 docstring
- 使用 dataclass 或 Pydantic 定义数据模型

## 依赖管理
- 使用 uv 管理依赖
- 开发依赖放在 dev group
- 锁定依赖版本

## 注意事项
- 不要使用 print 调试，使用 logging
- 配置通过环境变量或 .env 文件
- 数据库操作使用 async/await
```
