# 黎明助手 / Grim Dawn Assistant

Grim Dawn 的任務追蹤、地圖 Overlay 與自訂掉落篩選工具。

目前版本：**v0.4.12**

[下載最新版本](https://github.com/z-junn/GrimDawn_Quest_Tracker/releases/latest) · [v0.4.12 更新內容與檔案](https://github.com/z-junn/GrimDawn_Quest_Tracker/releases/tag/v0.4.12)

建議下載 Win64.zip，解壓縮後啟動 GrimDawnAssistant.exe。原始碼與「程式＋原始碼」完整包亦在 Release 提供。SHA256SUMS.txt 可核對下載內容。

## v0.4.12 更新

- 前後綴新增盾牌與副手法器，分類整理為「飾品&副手」。
- 對應詞綴的等級效果、職業分組與中英文搜尋一併加入。
- 遊戲端同步補上盾牌與副手法器辨識；更新後請重開 Grim Dawn。
- Filter 跟隨介面大小與文字大小設定。
- 已驗證 v0.4.11 → v0.4.12 保留已套用 Filter、具名存檔與 Overlay 設定。

## 功能

- 任務依章節及主線／支線分組，可獨立收合；依存檔階段顯示目標、NPC 與任務位置。同一目標的隨機地點可合併在同一張地圖。
- 地圖 Overlay、可自訂快捷鍵、方向線與 GPS 導航；保留迷霧探索引導與跨區路線功能。
- 掉落篩選整合詞條與前後綴，支援單手／雙手武器、護甲、飾品與副手的適用性選擇、效果說明、職業分組、AND／OR、Undo 與具名存檔。
- 搜尋接受簡體中文、繁體中文與英文。繁體為搜尋別名；顯示名稱以官方中英文 tag 核查。
- 數值條件接受單一 >、< 或 = 與 0～99999 整數，留空不限數值。傷害區間以上限比較，例如 80–120 符合 >100。

## 更新與設定

保留原 Data 與 Backups 資料夾；更新保留玩家 filter 存檔與 Overlay 設定。本版更新原生篩選 DLL，請退出並重開 Grim Dawn，再啟動 GDA。Overlay 引擎及 GPS 資料保持不變。

舊規則不會在開啟新版時被自動改寫。具名 filter 存檔與數值條件、Overlay 啟用／停用狀態和快捷鍵均保留。格式變更前備份，錯誤或失敗不會清空原始檔案。新編輯器草稿／具名存檔位於 Data/loot-editor.json，已套用規則位於 Data/loot-applied.json。

## 核查範圍與限制

全部 6191 筆前後綴定義已對照官方中英文 tag；189 個篩選項目使用衍生標籤，沒有冒充遊戲內獨立原句。13 個來源型複合效果僅判斷有無；103 個詞綴候選版本的正常生成路徑仍待確認。包含定義不代表保證掉落。

測試包含單元／原生 fixture、隔離介面與更新交接；未連接玩家遊戲或宣稱逐件實測掉落。版本指紋或資料讀取不符時保留原遊戲篩選。詳細核查報告與限制隨封包 docs/ 及 VERIFICATION.json 提供。

## English

Grim Dawn Assistant provides quest-stage maps, a map overlay and a custom loot filter. Version 0.4.12 adds shield/caster off-hand affixes under Accessories & Off-hands and fixes filter UI/text scaling. It includes unified property/affix filters, named presets, integer thresholds and simplified/traditional Chinese plus English search. Existing saved filters and Overlay preferences are preserved across updates.

Download the Win64 package from Releases. Restart Grim Dawn after updating to load the new filter bridge, and retain your existing Data folder. Source and complete packages are available with SHA256 checksums. Official game assets and names belong to Crate Entertainment; GrimTools map sources are credited in the application. See bundled licenses and verification reports.
