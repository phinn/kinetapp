# There's an AI for That — 提交备料(2026-11-13)

> **⛔ 2026-11-14 放弃:免费通道已关停。** 实测 `/submit/` 302 → `/launch/` 付费页
> ($49 起,唯一终点「Pay & Launch Tool」走 Stripe);`/create-tool/` 404 类重定向到搜索,
> `/create/` 是平台托管 mini-tool 非收录。备料保留作档案,若未来 TAAFT 恢复免费收录可复用。
> 免费目录替代:AlternativeTo(备料见 KinetAiosWin `PROMOTION_ALTERNATIVE.md`,注意 CF 挡自动化须用户手动)。

> 提交入口: https://theresanaiforthat.com/submit (免费,需注册账号;人工手贴,agent 不碰——同 PH 红线逻辑)
> 一次只提 1 款: KinetAios。其余 21 款是 utility(非 AI 站受众),提了 dilute 审核通过率,不提。

## 基本信息

- **Name**: KinetAios
- **Tagline** (≤60 chars): Local-first AI agent dashboard for macOS & Windows
- **Category**: Productivity → AI Agents
- **Pricing**: Paid ($12.99 one-time, Mac App Store) + Free open source (Windows/Linux CLI)
- **Platforms**: macOS, Windows
- **URL**: https://phinn.github.io/
- **GitHub**: https://github.com/phinn/KinetAios
- **App Store**: https://apps.apple.com/app/id6809450051

## One-liner (they often show this)

KinetAios is a local-first AI agent dashboard: multi-engine sessions (Claude Code, Codex, built-in Direct ReAct loop) with streaming answers, shell/file/web tools, SQLite long-term memory, and a global hotkey quick panel. No account, no cloud middleman — your keys, your data, your machine.

## Description (≤500 chars)

Most AI agent tools are a chat box bolted onto a terminal. KinetAios is a desktop dashboard built around them: pick an engine per conversation, watch tool calls and streaming tokens side by side, search every past turn with full-text memory, and summon it all with a global hotkey. The loop runs locally — API keys stay in your settings file, history stays in your SQLite. Open source core, native macOS app on the App Store, Windows build via winget.

## Key features (bullet list they may ask for)

1. Multi-engine: Claude Code, Codex CLI, and a built-in ReAct engine — switchable per conversation
2. Local-first: SQLite history + FTS5 recall; long-term memory extracted per turn
3. Native tools: shell (with approval gate), file read/write, web fetch
4. Global hotkey quick panel — agent answers without breaking your flow
5. Open source (MIT core) · 3,200+ clones · macOS & Windows

## Screenshot guidance

- 亮色暖纸白 UI 截图 1 张(铁律: 禁暗色)——用官网 og-image 风格: dashboard 主视图,能看到 streaming token + tool call 卡片
- 尺寸按他们上传器提示(一般 1200×750 或 16:10);已有 marketing/og-image.png (1200×630) 可微调
- Logo: 官网 favicon/512 版本

## Common review questions (预填答案)

- **Is it free?** Free trial via open source build; Mac App Store version $12.99 one-time.
- **What makes it different?** It's the only native-macOS GUI in the Claude Code client field that keeps sessions continuous across engines, and the whole loop runs on-device.
- **Who built it?** Solo developer (phinn), 22 apps on the App Store, all local-first. Site: https://phinn.github.io/

## 提交后动作

- 记录提交日期到 docs/upstream-pr-tracking.md(同 winget/awesome PR 追踪习惯)
- 通过后: phinn.github.io/index.html 的 press/cases 区不加(TAIft 是目录非 press);仅在 blog 新文或 X bio 变更时顺带提一句
