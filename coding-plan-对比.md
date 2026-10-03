# AI Coding Plan 对比（2026-10 更新版）

> 本文件为 **2026-10-04** 更新的各厂商 AI 编程订阅（Coding Plan）横向对比。
> 相较 8 月的老版本，**已补充 GPT-6（Astra/Sol/Luna）与 Claude Opus 5.5 等新旗舰模型**，并更新了各家最新档位价格与额度口径。
> 数据来源：各平台官方定价页 + codingplan.org（2026-09 横评）交叉核对。**价格与额度变动频繁，购买前务必以官方页面为准。**

## 一、速览对比表

| 平台 | 起步价 | 主流档位 | 核心模型（2026-10） | 额度口径 | 备注 |
| --- | --- | --- | --- | --- | --- |
| **ChatGPT (OpenAI)** | $8/月 (Go) | Plus $20 / Pro $100–200 | **GPT-6 Astra** · GPT-6 Sol · GPT-6 Luna · GPT-5.6 Sol | 套餐消息 / Codex 额度 | Pro $200 档新购暂停 |
| **Claude (Anthropic)** | $20/月 (Pro) | Max 5x $100 / Max 20x $200 | **Opus 5.5** · Fable 5.1 · Sonnet 5 · Haiku 4.5 | Pro 5× / Max 5×–20× | 含 Claude Code CLI |
| **阿里云百炼** | ¥39/月 (Lite) | Standard ¥139 / Pro ¥499 | Qwen3.8-Max (0902) · Qwen3.8-Flash · Kimi-K3 · Deepseek-v4-pro | 11,500–180,000 Credits/月 | 12 项 Harness 权益 |
| **OpenCode Go** | $10/月 | 单档 | GPT-6 Luna · DeepSeek V4.1 Flash · Kimi K3 · GLM-5.3-Flash · MiMo-V2.6-Flash · MiniMax M3 | 5h $12 / 周 $30 / 月 $60 | 32 款模型，6× 用量 |
| **智谱 GLM** | ¥118/月 (Lite) | Pro ¥538 / Max ¥1078 | GLM-5.3 · GLM-5.3-Flash | 5h 2000/12000/28000 · 周 10K/60K/140K 积分 | 支持 20+ 工具 |
| **MiniMax** | ¥49/月 (Plus) | Max ¥119 / Ultra ¥469 | MiniMax M3 · M2.7 · H3 · Speech 2.8 | 6亿–71亿+ token/月 | 全模态共享额度 |
| **Kimi** | ¥99/月 (Plus) | Pro ¥199 / Max ¥699 | Kimi K3 (2.8T / 1M) · K2.8 Preview · K2.7 Code 高速版 | 5h 滚动窗口（取消周限额） | Go ¥49 不含编程额度 |
| **火山引擎方舟** | ¥9.9 首购 Lite | Pro 首购 ¥49.9 | DeepSeek-V4.1-Flash · GLM-5.3 系列 · Doubao-Seed-Evolving · Kimi-K3 · MiniMax-M3 | Lite / Pro 月额度 | 2.5 折活动至 2026-11-08 |
| **小米 MiMo** | ¥39/月 (Lite) | Standard ¥99 / Pro ¥329 / Max ¥659 | MiMo-V2.6 系列 · MiMo-V2.6-Flash · MiMo TTS | 492–9,840 亿 Credits/年 | 无周限额 / 5h 限额 |

**其他可选**：NVIDIA NIM（免费，开源模型最高 40 rpm）、Ollama Pro（$20/月，含 $60 用量）、Google AI Ultra（$100/$200）、Fireworks Fire Pass、OpenRouter（部分模型 50 reqs/天免费）。

---

## 二、头部厂商详览（含 GPT-6 与 Opus 5.5）

### Claude（Anthropic）—— Opus 5.5 已上线

2026-10 最新模型阵容：**Opus 5.5**（新旗舰，agentic coding 定位）、Fable 5.1、Sonnet 5、Haiku 4.5。

| 档位 | 价格 | 说明 |
| --- | --- | --- |
| Free | $0 | 基础额度 |
| Pro | $20/月（年付约 $17/月） | Opus 5.5 / Sonnet 5 / Haiku 4.5 可用；Fable 5.1 按 Usage credits 额外计费；含 Claude Code CLI；上下文最高 1M |
| Max 5x | $100/月 | 5× Pro 用量；Fable 5.1 最多用周额度 50%；高峰优先 |
| Max 20x | $200/月 | 20× Pro 用量；同上 |

- **Opus 5.5**：1M 上下文、128K 最大输出，API 价约 $4–8 / $20–40（MTok），知识截止 2026-06。
- 额度口径：Pro 5× / Max 5×–20×，5 小时 + 周双窗口。

### ChatGPT（OpenAI）—— GPT-6 系列已上线

2026-10 最新模型阵容：**GPT-6 Astra**（最强）、GPT-6 Sol、GPT-6 Luna，另有 GPT-5.6 Sol。

| 档位 | 价格 | 说明 |
| --- | --- | --- |
| Go | $8/月 | GPT-6 Luna（桌面端），高于免费版 10 倍消息额度 |
| Plus | $20/月 | GPT-6 Sol（ChatGPT Work + Codex）；GPT-6 Astra 分批开放 |
| Pro | $100–200/月 | $100 档：unlimited GPT-6 Astra、优先级、更快；$200 档新购暂停 |

- **GPT-6 Astra**：API 价 $10/$50（MTok），1.05M 上下文，128K 输出，知识截止 2026-04。
- **GPT-6 Luna**：API 价 $0.10/$0.50（MTok），高性价比。

---

## 三、国内厂商详览

### 阿里云百炼 Token Plan

| 档位 | 价格 | 额度 | 特点 |
| --- | --- | --- | --- |
| Lite | ¥39/月 | 11,500 Credits/月 | 1–2 Agent 并发；夜间 22:00 起限时 4 折 |
| Standard | ¥139/月 | 45,000 Credits/月（≈4× Lite） | 3–4 Agent 并发；12 项 Harness |
| Pro | ¥499/月 | 180,000 Credits/月 | 6–8 Agent 并发；超额 88 折 |

模型：Qwen3.8-Max (0902)、Qwen3.8-Flash、Kimi-K3、Deepseek-v4-pro、Qwen3-VL-Plus、Qwen-Image-3.0-Pro。

### 智谱 GLM Coding Plan（连续包月价）

| 档位 | 价格 | 5h/周积分 | 说明 |
| --- | --- | --- | --- |
| Lite | ¥118/月（年付 ¥94.4） | 2,000 / 10,000 | GLM-5.3 / 5.3-Flash 全档可用 |
| Pro | ¥538/月（年付 ¥430.4） | 12,000 / 60,000 | 更快生成 + 高峰保障 |
| Max | ¥1078/月（年付 ¥862.4） | 28,000 / 140,000 | 最新旗舰优先、专属资源 |

模型：GLM-5.3（1M 上下文）、GLM-5.3-Flash。支持 ZCode / Claude Code 等 20+ 工具。

### MiniMax Token Plan

| 档位 | 价格 | 额度 | 说明 |
| --- | --- | --- | --- |
| Plus | ¥49/月 | 6亿+ token/月 | 3–4 Agent 并发 |
| Max | ¥119/月 | 18亿+ token/月 | 4–5 Agent；Hailuo 视频 3 条/日 |
| Ultra | ¥469/月 | 71亿+ token/月 | 6–7 Agent；Hailuo 视频 5 条/日 |

模型：MiniMax M3、M2.7、H3（已开源）、Speech 2.8，全模态共享额度。

### Kimi Code Plan（新会员体系）

| 档位 | 价格 | 说明 |
| --- | --- | --- |
| Go | ¥49/月（年付 ¥39） | 不含编程额度 |
| Plus | ¥99/月（年付 ¥79） | Kimi Code 可用；K3 旗舰 |
| Pro | ¥199/月（年付 ¥159） | K3 解锁 1M 上下文；K2.7 Code 高速版 |
| Max | ¥699/月（年付 ¥559） | 14× Agent 额度；Kimi Claw；100 项目 / 50GB |

模型：Kimi K3（2.8T / 1M）、K3-256K、K2.8 Preview、K2.7 Code 高速版。**新会员取消每周额度限制**，保留 5h 滚动窗口。

### 火山引擎方舟 Coding Plan

| 档位 | 刊例价 | 活动价 | 说明 |
| --- | --- | --- | --- |
| Lite | ¥40/月 | 首购 ¥9.9（前两月） | 个人轻量 |
| Pro | ¥200/月 | 首购 ¥49.9（前两月） | 5× Lite 用量 |

模型：DeepSeek-V4.1-Flash、GLM-5.3 系列、Doubao-Seed-Evolving、Kimi-K3、Kimi-K2.8-Preview、MiniMax-M3，支持 Auto 模式。活动至 2026-11-08，名额有限。

### 小米 MiMo Coding Plan（V2.6 系列）

| 档位 | 价格 | 额度（Credits/年） | 说明 |
| --- | --- | --- | --- |
| Lite | ¥39/月（年付 88 折） | 492 亿 | 夜间 0.8× 消耗 |
| Standard | ¥99/月 | 1,320 亿 | 2.7× Lite |
| Pro | ¥329/月 | 4,560 亿 | 9.3× Lite |
| Max | ¥659/月 | 9,840 亿 | 20× Lite；团队/发烧友首选 |

模型：MiMo-V2.6 系列、MiMo-V2.6-Flash、MiMo TTS。**无周限额与 5h 限额**。

---

## 四、选购建议（基于 2026-10 数据）

- **性价比 / 按量**：DeepSeek V4 Flash 按用量计费通常比多数 Coding Plan 便宜；OpenCode Go（$10/月）以 6× 用量 + 32 模型成为性价比标杆。
- **旗舰模型体验**：偏好最强闭源模型选 **Claude Max（Opus 5.5）** 或 **ChatGPT Pro（GPT-6 Astra）**；两者 $100/$200 档位互相对标。
- **团队 / 并发**：Kimi Max、智谱 GLM Pro/Max、阿里云百炼 Pro 各有侧重，按 Agent 并发与上下文需求选择。
- **国内轻量入门**：MiniMax Plus（¥49）、阿里云百炼 Lite（¥39）、火山方舟 Lite（首购 ¥9.9）门槛最低。
- **模型多样性**：火山引擎方舟、OpenCode Go 覆盖多家开源/旗舰模型。
- **无周限额刚需**：小米 MiMo 全档无周/5h 限额。

**通用提示**：一次提问常触发 5–30 次模型调用；先估算月消耗再选档位，避免买高或买低。已激活订阅多数不支持退款。

---

## 五、数据来源与时效说明

- 本表整理于 **2026-10-04**，主要依据各平台官方定价页，并参考 codingplan.org（2026-09 更新）做交叉核对。
- 相比 8 月的老版对比，本表**新增 GPT-6 系列（OpenAI）与 Opus 5.5（Anthropic）**，并更新了 Kimi 新会员体系、智谱 GLM 连续包月价、火山方舟活动价、小米 MiMo V2.6 等最新变动。
- 主要来源：claude.com / platform.claude.com、openai.com / help.openai.com、bigmodel.cn、kimi.com、volcengine.com、codingplan.org。

## 免责声明

本表仅为信息整理，供参考，不构成购买建议。价格、模型阵容与额度随时可能调整，请以各平台官网最新信息为准。
