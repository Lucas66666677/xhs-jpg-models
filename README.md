# 🚀 LUCAS 拆書實驗室 | 小紅書全自動排版工廠
![Python](https://img.shields.io/badge/Python-3.8%2B-blue)
![License](https://img.shields.io/badge/License-MIT-green)
[![Open In Colab](https://colab.research.google.com/assets/colab-badge.svg)](https://colab.research.google.com/drive/1fHmZH4gKLOYxKEmv-x9Q0DjM8tloEI98?usp=sharing)
> 這是一個專為深度內容創作者設計的自動化排版引擎。拒絕低質量的 AI 廢文感，利用像素級對齊算法，一鍵生成具備「外刊質感」的小紅書長圖卡。
---

## 🛠️ 核心功能 (Core Features)

- **像素級視覺換行 (Visual-Pixel Wrap)**：徹底解決中英混排時英文字符過窄導致的行末留白問題。
- **原子化列點控制 (Atomic List Control)**：自動監測列點高度，確保「03.」等內容不會在頁面底部被強行腰斬。
- **物理級呼吸間距 (Physical Paragraph Gap)**：模擬紙質雜誌排版，強製加入段落間的空白帶。
- **多語系避頭尾 (Kinsoku Shori)**：嚴格執行標點符號不落單、不居行首的排版準則。
- **一鍵無損下載**：跳過 ZIP 壓縮，直接向瀏覽器發送多重下載請求，獲取 1080x1440 最高畫質 JPG。

---

## 🎨 模板庫 (Template Registry)

目前已開發完成的 Model，後續將持續更新。

| 序號 | 模板名稱 (Model Name) | 視覺風格 | 連結 | 狀態 |
| :--- | :--- | :--- | :--- | :--- |
| **01** | **Modern Magazine (V5.5)** | 極簡白、紅色幾何、外刊質感 | [![Open In Colab](https://colab.research.google.com/assets/colab-badge.svg)](https://colab.research.google.com/drive/1fHmZH4gKLOYxKEmv-x9Q0DjM8tloEI98?usp=sharing)| ✅ 已上線 |
| 02 | Dark Mode Hardcore | 暗黑系、高對比、技術流 | [待更新] | 🚧 開發中 |
| 03 | Film Aesthetic | 底片質感、粗顆粒、膠卷邊框 | [待更新] | 📅 計劃中 |

---

## 🚀 如何使用 (Quick Start)

1. **點擊上方 `Open In Colab` 按鈕** 進入運行環境。
2. **上傳封面圖**：將你的底片作品或實拍照片命名為 `test_photo.jpg` 並上傳至左側資料夾。
3. **輸入文案**：在代碼下方的 `my_data` 模組中貼入你的簡體或繁體文案。
4. **一鍵運行**：點擊「全部執行」，檢查預覽圖後點擊底部的**綠色下載按鈕**。

---

## 📂 技術架構 (Architecture)

- **PIL (Pillow)**: 底層繪圖與圖像處理。
- **Ipywidgets**: 交互式 GUI 按鈕實現。
- **Noto Sans CJK SC**: 強制簡體中文索引渲染（解決字體變體問題）。

---

## ⚖️ 許可證 (License)

本項目採用 **MIT License**。歡迎 Fork 與交流，轉載請註明出處：**LUCAS 拆書實驗室**。

