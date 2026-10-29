# Pokelike Story Custom — 私人研究與自訂難度專案

> 狀態：**規劃／稽核階段**。目前沒有匯入 Pokelike 官方或第三方的遊戲程式與素材，沒有可玩的版本，也沒有部署網站。

## 專案目標

以 [Pokelike](https://pokelike.xyz/) 的 **Story 劇情模式**為功能比較基準，研究製作可自行調整難度的獨立網頁遊戲。

需求方向：
- 盤點官方目前提供的所有劇情地區、地圖路線、事件、道館、四天王、冠軍。
- 盤點寶可夢種類、屬性、能力、進化、招式、特性、裝備與自動戰鬥規則。
- 對使用權限明確的內容建立可靠的實作與驗證；未獲授權的原始碼及美術素材**不可直接複製**。
- 難度新增「原版基準（待驗證）／簡單／休閒／自訂」，優先調整敵方傷害、敵方 HP、經驗獎勵及戰後恢復。
- 繁體中文、桌面與手機瀏覽器操作、獨立本機存檔與匯出備份。

## 重要邊界

1. **禁止未經授權複製及發布**官方或第三方的程式、素材和遊戲資料；公開可讀取不代表已授權重製。
2. 不接入、不改寫 Pokelike 官方的帳號、雲端存檔、排行榜或多人服務。
3. 開發期不啟用 GitHub Pages 或其他部署。若後續公開分享，應先重新審查權利與內容。
4. 未完成實測前，不宣稱與任何官方版本完全相同。
5. 若儲存庫應保持私人，請在 GitHub **Settings → General → Danger Zone → Change repository visibility** 將它設為 Private（此設定不會由目前的初始化檔案更改）。

## 專案文件

- [AGENTS.md](AGENTS.md)：Codex／程式代理的工作原則。
- [docs/PROJECT_SCOPE.md](docs/PROJECT_SCOPE.md)：範圍、階段與驗收條件。
- [docs/FEATURE_AUDIT.md](docs/FEATURE_AUDIT.md)：功能對照表與待驗證事項。
- [docs/DIFFICULTY_DESIGN.md](docs/DIFFICULTY_DESIGN.md)：難度系統規格草案。
- [docs/CODEX_PHASE1.md](docs/CODEX_PHASE1.md)：第一階段供 Codex 使用的稽核指令。
- [docs/STORY_REQUIREMENTS.md](docs/STORY_REQUIREMENTS.md)：劇情模式畫面、事件與系統需求。
- [docs/TEST_CASES.md](docs/TEST_CASES.md)：戰鬥、地圖、難度、存檔驗收測試。
- [docs/PRE_CODEX_CHECKLIST.md](docs/PRE_CODEX_CHECKLIST.md)：無法使用 Codex 時的準備項目。
- [docs/DECISIONS_AND_HANDOFF.md](docs/DECISIONS_AND_HANDOFF.md)：已定與待定事項、Codex 交接指令。

## 目前進度

- [x] 建立專用 GitHub 儲存庫
- [x] 設立規格與開發規則文件
- [ ] 核對外部程式及素材授權
- [ ] 確認官方版本與功能清單
- [ ] 取得可合法修改的程式基礎或重新實作
- [ ] 戰鬥／地圖／存檔整合測試
- [ ] 難度選項可玩測試
- [ ] 完整劇情驗收

## 研究來源（只作功能比較，**不代表授權**）

- 官方遊戲：https://pokelike.xyz/
- 待審查之第三方參考專案：https://github.com/pcasaspere/pokelike_v2

本儲存庫現階段僅儲存自行撰寫的專案文件。
