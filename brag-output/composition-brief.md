# Hyperframes Composition Brief: AURA X

## Objective
Create a short launch-style brag video for AURA X — a scroll-driven 3D flagship-phone landing page that is Harry's portfolio piece.

## Output
- Composition directory: `brag-output/composition/`
- Rendered video: `brag-output/brag.mp4`
- Format: vertical — 1080x1920
- Duration: 20 seconds

## Source Material
- Project root: /Users/gangshuanfan/Documents/github/claude-mobile
- Primary files read: index.html (single-file site; Three.js phone from primitives)
- Product name: AURA X
- Tagline / strongest claim: 超越所見。／這不只是一支手機，是你口袋裡的旗艦。
- Key UI or visual moment to recreate: real hero screenshot with the 3D titanium phone (capture at scratchpad caps/hero-v.png, 1080x1920)
- Copy that must appear verbatim (Traditional Chinese — user override of the Simplified-Chinese default):
  - INTRODUCING AURA X
  - 超越所見。
  - 鈦金屬工藝 × 1 吋感光元件 × A1X 晶片
  - 這不是手機廣告。／是一個網頁。
  - harryfan.github.io/blog

## Creative Direction
- Tone preset: cinematic
- Creative direction: 旗艦手機 keynote 產品片，最後一秒揭穿是網頁作品
- Interpretation: 大字深黑、克制推移、硬切；每句話停足讀秒；能量來自貼拍入場
- Angle: 「一場旗艦手機發表會，只需要一個 HTML 檔案。」觀眾先以為在看手機廣告，最後發現是網頁作品——雙重炫耀。
- Hook: 黑幕 mono cyan kicker 逐字打出 → 巨型「超越所見。」重擊
- Outro / punchline: 「這不是手機廣告。是一個網頁。」→ AURA X wordmark + 署名
- Avoid: generic SaaS language, abstract filler, redesigning the site's visual identity

## Visual Identity
- Background: #08090C (secondary #14161B)
- Text: #FFFFFF / rgba(255,255,255,.7)
- Accent: #45D6FF (support #58E6A9)
- Display font: -apple-system / "Noto Sans TC" weight 800, letter-spacing -0.02em
- Mono font: "SF Mono", ui-monospace (kickers, spec digits, caps)
- Visual references: 72px grid overlay at 2.5% white; cyan glow; pill buttons; watermark bottom-right "harryfan.github.io/blog" in mono 10px persists through the whole video

## Assets available (already on disk)
- caps/hero-v.png — real site hero, 3D phone, 1080x1920 (scratchpad caps dir; copy into composition/assets/img/)
- caps/camera-v.png — lens module close-up, 1080x1920
- assets/sample-night.jpg, sample-portrait.jpg, sample-tele.jpg, sample-macro.jpg — 16:9 sample photos (project assets/)

## Storyboard (contract = brag-output/brag-plan.md)
1. 開場 hook — 3.7s — kicker types out; 「超越所見。」slams at 3.70s cue; grid bg
2. 手機亮相 — 3.3s — hero-v.png full-bleed, scale 1.0→1.06; caption 鈦金屬工藝 × 1 吋感光元件 × A1X 晶片 (hold ≥2s)
3. 規格三連發 — 3.5s — `1"` 感光元件 / `ƒ/1.6` 主鏡光圈 / `5×` 光學變焦, one per ~beat (7.40/8.44/9.50), settle together ~1s
4. 樣張快切 — 4.5s — 4 sample photos hard-cut from 10.54s cue; mono caps bottom-left; top label "Shot on AURA X"
5. 揭穿 + 署名 — 5.0s — 「這不是手機廣告。」(1.2s hold) →「是一個網頁。」(1.2s hold) → AURA X wordmark + 作品 · harryfan.github.io/blog; music fades from 18.5s

## Audio
- Audio role: cinematic support
- Audio arc: low bed in → title hit 3.70s → beat-spaced spec chips → photo cuts on beats → fade under credits
- Music: happy-beats-business-moves-vol-9-by-ende-dot-app.mp3 (114.84 BPM)
- Music treatment: start 0s, volume 0.35, afade out last 1.5s
- Music cue guidance: bundled preset assets/music/cues/happy-beats-business-moves-vol-9-by-ende-dot-app.music-cues.json; strong cues 3.70 / 10.54 / 15.28; beat grid 7.40 / 8.44 / 9.50 for spec chips (every-other-beat spacing for readable text)
- Audio-reactive treatment: subtle — cyan glow breathes with bass; no waveform visuals; skip if extraction unavailable (document it)
- Audio-coupled moments:
  - Scene 1 — kicker typing (keyboard/keypress-*.wav randomized) + title hit (impact/impactBell_heavy_000)
  - Scene 3 — spec chips (interface/drop_* one per chip)
  - Scene 4 — photo cuts (camera-shutter-like: interface/click_* or casino/card-place)
  - Scene 5 — second line lands near 15.28s cue; no SFX after credits appear
- SFX selection guidance: cinematic = 2-3 big ones + sparse ticks; consult sfx-analysis.md; prefer low HF-risk
- Exact SFX choice: Hyperframes decides filenames/timestamps/volumes from implemented motion
- Audio files: copy chosen music + SFX into brag-output/composition/assets/

## Hyperframes Instructions
Per current hyperframes skill. Requirements: real hero screenshot must appear; all text readable (0.3s/word, min 1.2s); 20s total; lint + validate must pass; local assets only; deterministic timeline (paused master timeline, no Date.now/random/RAF-driven state).
