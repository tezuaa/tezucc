+++
date = '2026-02-13T02:50:00+08:00'
draft = false
title = 'x2md：讓推文成為你筆記的一部分'
slug = 'project-x2md-intro'
categories = ['project']
tags = ['chrome-extension', 'tools', 'markdown', 'twitter']
description = '一個輕量級的 Chrome Extension，讓你一鍵將 X (Twitter) 推文保存為 Markdown，無縫整合到你的 Obsidian 或 Notion。'
image = ''
+++

在這個資訊碎片化的時代，X (Twitter) 往往是靈感與新知的源頭。
但要將這些有價值的推文保存下來，往往需要繁瑣的複製貼上，或者依賴不穩定的第三方服務。

於是，**x2md** 誕生了。

下載連結 [https://github.com/tezuaa/x2md](https://github.com/tezuaa/x2md)

這是一個極簡主義的 Chrome Extension，它的目標只有一個：
**讓保存推文變得像點個讚一樣簡單。**

## 核心功能

安裝後，你會在每一條推文的 Action Bar（按讚、轉推那排）旁邊，發現一個新的「💾」按鈕。

點擊它，這條推文就會瞬間變成一個格式完美的 `.md` 檔案下載到你的電腦裡。
檔名就是推文的 ID，確保唯一性且易於索引。

## Markdown 格式預覽

下載下來的 Markdown 檔案會長這樣：

```markdown
# Tweet by @username

> 這是推文的內容...
> 這裡可能還有第二行...

- **Author**: Display Name (@handle)
- **Date**: 2026-02-13
- **Tweet URL**: https://x.com/username/status/123456
- **Images**:
  ![](https://pbs.twimg.com/media/...)
```

這樣的格式，可以直接拖進 Obsidian、Notion 或任何支援 Markdown 的筆記軟體中，瞬間成為你知識庫的一部分。

## 技術實現 (Under the Hood)

這是一個純粹的瀏覽器擴充功能，沒有後端伺服器，不蒐集任何數據。

- **Manifest V3**：採用最新的 Chrome 擴充標準，安全、輕量。
- **MutationObserver**：因為 X 是一個 SPA (Single Page Application)，推文是動態載入的。我們使用 DOM 監聽技術，確保即使你無限捲動，按鈕也會準確地出現在每一條新載入的推文旁。
- **Zero Permissions**：不需要讀取你的瀏覽紀錄，也不需要特殊的權限。所有的下載動作都是透過瀏覽器原生的 Blob URL 技術在本地完成的。

## 如何使用

目前專案已開源，你可以手動安裝體驗：

1.  下載專案原始碼。
2.  在 Chrome 打開 `chrome://extensions/`。
3.  開啟右上角的「開發者模式」。
4.  點擊「載入未封裝項目」，選擇 `x2md` 資料夾。
5.  前往 [x.com](https://x.com)，開始你的收藏之旅。

不再讓靈感在 Timeline 中流失。
**x2md**，為你的知識庫捕獲每一隻飛過的藍鳥。
