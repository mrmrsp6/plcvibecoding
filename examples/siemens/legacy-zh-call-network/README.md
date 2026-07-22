# 西门子中文标签调用网络示例

这是一个已脱敏的最小西门子 TIA Portal 示例工程，用于演示中文标签、调用网络（Call Network）以及传统项目结构。

## 文件

- `payload/PublicLegacyZhCallNetwork.ap16`：示例工程文件，可在 TIA Portal 中打开。
- `payload/System/PEData.plf`：工程辅助数据文件。
- `redaction-report.md`：脱敏声明与校验信息。

## 覆盖的梯形图元素

- 中文标签与注释
- 传统调用网络结构
- 基本逻辑组织方式

## 使用方式

1. 在 TIA Portal 中打开 `payload/PublicLegacyZhCallNetwork.ap16`。
2. 结合本仓库 [`skills/SKILL.md`](../../../skills/SKILL.md) 的护栏，让 AI 协助分析程序结构。
3. 任何修改建议先在离线环境或仿真器中验证。

## 脱敏说明

本示例由维护者从公开教学场景生成，不包含客户数据或专有程序名称。详见 `redaction-report.md`。
