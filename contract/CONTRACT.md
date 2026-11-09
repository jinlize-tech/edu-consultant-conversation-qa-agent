# 输入输出契约

## 输入字段

| 键 | 名称 | 类型 | 必填 |
|---|---|---|---|
| `conversation_transcripts_redacted` | 脱敏沟通记录 | array | 是 |
| `authorization_status` | 录制与使用授权状态 | string | 是 |
| `course_and_price` | 课程与价格 | string | 是 |
| `consultant_stage` | 沟通阶段 | string | 是 |
| `sales_policy` | 销售规范 | string | 是 |
| `prohibited_claims` | 禁用承诺 | array | 是 |
| `review_period` | 质检周期 | string | 是 |

## 状态

- `completed`：核心成果完整，关键结论人工确认要求满足。
- `completed_with_limits`：至少一项实质成果，说明限制、已完成和受阻范围。
- `needs_input`：必填字段缺失。
- `needs_confirmation`：资料冲突或人工确认未完成。
- `failed`：计算或工具失败。

## 输出

- `沟通质检报告`：结构化条目数组，不允许空壳或占位文本。
- `证据片段`：结构化条目数组，不允许空壳或占位文本。
- `风险承诺`：结构化条目数组，不允许空壳或占位文本。
- `需求缺口`：结构化条目数组，不允许空壳或占位文本。
- `辅导要点`：结构化条目数组，不允许空壳或占位文本。
- `团队趋势和复测记录`：结构化条目数组，不允许空壳或占位文本。

完整机器契约见`contract/input.schema.json`、`contract/output.schema.json`和`contract/runtime_contract.json`。
