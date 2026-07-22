# PLC 示例工程

本目录包含已脱敏的 PLC 示例工程，用于学习、测试与验证 AI 协作工作流。所有示例均已移除客户数据、私人名称与专有标识。

## 目录结构

```text
examples/
├── melsec/
│   ├── fb-branch-mc/              # 三菱：功能块调用 + 分支 + MC/MCR
│   └── structure-primitives/      # 三菱：基本结构原语
├── siemens/
│   └── legacy-zh-call-network/    # 西门子：中文标签 + 调用网络
└── common/
    └── prompt-template.md         # 公开可用的 AI 协作者提示词模板
```

## 示例说明

### 三菱示例

| 示例 | 用途 | 文件 |
|------|------|------|
| `fb-branch-mc` | 演示功能块调用、MPS/MRD/MPP 分支栈、MC/MCR 控制区 | `payload/public-fb-branch-mc.gxw` |
| `structure-primitives` | 演示三菱工程基本结构元素 | `payload/public-structure-primitives.gxw` |

### 西门子示例

| 示例 | 用途 | 文件 |
|------|------|------|
| `legacy-zh-call-network` | 演示中文标签与调用网络结构 | `payload/PublicLegacyZhCallNetwork.ap16` |

## 使用建议

1. 在 GX Works 或 TIA Portal 中打开对应品牌的示例工程。
2. 配合 [`skills/SKILL.md`](../skills/SKILL.md) 中的护栏，让 AI 协助分析、审查或提出修改建议。
3. 所有修改建议先在离线环境中验证，再应用到生产项目。

## 脱敏声明

每个示例目录下的 `redaction-report.md` 记录了脱敏范围：

- 不包含任何客户项目或专有数据；
- 设备地址、程序名称已替换为通用占位符；
- 未调用任何官方软件、模拟器或第三方验证工具生成。

## 许可证

示例工程与项目文件同样遵循本仓库的 [MIT 许可证](../LICENSE)。
