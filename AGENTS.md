# AGENTS.md — Cross-Project Studio Operating Rules

這個 repository 是跨專案的 Studio Knowledge Base。CoWork、Codex、ChatGPT 或其他 Agent 在使用本庫時，必須遵守以下流程。

## Startup Rule

任何正式製作任務開始前：
1. 先讀 `STUDIO_CONSTITUTION.md`。
2. 判斷這個任務屬於哪些 Department。
3. 查 `skills/REGISTRY.yaml`，只載入與任務相關的 Skill。
4. 再讀該專案自己的 Project Canon。
5. 將 `skills_loaded` 寫進 task / shot manifest。
6. 執行前確認所有 required Skill 的 checklist。

## Skill Routing

不要把全部 Skill 都塞進上下文。依 task trigger 動態載入。

例：巨物城市鏡頭可能載入：
- `GROUND_LEVEL_KAIJU_POV`
- `STORYBOARD_TO_3D_LAYOUT`
- `PRIMARY_MASS_SECONDARY_MECHANICS`
- `ENVIRONMENTAL_SCALE_REACTION`
- `GIANT_HUMAN_SPATIAL_BLOCKING`
- `WORLDIZED_SPATIAL_SOUND`

## CoWork Responsibility

CoWork 是主要片場執行者，可切換職務模式：Shot Planner、Cinematography、Previs/Physics、VFX/Generative、Editorial、Sound。

每次切換職務，只載入該職務需要的 Skill。

CoWork 必須：
- 先做物理與 Canon 檢查，再做視覺生成；
- 任何付費生成前跑 cost/preflight；
- 新發現先回報為 Skill Candidate，不可自行升級為 Studio Standard；
- 完工回報 `skills_used / skills_created / skills_upgraded / failure_modes_seen`。

## Codex Responsibility

Codex 是 Production Engineering / QA / Skill Engineering。

Codex 必須：
- 驗證 task 裡的 skill_id 都存在；
- 若應觸發 Skill Pack 卻沒有 `skills_loaded`，標記 `preflight_missing`；
- 管理 Scene Lock、revision、artifact、Canon、manifest；
- 對可自動化檢查建立 Gate；
- 只有經多個正式 Shot 驗證的 L3 Skill，才可提案升為 L4 automation。

## ChatGPT / Director Hub Responsibility

- 做 Skill Routing；
- 決定 active Departments 與 required Skills；
- 以 Skill checklist 審核成果，而不是只看『好不好看』；
- 新工具出現時可替換 tool route，但不可破壞已驗證能力與標準。

## Knowledge Contribution

任何新知識依序進入：
`learnings/raw` → `learnings/distilled` → `skills` → automation / studio standard。

禁止直接把一次性的 prompt、事故心得或單一模型技巧當成永久 Skill。
