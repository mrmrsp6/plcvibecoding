# 三菱 FB / 分支 / MC 示例

这是一个已脱敏的最小三菱 GX Works 示例工程，用于演示功能块调用、分支栈（MPS/MRD/MPP）以及 MC/MCR 控制区。

## 文件

- `payload/public-fb-branch-mc.gxw`：示例工程文件，可在 GX Works 中打开。
- `redaction-report.md`：脱敏声明与校验信息。

## 覆盖的梯形图元素

- 功能块（FB）调用与输入/输出绑定
- 分支栈指令 MPS / MRD / MPP
- 主控指令 MC / MCR

## 使用方式

1. 在 GX Works 中打开 `payload/public-fb-branch-mc.gxw`。
2. 结合本仓库 [`skills/SKILL.md`](../../../skills/SKILL.md) 的护栏，让 AI 协助分析程序结构。
3. 任何修改建议先在离线环境或仿真器中验证。

## 脱敏说明

本示例由维护者从公开教学场景生成，不包含客户数据或专有程序名称。详见 `redaction-report.md`。
