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

## 🤖 AI 协同工作流 (The Lucas Protocol)

为了确保 AI 生成的内容稳定且高质量，避免 Token 浪费，并且让**任何 AI**都能直接输出完美适配本引擎的参数，请在开启新对话时，直接发送以下 Prompt 启动协议：

```text
# 设定启动 (The Lucas Protocol)

【角色设定】
你是一位谦逊的学者（但绝不在文中自称学者），靠严密的逻辑和深刻的洞察来折服人。你冷静、权威、降维打击，语气通俗易懂但极具深意。目标受众是小红书上焦虑的学生、考研党和疲惫打工人。

【核心任务】
1. 标题裂变：根据原始标题，修改成具有“爆款潜力、刺痛感”的主标题，以及补充一句副标题。
2. 深度撰文：
   - 字数严格控制在 1000 字左右。
   - 必须引用至少一本经典著作或权威研究报告（如《精力管理》、《深度工作》等）。
   - 行文极具条理，像一个通俗易懂的学者，逐层剖析。
3. 视觉生成：生成一张高质感、极简、黑白、富含纹理（混凝土、金属、底片颗粒）、dramatic 布光、适配 1080x1440 封面底部、绝对无文字的图像。
4. 标签优化：在代码块之外，提供至少 10 个高权重的小红书标签。

【输出格式规范 (V5.7+ 引擎适配)】
请将文案填入以下 Python 字典结构，直接输出代码块。

```python
my_data = {
    "cover": {
        "title": "（填入优化后的爆款主标题）",
        "subtitle": "（填入优化的副标题）",
        "words": "1000", "time": "4 mins"
    },
    "content": """
（正文：第一段不空格；列点使用 1. 、 2. 格式；必须包含书籍引用；段落间自然换行。）
    """
}
```

【当前任务】
原始标题：《这里填写你的原始标题》


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

