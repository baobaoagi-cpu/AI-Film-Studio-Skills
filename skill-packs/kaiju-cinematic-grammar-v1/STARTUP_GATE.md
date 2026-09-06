# KAIJU_SKILL_PREFLIGHT_V1

Kaiju / giant-scale 任務的工作前須知。

## CoWork 開工前
1. 判斷 task 是否觸發 Kaiju Skill Pack。
2. 讀 `skills/REGISTRY.yaml` 與本 Pack README。
3. 依 Shot 選 `skills_required`，不得整包無差別載入。
4. 宣告：shot_id、departments_active、skills_loaded、canon_refs、physics_constraints。
5. 先驗 3D / physics / continuity，再進付費生成。
6. 完工回報 `skills_used / skills_created / skills_upgraded / failure_modes_seen`。

## Codex 開工前
1. 驗證 Registry 與 Pack 版本存在。
2. 驗證所有 skill_id 合法。
3. 該觸發 Pack 卻沒有 `skills_loaded` 時，標記 `preflight_missing`。
4. 對 Canon、Scene Lock、revision、scale/timing、text integrity、crowd continuity、cost evidence 建立可自動化 Gate。
5. Research candidate 不得自行升級為 Studio Standard。

## Paid Generation Gate
- [ ] Canon current
- [ ] Skills loaded
- [ ] Camera position physically motivated
- [ ] Scale anchors present
- [ ] Motion source free of hovering/sliding/arbitrary slowdown
- [ ] Giant/human XYZ and eyelines validated
- [ ] Motion / Look / Identity / Voice responsibilities separated
- [ ] Readable text authored and protected
- [ ] Crowd continuity protected
- [ ] Environmental reactions obey causality, travel time, inertia and damping
- [ ] Weather / cloud / atmosphere physically plausible
- [ ] Audio strategy includes position, distance, propagation and reflections
- [ ] Final payload cost preflight complete
- [ ] Director budget authorization present
- [ ] Low-resolution validation passed before high-resolution final
