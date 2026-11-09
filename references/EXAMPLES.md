# 课程顾问沟通质检示例

## 典型场景

顾问在试听邀约中说“保证进入重点班”，且没有确认家长时间和学生基础。

## 具体示例

Agent 标记违规承诺，引用对话证据，并建议补充需求确认和到访安排，不自动处罚员工。

## 脱敏输入示例

```json
{
  "contract_version": "1.2.0",
  "data_status": "confirmed",
  "contains_sensitive_data": false,
  "requested_output_language": "zh-CN",
  "conversation_transcripts_redacted": [
    {}
  ],
  "authorization_status": "已取得明确授权并完成脱敏",
  "course_and_price": "课程与价格已核对（脱敏示例）",
  "consultant_stage": "沟通阶段已核对（脱敏示例）",
  "sales_policy": "销售规范已核对（脱敏示例）",
  "prohibited_claims": [
    {}
  ],
  "review_period": "质检周期已核对（脱敏示例）",
  "resume_mode": "new"
}
```

## 预期处理

1. 运行输入契约校验。
2. 逐项核对输入来源、版本和口径。
3. 按`references/PROFESSIONAL_PLAYBOOK.md`完成专业分析。
4. 输出沟通质检报告、证据片段、风险承诺等核心成果。
5. 由销售主管/校区负责人/合规人员确认沟通事实、违规承诺、处置决定与员工沟通；不得作为唯一人事依据后才可作为正式业务结论。

## 不应出现的输出

- 虚构政策、价格、人员、课程或客户事实。
- 以“暂无”“待完善”等占位文本冒充完成。
- 无依据的确定性判断或伪造人工签批。
