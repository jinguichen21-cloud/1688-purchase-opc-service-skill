# 1688 Purchase OPC Service Skill

这个 Skill 用于企业采购推荐场景。

它约束 AI 在调用 `1688_opc_purchase_service` 后：
- 第一部分只返回最多 3 个商品
- 第二部分固定返回采购提示和 markdown 下单深链 `[1688企业采购agent](...)`
- 执行时必须把下单链接中的 `${corpId}` 替换为悟空当前真实 `corpId`

目录说明：
- `SKILL.md`：主技能说明
- `references/api-reference.md`：字段和输出格式细则
- `references/error-codes.md`：常见异常处理
- `tests/testcases.json`：单 tool 评测样例
