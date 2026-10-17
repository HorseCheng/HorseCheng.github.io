# HorseCheng · Vibe Coding 作品集

用 AI 協作（vibe coding）做出來、實際上線的網站作品集。純靜態頁面（單一 `index.html`），直接用 GitHub Pages 發佈。

## 收錄作品

| 作品 | 說明 | 網址 |
|---|---|---|
| LibriAI | 書籍／漫畫／小說閱讀追蹤 | https://libriai-1044062718546.us-west1.run.app/ |
| CineAI | 電影／影集／動漫追蹤 | https://cineai-1044062718546.us-west1.run.app/ |
| News Feed | AI 新聞聚合閱讀器 | https://news-feed-horsecheng.web.app/ |
| Portfolio Tracker | 股票資產管理 | https://stock-horsecheng.web.app/ |
| 日語學習平台 | JLPT N5–N3 | https://japanese-learning-horsecheng.web.app/ |
| 寶可夢卡牌抽獎所 | 抽卡模擬器 | https://ptcg-gacha-horsecheng.web.app/ |
| AI 日報 | ChatGPT Dot 每日 08:00 自動更新 | https://llm-daily-tw.horsecheng.chatgpt.site/ |
| Pokémon GO 活動筆記 | ChatGPT Dot 每日 08:00 自動更新 | https://pokemon-go-event-fieldnotes.horsecheng.chatgpt.site/ |
| Pokémon Sleep 睡眠研究筆記 | ChatGPT Dot 每日 08:00 自動更新 | https://pokemon-sleep-fieldnotes.horsecheng.chatgpt.site/ |

## 結構

```
index.html            整個網站（CSS / JS 內嵌）
assets/favicon.svg
assets/shots/*.webp   各網站截圖
```

## 發佈到 GitHub Pages

1. 在 GitHub 建立名為 `<你的帳號>.github.io` 的 repo（這樣網址就是 `https://<你的帳號>.github.io/`）。
2. 推上去：
   ```bash
   git init
   git add .
   git commit -m "Initial portfolio"
   git branch -M main
   git remote add origin https://github.com/<你的帳號>/<你的帳號>.github.io.git
   git push -u origin main
   ```
3. Repo → Settings → Pages → Source 選 **Deploy from a branch**，Branch 選 `main` / `(root)`。

## 新增作品

複製 `index.html` 裡任一個 `<article class="app">`（全端應用）或 `<a class="card">`（自動化資訊站）區塊，改掉文字、連結、截圖和 `--c` 主題色。截圖放在 `assets/shots/`，建議寬度約 1500px、WebP 格式。
