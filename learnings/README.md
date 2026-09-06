# Learnings Pipeline

這裡保存尚未成為正式 Skill 的知識。

## raw/
一次性的實驗結果、錯誤、事故、成功案例、工具觀察。

建議格式：
- date
- project / shot
- observation
- tool / model
- evidence
- cost
- suspected cause

## distilled/
經過原因分析後的可泛化規則。

必須回答：
- 為什麼？
- 哪些情況成立？
- 哪些情況不成立？
- 能否以數字、工具或 Gate 固化？

## validated/
準備升級或已通過正式 Shot 驗證的 Skill 候選。

只有通過 checklist、具 evidence、可被不同執行者重複，才能搬進 `skills/`。

## Knowledge Distillation Rule

每個重要 Shot 完工後，至少做一次：
`raw learning → root cause → distilled rule → candidate skill → validation`。
