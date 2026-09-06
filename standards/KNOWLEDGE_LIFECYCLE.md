# Knowledge Lifecycle Standard

跨專案知識不得直接從聊天或單次實驗跳成永久 Skill。

## Lifecycle

`Raw Learning → Distilled Knowledge → SOP → Validated Skill → Automated Skill → Studio Standard`

### L0 — Raw Learning / Note
記錄：發生什麼、在哪一顆 Shot、使用哪個工具、成功或失敗。

### L1 — Rule
找出原因與因果，不只記結果。

### L2 — SOP
寫清楚 trigger、inputs、process、checks、outputs、handoff、failure modes。

### L3 — Validated Skill
至少在一顆正式 production Shot 中驗證成功，且別的執行者可以依 SOP 重複。

### L4 — Automated Skill
Codex / Production Engineering 可以自動檢查或執行至少一部分流程。

### L5 — Studio Standard
跨多個 Shot / Project 穩定成立，成為片廠硬規則。

## Promotion Record

每次升級都要留下：
- skill_id
- from_level / to_level
- evidence_shots
- root_cause / rationale
- tests_or_checklist
- approver
- date

## Deprecation

工具或模型可以淘汰；Skill Intent 不必跟著淘汰。

如果新工具更好，更新 tool route，而不是重寫已驗證的製片能力。

若規則被新證據推翻，標記 deprecated 並保留原因，禁止靜默覆寫歷史。
