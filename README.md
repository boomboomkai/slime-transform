# 史萊姆變身記

像素風格的動作 RPG。你是一隻藍色小史萊姆，打倒怪物學會牠們的技能，打滿數量就能變身成那種怪物。

整個遊戲只有一個 `index.html`，不需要安裝或建置，用瀏覽器打開就能玩，手機和電腦都支援。

## 遊戲特色

- **5 個章節、50 個小節**：每個小節都有不同的怪物和 BOSS，打贏才能解鎖下一關
- **變身系統**：5 種怪物形態，各有 3 個技能和 1 個終極技能
- **裝備掉落**：12 個裝備欄位，白、綠、藍、紫、橘五種稀有度，傳說裝備有特殊被動
- **強化與鑲嵌**：裝備最高 +15，6 種寶石可以合成升級
- **大地圖與戰爭迷霧**、小地圖、世界地圖傳送
- **自動戰鬥**、成就系統、商店與永久強化、新手教學
- 即時合成的 8-bit 背景音樂與音效

## 操作

| | 手機 | 電腦 |
|---|---|---|
| 移動 | 左半邊拖曳 | WASD／方向鍵 |
| 攻擊 | 按住「攻擊」 | J／空白鍵 |
| 技能 | 點技能按鈕 | 1～5 |
| 藥水 | 點紅、藍瓶 | Q／E |
| 自動戰鬥 | 「自動」按鈕 | R |
| 裝備／物品／變身／選單 | 右上角按鈕 | I／O／T／M |

## 在本機遊玩

直接用瀏覽器打開 `index.html` 即可。

## 發佈到 GitHub Pages

1. 在 GitHub 建立一個新的 repository（例如 `slime-transform`）
2. 把這個資料夾裡的檔案上傳（或用 git push）到 repository 的 `main` 分支
3. 到 repository 的 **Settings → Pages**
4. **Source** 選 **Deploy from a branch**，Branch 選 `main`、資料夾選 `/ (root)`，按 **Save**
5. 等一兩分鐘，遊戲網址會是 `https://<你的帳號>.github.io/<repository 名稱>/`

用指令上傳：

```bash
cd slime-transform
git init
git add .
git commit -m "史萊姆變身記"
git branch -M main
git remote add origin https://github.com/<你的帳號>/slime-transform.git
git push -u origin main
```

## 存檔

進度存在瀏覽器的 localStorage，換瀏覽器或清除網站資料會重新開始。

## 技術

純 HTML、CSS、JavaScript（Canvas 2D 繪圖、Web Audio 即時合成聲音），沒有使用任何框架。字型使用 Google Fonts 的 DotGothic16，沒有網路時會改用系統字型。
