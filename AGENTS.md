# AGENTS.md - JLPT 日語文法與詞彙知識庫 (Nihongo Lab)

## 1. 專案目的 (Project Overview)
本專案為一個靜態網頁形式的「JLPT 日語學習知識庫」，旨在系統化整理日語檢定（N5 至 N1）的文法解析、易混淆句型比較與核心單字筆記。
透過本文件的規範，AI 助教（Coding Agent）能夠在收到簡單的日語文法或單字主題時，自動生成符合全站統一視覺風格、排版結構與互動邏輯的教材頁面，並自動更新網站首頁的導覽索引。

## 2. 技術架構與檔案命名規範 (Architecture & File Naming)
本專案採用純靜態網頁技術（Vanilla HTML5 / CSS3 / ES6 JavaScript），不依賴任何外部前端框架或打包工具，以確保可直接部署於 GitHub Pages。

### 目錄結構
```text
project-root/
├── AGENTS.md                 # AI 協作與開發規則說明文件
├── index.html                # 知識庫首頁（包含級別篩選器與所有筆記卡片索引）
├── assets/
│   └── css/
│       └── style.css         # 全站共用樣式表（包含設計系統變數與 RWD 排版）
└── lessons/                  # 存放所有獨立的文法/單字講義頁面
    ├── n3-uchi-ni.html       # 範例講義：～うちに (N3)
    └── n2-ni-tsuke.html      # 範例講義：～につけ (N2)