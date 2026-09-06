# AI Film Studio Skills

跨專案、可重複使用的 AI 電影製作知識與技能庫。

這個 repository 保存的是「製片廠能力」，不是單一作品的 Canon。

## 核心目標

- 把每次拍片的成功、失敗與修正蒸餾成可重複使用的 Skill。
- 讓 ChatGPT / CoWork / Codex 在不同專案中共享同一套製片知識。
- 將 Raw Learning → Distilled Knowledge → Validated Skill → Automated Skill 持續迭代。
- 優先使用市場上最成熟的工具；只自建缺少的 orchestration、QA、locking、canon、cost 與 workflow glue。

## 知識分層

1. **Raw Learning**：一次實驗、事故、成功案例。
2. **Distilled Knowledge**：找出原因後形成的規則與 SOP。
3. **Validated Skill**：已在正式 Shot 中驗證，可重複使用。
4. **Automated Skill**：可由 Production Engineering 自動檢查或執行。
5. **Studio Standard**：跨專案強制採用的製片標準。

## 主要入口

- `STUDIO_CONSTITUTION.md` — 片廠最高原則
- `AGENTS.md` — Agent 工作前須知與 Skill 調用規則
- `skills/REGISTRY.yaml` — 全域 Skill Registry
- `departments/` — 10 個 Virtual Studio Departments
- `skill-packs/` — 可按任務載入的技能包
- `standards/` — 跨專案硬標準與防錯機制
- `templates/` — Shot / Skill / Postmortem 模板
- `research/` — 電影、工具與實驗研究

## Studio Mantra

> 我們不是在訓練一個 AI；我們是在訓練一整間會拍電影的虛擬製片廠。
