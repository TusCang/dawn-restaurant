# 黎明餐館 Dawn Restaurant Website

一個完整的靜態餐廳網站，使用 GitHub Pages 部署。

## 頁面結構

| 檔案 | 頁面 | 說明 |
|------|------|------|
| `index.html` | 首頁 | Hero、特色介紹、本週推薦、顧客好評 |
| `menu.html` | 菜單 | 早午餐、午餐、晚餐、飲品甜點 |
| `story.html` | 我們的故事 | 品牌故事、創辦理念、團隊介紹 |
| `reservation.html` | 訂位 | 線上訂位表單、訂位須知 |
| `gallery.html` | 環境照片 | 空間、料理相片集 |
| `events.html` | 活動消息 | 近期活動列表、電子報訂閱 |
| `contact.html` | 聯絡我們 | 聯絡資訊、留言表單、停車資訊 |
| `feedback.html` | 滿意度調查 | 內嵌 Google Forms 問卷 |

## GitHub Pages 部署方式

1. 在 GitHub 新建一個 Repository（例如 `dawn-restaurant`）
2. 將所有檔案上傳至該 Repository（保持資料夾結構）
3. 進入 Repository 的 **Settings** → **Pages**
4. Source 選擇 `Deploy from a branch`
5. Branch 選擇 `main`，資料夾選 `/ (root)`
6. 點擊 **Save**，等待約 1-3 分鐘

部署完成後，網站網址為：
```
https://[你的GitHub帳號].github.io/dawn-restaurant/
```

## 檔案結構

```
dawn-restaurant/
├── index.html
├── menu.html
├── story.html
├── reservation.html
├── gallery.html
├── events.html
├── contact.html
├── feedback.html
├── css/
│   └── style.css
├── js/
│   └── main.js
└── README.md
```

## 自訂說明

- **更換 Google Form**：在 `feedback.html` 找到 `<iframe>` 標籤，替換 `src` 屬性中的 URL
- **修改餐廳資訊**：各頁面中的地址、電話等資訊可直接編輯 HTML
- **新增真實圖片**：`gallery.html` 中的 emoji 佔位圖可替換為 `<img>` 標籤
- **字型**：使用 Google Fonts 的 Noto Serif TC（中文）及 Cormorant Garamond（西文）

## 技術規格

- 純靜態 HTML/CSS/JavaScript，無框架依賴
- 響應式設計，支援手機、平板、桌機
- 使用 CSS 變數管理色彩系統
- IntersectionObserver API 實現滾動動畫
