# ART WORKER — Electric Shock Pose Detection

# ART WORKER — 电击姿态检测

---

## English

A browser-based interactive art piece that uses your webcam to detect human poses and overlays a glowing skeleton. Every few seconds, it simulates a high-voltage electric shock: the canvas shakes, the skeleton jitters, white lightning arcs crackle between joints, and a synthesized zap sound plays.

### Features

- Real-time multi-person pose detection (MoveNet via TensorFlow.js)
- Skeleton overlay with head box and "ART WORKER" label
- Periodic electric shock simulation (adjustable interval, default 2s)
- Visual effects: white lightning, canvas shake, skeleton jitter, white flash
- Synthesized electric zap sound (Web Audio API)
- Camera switching (front/back) for mobile
- Sound toggle and manual shock test

### Controls

- **Sound ON/OFF** — toggle audio
- **Front/Back camera** — switch camera (mobile)
- **Interval slider** — set shock interval (2–20s)
- **Test shock** — trigger a shock immediately

### How to Use

1. Open the HTML file in a modern browser (Chrome, Safari, etc.).
2. Allow camera access.
3. Stand in frame and watch the skeleton. Shocks occur automatically.
4. Use the controls to adjust settings.

### Technical

- TensorFlow.js + MoveNet (MULTIPOSE_LIGHTNING)
- Web Audio API for synthesized zap
- Canvas 2D rendering
- No build step; just a single HTML file.

### Customization

- `SHOCK_DURATION_MS` (default 700) — how long each shock lasts.
- `shockIntervalMs` (default 2000) — time between shocks.
- `mirror` — automatically set based on camera facing (front mirrored, back un-mirrored).

### Credits

Pose detection by TensorFlow.js MoveNet. Synthesized sound and visual effects original.

---

## 中文

一个基于浏览器的互动艺术作品：使用摄像头检测人体姿态，并叠加发光骨架。每隔几秒模拟一次高压电击：画布震动、骨架抖动、白色闪电在关节间劈啪作响，并播放合成电击音效。

### 功能

- 实时多人姿态检测（基于 TensorFlow.js 的 MoveNet）
- 骨架叠加、头部框和 "ART WORKER" 标签
- 周期性电击模拟（间隔可调，默认 2 秒）
- 视觉效果：白色闪电、画布震动、骨架抖动、白光闪烁
- 合成电击音效（Web Audio API）
- 摄像头切换（前置/后置），适用于手机
- 声音开关和手动电击测试

### 控件

- **声音开/关** — 切换音频
- **前置/后置摄像头** — 切换摄像头（手机）
- **间隔滑块** — 设置电击间隔（2–20 秒）
- **测试电击** — 立即触发电击

### 使用方法

1. 在现代浏览器中打开 HTML 文件（Chrome、Safari 等）。
2. 允许摄像头访问。
3. 站在画面中，观察骨架。电击会自动发生。
4. 使用控件调整设置。

### 技术

- TensorFlow.js + MoveNet（MULTIPOSE_LIGHTNING）
- Web Audio API 合成电击音效
- Canvas 2D 渲染
- 无需构建步骤；单个 HTML 文件。

### 自定义

- `SHOCK_DURATION_MS`（默认 700）— 每次电击持续时间。
- `shockIntervalMs`（默认 2000）— 电击间隔时间。
- `mirror` — 根据摄像头朝向自动设置（前置镜像，后置不镜像）。

### 致谢

姿态检测由 TensorFlow.js MoveNet 提供。合成音效和视觉效果为原创。
