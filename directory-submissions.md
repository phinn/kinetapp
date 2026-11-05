# 目录站批量提交包(2026-11-05 实探版)

> 素材源:`/tmp/asc_live_apps.json`(20 在售 app,iTunes US 实时核对)。
> 四站实探结论 + 可直接粘贴的提交模板 + 人工执行清单。

---

## 一、通道现状(2026-11-05 实测)

| 站点 | 是否收费 | 是否有墙 | 提交入口 | 结论 |
|---|---|---|---|---|
| **MacUpdate** | 免费 | 无 CF 墙 | 登录后 https://www.macupdate.com/content/submit | ✅ 首批人工执行,难度最低 |
| **AlternativeTo** | 免费 | Cloudflare | 需注册+邮箱验证;登录后右上角用户菜单 → **Suggest new application**;给现有 app 加对手走 Contribute → Suggest Alternatives | ✅ 第二批,审核有 backlog |
| **Softpedia** | 免费 | Cloudflare(403) | https://www.softpedia.com/dynamic/submit-software.shtml | ✅ 第三批,过盾后人工填表 |
| **TAAFT** (theresanaiforthat) | **付费 $49 起**(50-100 点击/周) | Cloudflare | /launch/ 需登录+付费套餐 | ❌ 收费站一律不投(2026-11-05 定案),8 AI app≈$392 无验证 ROI,不碰 |

关键事实:
- MacUpdate 全站搜索 **零 kinet 收录** → 4 个 mac app 全是新提,无认领环节
- `phinn@outlook.com` 在 MacUpdate **已有账号**(注册报 email taken,密码未知) → 登录页走 **"Email me a Quick Sign In Link"**(magic link)即可,无需重置
- AlternativeTo 同理:先试已有账号,搜过 kinetbrief 无收录
- iOS 目录站(AppAdvice/148apps 类)已死或关闭提交,不投入

---

## 二、MacUpdate 提交模板(4 个 mac app,直接粘贴)

**通用字段**:开发者 Phinn / 公司 Kinet / 联系 phinn@outlook.com / 官网 https://phinn.github.io/kinetapp

### 1. KinetFlashFind: File Search
- Category: System Utilities → File Management
- Price: $6.99(买断,非订阅)
- Link: https://apps.apple.com/us/app/kinetflashfind-file-search/id6808698046
- Desc: Instant file search for Mac. FlashFind indexes your disk in seconds and finds files by name or content as you type — no waiting, no spinner. Local-first, nothing leaves your machine.

### 2. KinetAios: All-in-One AI Agent
- Category: Developer Tools → AI / System Utilities
- Price: $12.99(买断)
- Link: https://apps.apple.com/us/app/kinetaios-all-in-one-ai-agent/id6809450051
- Desc: Local-first AI agent dashboard for Mac. Multi-engine sessions (built-in ReAct engine, Claude Code, Codex), streaming answers, shell/file/web tools, SQLite history with long-term memory, global hotkey. Bring your own API key.

### 3. DriftDesk — Focus Ambience
- Category: Lifestyle → Other / System Utilities → Desktop
- Price: $4.99(买断)
- Link: https://apps.apple.com/us/app/driftdesk-focus-ambience/id6817377455
- Desc: Focus ambience for your desktop. DriftDesk layers procedural soundscapes and subtle motion wallpapers to help you sink into deep work — fully offline, zero accounts.

### 4. KinetMagicDisk: Disk Usage
- Category: System Utilities → Disk Management
- Price: $9.99(买断)
- Link: https://apps.apple.com/us/app/kinetmagicdisk-disk-usage/id6813423397
- Desc: See what's eating your disk. MagicDisk maps storage as a treemap you can act on — clean caches, duplicates and dead weight in a few clicks. Read-only by design; deletes only what you approve.

---

## 三、AlternativeTo 提交策略(重要:换打法)

AlternativeTo 是「替代品推荐」库 —— 直接 Suggest new application 审核慢且无替代语境。**优打法定成两步**:

1. **给现有大 app 加 alternative**(秒过审,借大 app 流量):
   - KinetAios → 在 `ChatGPT` 页 Suggest alternative(桌面 AI agent 对标)
   - KinetBrief / KinetMinutes → 在 `Otter.ai` 页 Suggest alternative(会议纪要)
   - KinetRain → 在 `Noisli` / `rainy mood` 页
   - DriftDesk → 在 `Noisli` 页;Clasp Focus → 在 `Forest` / `Focus To-Do` 页
   - KinetMagicDisk → 在 `DaisyDisk` 页;KinetFlashFind → 在 `EasyFind` 页
   - KinetMemory → 在 `Anki` 页;DuoFolio → 在 `KyBook` 页
   - KinetFit → 在 `Strong` / `Hevy` 页;KinetStudy → 在 `Photomath` 页
2. 大 app 全覆盖后,再统一 **Suggest new application** 补剩余(挂官网聚合页链接)

---

## 四、Softpedia 提交(4 mac 同模板,表单字段对齐 MacUpdate 版)

Softpedia 特色字段:平台选 **macOS**,分类按站内分类树选,「App Store link」栏直接填 apps.apple.com 链接(MAS 应用标注 MAS,免上传安装包)。提交后审核数日,收录页会回链 App Store。

---

## 五、人工执行清单(按序,约 40 分钟)

1. [ ] MacUpdate:https://member.macupdate.com → Sign in → **Email me a Quick Sign In Link**(phinn@outlook.com)→ 收邮件点链接登录
2. [ ] MacUpdate:逐个提交 4 个 mac app(模板照抄 § 二)
3. [ ] AlternativeTo:登录(试已有账号/magic link)→ 按 § 三打 11 个大 app 的 alternative(每个 30 秒)
4. [ ] Softpedia:过 CF 盾 → /dynamic/submit-software.shtml → 4 个 mac(§ 二文案复用);它本会自动爬 App Store,优先级最低
5. ~~TAAFT~~:付费站一律不投(定案)

## 六、验收口径

- 一周后逐站搜 `kinet` / 各产品名,记录收录 URL → 记进 promo 面板渠道清单
- 官网 analytics 看 directory 站 referrer 变化(基线:11-03 全站 313 uv)
- ~~TAAFT~~ **收费不投**(2026-11-05 用户定案:收费的都不投,连同未来任何 paid listing 通道)
