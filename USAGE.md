# 使用说明

## 适用任务

顾问在试听邀约中说“保证进入重点班”，且没有确认家长时间和学生基础。

## 准备输入

沟通转录/摘要、课程与价格、授权状态、沟通目标、顾问阶段、销售规范和禁用承诺。使用前先脱敏姓名、联系方式和与任务无关的敏感信息。

## 操作步骤

1. 确认授权和数据范围
2. 切分沟通结构
3. 评分与引用证据
4. 标记事实/合规风险
5. 生成一对一辅导
6. 抽样复测

## 校验命令

```powershell
node scripts/validate_input.js examples/typical_input.json
node scripts/validate_output.js examples/typical_output.json
```

## 状态使用

- `completed`：核心成果完整。
- `completed_with_limits`：只完成可验证部分，并说明受阻范围。
- `needs_input`：缺少关键输入。
- `needs_confirmation`：资料冲突或需人工确认。
- `failed`：工具或计算失败，提供恢复动作。

## 人工确认

销售主管/校区负责人/合规人员复核沟通事实、违规承诺、处置决定与员工沟通；不得作为唯一人事依据后，成果才可进入正式业务使用。
