# FastAPI Modern Starter 🚀

这是一个基于 **FastAPI** 的现代化后端项目模板。它集成了最前沿的 Python 工具链：使用 **uv** 进行依赖管理，使用 **Ruff** 进行代码质量控制，并配备了完整的 **GitHub Actions** 自动化流程。

## ✨ 特性 (Features)

* ⚡ **高性能**: 基于 FastAPI，原生支持异步开发。
* 📦 **极速包管理**: 使用 [uv](https://github.com/astral-sh/uv) 替代 pip，秒级安装依赖。
* 🛠️ **代码规范**: 内置 [Ruff](https://github.com/astral-sh/ruff) 配置，涵盖格式化、导入排序及代码检查（Lint）。
* 🧪 **完备测试**: 预集成 `pytest` 和 `pytest-asyncio`。
* 🤖 **自动 CI/CD**: 预设 GitHub Actions，自动执行代码检查、测试及 Release 发布。

---

## 🛠️ 快速开始 (Quick Start)

### 1. 安装 uv

如果尚未安装 `uv`，请运行以下命令：

```bash
# macOS/Linux
curl -LsSf https://astral.sh/uv/install.sh | sh
# Windows
powershell -c "irbr https://astral.sh/uv/install.ps1 | iex"
```

### 2. 初始化环境

克隆仓库后，一键同步依赖并创建虚拟环境：

```bash
git clone git@github.com:aihohu/pydemo.git

cd pydemo

uv sync
```

### 3. 运行项目

```bash
fastapi dev app/main.py
```

访问 API 文档：[http://127.0.0.1:8000/docs](http://127.0.0.1:8000/docs)

---

## 👨‍💻 开发指南 (Development)

### 代码质量检查

在提交代码前，请确保通过 Ruff 的自动化修复和检查：

```bash
# 格式化代码
uv run ruff format .

# 代码检查并自动修复
uv run ruff check --fix .
```

### 运行测试

```bash
uv run pytest
```

---

## 📂 项目结构 (Structure)

```text
├── .github/          # GitHub Actions, Issue & PR 模板
├── app/              # 源代码目录
│   ├── __init__.py
│   └── main.py       # 入口文件
├── tests/            # 测试目录
│   ├── conftest.py   # Pytest 配置
│   └── test_main.py
├── pyproject.toml    # Ruff, uv & 项目配置
└── README.md

```

---

## 🤝 贡献 (Contributing)

欢迎任何形式的贡献！请阅读 [CONTRIBUTING.md](./CONTRIBUTING.md) 了解如何开始。

1. Fork 本项目
2. 创建您的特性分支 (`git checkout -b feature/AmazingFeature`)
3. 提交更改 (`git commit -m 'Add some AmazingFeature'`)
4. 推送到分支 (`git push origin feature/AmazingFeature`)
5. 开启一个 Pull Request

---

## 📄 开源协议 (License)

本项目采用 [MIT] 协议开源。