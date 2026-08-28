# MD Viewer 大师级宣传片制作实施计划

> **For agentic workers:** REQUIRED SUB-SKILL: Use superpowers:subagent-driven-development (recommended) or superpowers:executing-plans to implement this plan task-by-task. Steps use checkbox (`- [ ]`) syntax for tracking.

**Goal:** 打造 1080p@60fps 大师级 MD Viewer 品牌宣传片（约 48 秒），实现「静谧工匠 · 极简心流」艺术质感，去除一切 AI 生硬感。

**Architecture:** 采用全本地自动化管线：Playwright+CDP 60fps 真实客户端贝塞尔运镜采集、瑞士国际主义微光 HTML 卡片渲染、晓晓大气知性神经语音合成、电影级 Felt Piano + Ambient Pad 配乐引擎与 FFmpeg 广播级混缩合成。

**Tech Stack:** Node.js, Playwright, Chrome DevTools Protocol, msedge-tts, Web Audio/PCM Synth, ffmpeg-static, HTML5/CSS3.

---

### Task 1: 晓晓神经语音与气口时序合成系统 (`promo/voice_master.js`)

**Files:**
- Create: `promo/voice_master.js`
- Test Output: `promo/voice_master/*.mp3`, `promo/voice_master/lines.json`

- [ ] **Step 1: 编写 voice_master.js 脚本**
  - 实现 5 幕台词的神经语音合成（`zh-CN-XiaoxiaoNeural`，`rate: -4%`，`pitch: +0Hz`，加呼吸气口与留白）。
  - 精确测量每段 MP3 时长并输出 `lines.json` 供剪辑网格使用。

- [ ] **Step 2: 执行合成并验证音频文件完整性**
  - 运行 `node promo/voice_master.js`
  - 验证生成 5 段清晰、无截断的旁白音频。

---

### Task 2: 电影级 Ambient Felt Piano 配乐与 UI 触觉音效引擎 (`promo/music_master.js`)

**Files:**
- Create: `promo/music_master.js`
- Test Output: `promo/music_master.wav`

- [ ] **Step 1: 编写纯净电影级氛围音乐与拟真音效生成器**
  - 摒弃劣质蜂鸣器，采用多层泛音衰减的 Felt Piano 单音旋律 + 温暖立体声扩散的 Ambient Pad 弦波合成。
  - 生成全屏展开空气音（Glass Whoosh）、换向吸附微声（Tactile Snap）等 UI 触觉音效。

- [ ] **Step 2: 执行生成并验证配乐音质与时长**
  - 运行 `node promo/music_master.js`
  - 验证生成 48~52s 48kHz 16-bit 立体声 WAV 文件。

---

### Task 3: 瑞士国际主义排版卡片与微光字幕系统 (`promo/cards_master/`)

**Files:**
- Create: `promo/cards_master/title.html`
- Create: `promo/cards_master/caption.html`
- Create: `promo/cards_master/end.html`

- [ ] **Step 1: 编写序章黑曜石悬浮标题卡 `title.html`**
  - 黑曜石深色背景 (`#08090D`)、晨曦微光流转、纯粹瑞士排版与呼吸感留白。
- [ ] **Step 2: 编写极简底栏微光动态标注 `caption.html`**
  - 极简纤细字体、半透明环境光渐变底栏、优雅的 Ease-Out Expo 浮入与文字追踪。
- [ ] **Step 3: 编写尾幕毛玻璃终身买断卡 `end.html`**
  - 晶体毛玻璃 Pill 胶囊（14天免费试用 · 终身买断制）与 GitHub 官方链接。

---

### Task 4: 真实客户端 60fps 贝塞尔平滑运镜采集 (`promo/shoot_master.js`)

**Files:**
- Create: `promo/shoot_master.js`
- Output: `promo/shots_master/`

- [ ] **Step 1: 编写真实 Electron 应用 CDP 60fps 采集脚本**
  - ACT 1: 主窗口优雅居中悬浮升起。
  - ACT 2: 宏观平滑推入文档，平缓下滚展示公式、表格与代码高亮。
  - ACT 3: 点击架构图瞬间无缝全屏，210% 矢量无损缩放、平移漫游、一键 TD→LR 翻转与 ELK 重排。
  - ACT 4: 按下 F11 步入禅阅模式，版心舒展，明暗模式自如翻转。
- [ ] **Step 2: 执行采集并验证各幕镜头帧序列无死帧**
  - 运行 `node promo/shoot_master.js`
  - 确认生成 `b1_intro`, `b2_canvas`, `b3_diagram`, `b4_zen`, `b5_outro` 对应帧序列。

---

### Task 5: 60fps 透明通道卡片与字幕帧渲染 (`promo/shoot_cards_master.js`)

**Files:**
- Create: `promo/shoot_cards_master.js`
- Output: `promo/shots_master/cards/`

- [ ] **Step 1: 编写 Headless Chromium 逐帧卡片渲染脚本**
  - 60fps 逐帧捕获 `title.html`, `caption.html` 序列与 `end.html`。
- [ ] **Step 2: 执行渲染并验证透明通道帧序列**
  - 运行 `node promo/shoot_cards_master.js`。

---

### Task 6: 广播级 60fps 混缩与母带合成管线 (`promo/assemble_master.js`)

**Files:**
- Create: `promo/assemble_master.js`
- Output: `promo/md-viewer-promo-master.mp4`

- [ ] **Step 1: 编写多轨精准对位与母带合成脚本**
  - 按配音与呼吸节奏网格无缝拼接 5 幕镜头。
  - 多轨音频混缩：晓晓旁白 + 电影级配乐（带 Sidechain 智能避让）+ UI 触觉音效。
  - 广播级响度标准化：`-14 LUFS`，`-1.5 dBTP`。
  - 导出规格：1080p@60fps H.264 High Profile (yuv420p) + AAC 192k + `+faststart`。
- [ ] **Step 2: 执行最终母带合成**
  - 运行 `node promo/assemble_master.js`。

---

### Task 7: 审片质检与最终交付

**Files:**
- Output: `promo/md-viewer-promo-master.mp4`
- Summary Report: `promo/MASTER_REVIEW.md`

- [ ] **Step 1: 全片均匀抽帧核验**
  - 检查折行、文字清晰度、图表矢量放大、全屏过渡与尾幕 CTA。
- [ ] **Step 2: 验证全端兼容性与音画完美同步**
