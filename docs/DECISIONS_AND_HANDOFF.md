# 已確定事項／待決事項／Codex 交接

## 已確定（來自使用者與目前專案）
- 目標：Pokelike **劇情模式**方向的獨立私人調整版本，增加難度選擇。
- 希望保留所有地區與核心玩法；具體複製與素材使用以權利許可為前提。
- 暫不製作 Battle Tower、多人／每日挑戰等非 Story 系統。
- 先在 GitHub 寫規格、再交由 Codex 做詳細稽核；**不直接部署**。
- 專案：https://github.com/TMHfred/pokelike-story-custom ，主分支 main。
- GitHub 目前 PUBLIC；私人研究者可自行切換 PRIVATE。
- 特別重視：選路策略、敵我隊伍與裝備、自動戰鬥、道館／聯盟、可恢復與經驗調整。

## 尚未決定（下列先採建議預設；需要使用者未來決定）
| 決策 | 建議預設 | 為什麼 |
|---|---|---|
| 首個技術驗收地區 | 關都 | 先做一地完整閉環，降低跨區誤差 |
| 預設難度 | 簡單 | 兼顧策略與降低重打成本 |
| 遊戲途中更改難度 | 不允許，下一局生效 | 存檔與測試一致 |
| 失敗後重來 | 保留 Roguelike 新局循環 | 避免把遊戲改成無限制復活 |
| 戰鬥資訊顯示 | 簡略播放＋可展開日誌 | 便於排查特性／道具錯誤 |
| 視覺與素材 | 先用自製占位圖 | 不依賴未授權素材 |
| 語系 | 繁體中文優先 | 符合使用者遊玩習慣 |
| 私人遊玩／網站發布 | 只做本機測試，不部署 | 避免授權與存檔風險 |

## Codex 之後的操作順序
1. 讀取 AGENTS.md、README.md、docs/CODEX_PHASE1.md、docs/STORY_REQUIREMENTS.md、docs/TEST_CASES.md、docs/DIFFICULTY_DESIGN.md。
2. 完成授權／來源、版本、功能對照與架構稽核；未能證實的部分標 UNKNOWN。
3. 提交 docs/LICENSE_AUDIT.md、docs/ARCHITECTURE_REVIEW.md、docs/GAP_MATRIX.md、docs/IMPLEMENTATION_PLAN.md、docs/RISK_LOG.md。
4. 產出一個供檢視的 PR，**先停止，不直接開始遊戲製作**。
5. 實作階段經核定後，再切分地圖、戰鬥、裝備、難度與存檔等可獨立測試的工作項。

## 可以直接貼給 Codex 的交接指令
「請開啟 TMHfred/pokelike-story-custom，閱讀 AGENTS.md 和 docs/CODEX_PHASE1.md，並參閱 docs/STORY_REQUIREMENTS.md、docs/TEST_CASES.md、docs/DIFFICULTY_DESIGN.md、docs/DECISIONS_AND_HANDOFF.md。先完成第一階段來源／授權與版本稽核，製作五份指定報告並列出有證據的功能差異。不要匯入未授權程式或素材、不要修改正式遊戲或存檔、不要部署網站。完成後用 PR 提供檢查，不要進入第二階段。」
