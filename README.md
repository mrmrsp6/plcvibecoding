# PLCvibeCoding

PLC 工程 AI 协作工作台

[English](#english) | [中文](#中文)

---

## 中文

PLCvibeCoding 是一款面向 PLC（可编程逻辑控制器）工程的桌面端 AI 协作工具。它把“工程导入 → 结构化理解 → AI 协作 → Patch 预览 → 安全写回”整合到一个界面里闭环完成，帮助工程师在工业控制场景下更安全、更高效地利用大语言模型。

> 本仓库仅包含项目公开资料：**产品文档、可复用的工作流技能（Skill）以及已脱敏的 PLC 示例工程**。核心应用源码与安装包不在代码仓库中；安装包请见 [GitHub Releases](https://github.com/mrmrsp6/plcvibecoding/releases)。

### 适用场景

- 导入三菱 GX Works / 西门子 TIA 工程，在统一视图中浏览梯形图与程序结构。
- 与 AI 协作完成需求分析、逻辑审查、修改建议与补丁规划。
- 在正式写回 PLC 或工程文件之前，先预览变更、确认影响范围。
- 使用统一的 prompt 护栏技能，让任意 AI 助手都能按保守、可控的方式处理 PLC 任务。

### 仓库内容

```text
.
├── docs/                 # 产品文档
│   ├── intro.md          # 产品定位与价值
│   ├── features.md       # 功能清单
│   ├── architecture-overview.md  # 高层架构说明
│   └── user-guide.md     # 公开技能使用指南
├── skills/               # 可复用的 AI 工作流技能
│   ├── SKILL.md          # 通用 PLC 协作护栏
│   ├── agents/
│   └── references/
├── examples/             # 已脱敏的 PLC 示例工程
│   ├── melsec/
│   └── siemens/
├── LICENSE               # MIT
└── NOTICE                # 第三方致谢
```

### 快速开始

1. 浏览 [`docs/intro.md`](docs/intro.md) 了解产品定位。
2. 查看 [`docs/features.md`](docs/features.md) 了解公开功能。
3. 在 [`skills/SKILL.md`](skills/SKILL.md) 中获取可在任意 AI 助手中使用的 PLC 协作护栏。
4. 在 [`examples/`](examples/) 中查看三菱与西门子脱敏示例工程。

### 安装包

Windows 安装包由维护者在 [Releases](https://github.com/mrmrsp6/plcvibecoding/releases) 中单独发布，不在本仓库源码中。

### 许可证

本仓库采用 [MIT 许可证](LICENSE)。第三方依赖与致谢请见 [NOTICE](NOTICE)。

---

## English

PLCvibeCoding is a desktop AI collaboration workbench for PLC (Programmable Logic Controller) projects. It closes the loop of "project import → structured understanding → AI collaboration → patch preview → safe writeback" in a single interface, helping engineers leverage large language models more safely and efficiently in industrial control scenarios.

> This repository only contains public materials: **product documentation, reusable workflow skills, and redacted PLC sample projects**. The core application source code and installer packages are not in this code repository; installers are published via [GitHub Releases](https://github.com/mrmrsp6/plcvibecoding/releases).

### Use Cases

- Import Mitsubishi GX Works / Siemens TIA projects and browse ladder logic and program structure in a unified view.
- Collaborate with AI on requirement analysis, logic review, modification suggestions, and patch planning.
- Preview changes and confirm impact before writing back to the PLC or project file.
- Use the shared prompt-guard skill to make any AI assistant handle PLC tasks in a conservative, controllable way.

### Repository Contents

```text
.
├── docs/                 # Product documentation
│   ├── intro.md          # Product positioning and value
│   ├── features.md       # Feature list
│   ├── architecture-overview.md  # High-level architecture
│   └── user-guide.md     # How to use the public skills
├── skills/               # Reusable AI workflow skills
│   ├── SKILL.md          # General PLC collaboration guardrails
│   ├── agents/
│   └── references/
├── examples/             # Redacted PLC sample projects
│   ├── melsec/
│   └── siemens/
├── LICENSE               # MIT
└── NOTICE                # Third-party notices
```

### Quick Start

1. Read [`docs/intro.md`](docs/intro.md) for product positioning.
2. See [`docs/features.md`](docs/features.md) for the public feature list.
3. Get the PLC collaboration guardrail for any AI assistant in [`skills/SKILL.md`](skills/SKILL.md).
4. Browse redacted Mitsubishi and Siemens sample projects in [`examples/`](examples/).

### Installer

The Windows installer is published separately by the maintainers in [Releases](https://github.com/mrmrsp6/plcvibecoding/releases), not in this source repository.

### License

This repository is licensed under the [MIT License](LICENSE). Third-party dependencies and acknowledgments are listed in [NOTICE](NOTICE).
