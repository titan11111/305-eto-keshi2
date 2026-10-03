# 305-eto-keshi2 学び

## 2026-10-03 v2を305に集約（262は復元）

- 誤って262に入れていた回転・12種・袋リトライ修正・連続配置ガードは **305 index.html** が正本
- 262は `79ba69b` 相当（3分タイムアタック・回転なし）にGitHubへ戻した

## 2026-10-03 袋リトライバグ

- `drawEtoFromBag` が配置失敗のたびに `etoSeen` を立てていた → `previewEtoKind` / `pickKindForCell` に分離

## 2026-10-03 262からマージ

- ベースを262に差し替え、回転を統合（`docs/rotation-mechanism.md`）
