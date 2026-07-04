# Brag Plan: AURA X — 超越所見。

## What is this app?
一頁式旗艦手機發表會網站：scroll-driven Three.js 3D 鈦金屬手機（純 primitives、零模型素材）、鏡頭模組捲動展開、hotspot 規格卡、即時換色配置器、AI 生成樣張——全部裝在一個 `index.html` 裡。這是 Harry 的作品集作品。

## The angle
「一場旗艦手機發表會，只需要一個 HTML 檔案。」
以假亂真的 keynote 質感產品片——觀眾先以為在看手機廣告，最後才發現這是一個網頁作品。雙重炫耀：產品片本身美，且它宣傳的東西是「我寫的網站」。

## Hook (first 2-3 seconds)
純黑。等寬字體 cyan kicker「INTRODUCING AURA X」逐字打出，接著巨型繁中標題「超越所見。」重擊入場，光暈一閃。前 2 秒就是發表會開場的儀式感。

## Key moments (the middle)
- 真實網站 hero 截圖（3D 鈦金手機 + cyan 光）緩慢推近——展示 WebGL 手機是「畫」出來的。
- 相機規格三連發：`1"` 感光元件 / `ƒ/1.6` 光圈 / `5×` 光學變焦，逐一貼著節拍入場。
- 四張 AI 樣張快切（夜景→人像→望遠→微距），各帶等寬字幕 cap（NIGHT MODE · ISO 800…）。

## Outro / punchline
「這不是手機廣告。是一個網頁。」→ AURA X wordmark + 「作品 · harryfan.github.io/blog」。
最後一拍讓觀眾意識到整支片在炫網站。

## User flow worth showing
none — landing-page only。但有互動亮點：配色 swatch 即時換色 + 樣張 tab 切換。樣張快切場景即代表 tab 互動；換色若素材允許以兩張不同主題截圖對切呈現。

## Tone
- Preset: cinematic
- Creative direction: 旗艦手機 keynote 產品片，最後一秒揭穿是網頁作品
- Interpretation: 大字、深黑底、克制的鏡頭推移與硬切；文字少而大，每句話都停得夠久；能量來自節拍對齊的入場而非閃爍。

## Format: vertical — 1080x1920
（主戰場是小紅書/短影音，直式優先。）

## Duration: 20s

## Visual identity (from the project)
- Background: #08090C（--bg），次層 #14161B
- Accent: #45D6FF（cyan），輔助 #58E6A9（success green）
- Text: #FFFFFF，次要 rgba(255,255,255,.7)
- Display font: -apple-system / Noto Sans TC 粗黑體（800，letter-spacing -0.02em）
- Mono font: SF Mono / JetBrains Mono（kicker 與規格數字用）
- Strongest visual element: 3D 鈦金手機 hero + cyan glow；grid overlay（72px 網格線）可作背景質感
- 浮水印：右下角固定「harryfan.github.io/blog」（mono, 小字, 40% 白）全片常駐

## Share copy (draft)
一個 HTML 檔案，裝下一場旗艦手機發表會——3D 手機、捲動運鏡、換色配置器，全部手寫。AURA X，我的新作品。

## Audio direction
- Role: cinematic support——節拍感的premium bed，撐住 keynote 儀式感
- Music: happy-beats-business-moves-vol-9（114.84 BPM，唯一 bundled 曲風中最穩的律動）
- Music treatment: 0s 進、-14dB 姿態、最後 1.5s fade out；大場景切換落在 strong cue
- Music cue guidance: preset 已讀（vol-9）。strong cues：3.70s（標題重擊）、10.54s（樣張快切開始）、15.28s 附近（揭穿卡入場）。sequential 規格三連發用 beat grid 6.34 / 7.40 / 8.44（隔拍，留讀秒）
- Audio-reactive treatment: subtle——cyan glow 隨低頻呼吸，不加波形條
- SFX posture: sparse、motion-matched：打字聲（hook kicker）、低沉 impact（標題）、輕 UI tick（規格入場）、快門聲（樣張切換）
- Audio-coupled moments: kicker 逐字打出、規格三連發隔拍入場、樣張快切對節拍
- Restraint rule: 不用 riser 疊 riser；SFX 音量低於音樂；揭穿卡之後不再加任何 SFX

## Storyboard

### Scene 1 — 開場 hook — 3.7s
純黑 + 微弱 72px 網格。mono cyan「INTRODUCING AURA X」逐字打出（~1s），2 秒處巨型「超越所見。」硬入 + glow 閃一下，穩住到 3.7s。
Sequential/interaction: yes — kicker 逐字打字
Audio intent: 安靜開場 → 3.70s strong cue 標題重擊
Audio-coupled idea: 打字 key ticks；標題落點對 3.70s cue + impact
Music: bed 低姿態進場
Transition mood: hard cut → Scene 2

### Scene 2 — 手機亮相 — 3.3s（3.7–7.0s）
真實 hero 截圖（3D 鈦金手機、cyan 光）滿版，緩慢 scale 1.0→1.06 推近。下三分之一疊字：「鈦金屬工藝 × 1 吋感光元件 × A1X 晶片」（停 ≥2s）。
Sequential/interaction: none
Audio intent: 開闊、premium
Audio-coupled idea: glow 隨低頻subtle呼吸
Music: bed 持續
Transition mood: clean wipe → Scene 3

### Scene 3 — 規格三連發 — 3.5s（7.0–10.5s）
深黑底，三枚 mono 大數字規格 chip 逐一入場（各隔一拍：~7.40 / 8.44 / 9.50）：`1"` 感光元件 → `ƒ/1.6` 主鏡光圈 → `5×` 光學變焦。全部到齊後合停 ~1s。
Sequential/interaction: yes — 三 chip 隔拍逐一入場，each with UI tick
Audio intent: 節奏感、精準
Audio-coupled idea: 每 chip 對 beat grid（隔拍留讀秒）
Music: bed 持續
Transition mood: hard cut → Scene 4

### Scene 4 — 樣張快切 — 4.5s（10.5–15.0s）
從 10.54s strong cue 起，四張真實樣張快切（夜景 1.3s → 人像 1.1s → 望遠 1.1s → 微距 1.0s），每張左下 mono cap（NIGHT MODE · ISO 800 · 1/8s…）。頂部小標「Shot on AURA X」常駐。
Sequential/interaction: yes — 四連快切，每切一聲快門
Audio intent: 高潮段，切點貼拍
Audio-coupled idea: 快門 SFX 對切點
Music: bed 持續（能量最高段）
Transition mood: dramatic → Scene 5

### Scene 5 — 揭穿 + 署名 — 5.0s（15.0–20.0s）
黑底。第一行：「這不是手機廣告。」（停 1.2s）第二行接上：「是一個網頁。」（停 1.2s）淡入 AURA X wordmark（AURA cyan + X 白）與「作品 · harryfan.github.io/blog」。音樂 18.5s 起 fade。
Sequential/interaction: yes — 兩行文案先後入場
Audio intent: 收束、留白
Audio-coupled idea: 第二行落在 ~15.28s 附近 cue；之後無 SFX
Music: fade out 最後 1.5s
Transition mood: soft fade to black → end

**Music mood for this video:** cinematic-upbeat（vol-9）
**Audio summary:** 低姿態 bed 進場 → 3.7s 標題重擊 → 規格隔拍三連 → 樣張貼拍快切最高潮 → 揭穿卡收音樂淡出，全程 SFX 稀疏貼動作。

（場景合計：3.7 + 3.3 + 3.5 + 4.5 + 5.0 = 20.0s ✓）
