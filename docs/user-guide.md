# 公开技能使用指南

本仓库的 [`skills/`](../skills/) 目录提供了一套通用的 PLC 协作护栏，可直接在任何支持 Markdown system prompt 的 AI 助手（ChatGPT、Claude、DeepSeek、Ollama 等）中使用。

## 什么是 PLC 公开工作流护栏

它是一个轻量级的检查清单，用于提醒 AI 在处理 PLC 或梯形逻辑任务时：

- 先收集足够证据再下结论；
- 把确定的事实与推断分开；
- 补丁类任务必须有明确目标、最小改动与验证计划；
- 部署是独立授权边界，生成补丁不等于允许修改现场设备。

## 如何使用

### 方式一：直接复制到 system prompt

1. 打开 [`skills/SKILL.md`](../skills/SKILL.md)。
2. 将全文复制到你的 AI 助手的 system prompt 或自定义指令框中。
3. 在对话中上传 PLC 程序片段、梯形图截图或工程描述即可开始协作。

### 方式二：作为 Agent / Skill 引用

如果你使用的平台支持 YAML/JSON skill 定义，可引用 [`skills/agents/openai.yaml`](../skills/agents/openai.yaml) 中的接口声明。

### 方式三：按需引用参考文档

- [`skills/references/evidence-routing.md`](../skills/references/evidence-routing.md) — 证据收集与路由检查单
- [`skills/references/patch-safety.md`](../skills/references/patch-safety.md) — 补丁规划约束
- [`skills/references/release-boundary.md`](../skills/references/release-boundary.md) — 捕获保留与部署门禁

## 示例对话

**用户**：请帮我检查一下这段三菱梯形图有没有双线圈问题。

**AI（加载 SKILL.md 后）**：

> 在回答之前，我会先确认以下证据：
> 1. 你提供的程序片段是否包含完整的主程序 / 子程序 / 中断程序；
> 2. 相同输出继电器 Y 是否在多个梯级中被赋值；
> 3. 是否存在 MC/MCR 或跳转指令导致同一输出在不同条件下被覆盖。
>
> 请上传完整程序或告知我需要重点检查的程序块。

## 适用边界

- 本技能为**通用、厂商中立**的护栏，不替代具体品牌官方文档。
- 对于涉及现场设备的修改，仍需由具备资质的工程师确认并授权。
