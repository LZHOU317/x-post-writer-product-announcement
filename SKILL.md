---
name: x-post-writer
description: 撰写高质量X/Twitter产品宣发帖文。当用户要求写X帖文、Twitter帖文、产品发布推文、宣发文案、launch post、tweet、X post、推特文案，或者提到"帮我写个X"、"发布推文"、"宣发帖文"、"写个tweet"、"产品发布文案"、"X thread"、"推文"等任何涉及X/Twitter平台产品宣发的请求时，必须触发本技能。即使用户只是说"帮我发个X"或"写个产品发布"也要触发。本技能基于对Anthropic官方@claudeai账号过去3个月宣发帖文的深度拆解，提炼出一套经过验证的方法论，确保每条帖文做到：不被折叠、信息密度高、结构清晰、Thread层次分明。
---

# X/Twitter 产品宣发帖文撰写技能

## 方法论来源

本技能的所有原则和模式，来自对 **@claudeai** 官方X账号在2025年底至2026年初（约3个月）所有产品宣发帖文的系统性拆解。以下方法论不是泛泛的"社媒写作技巧"，而是从高engagement（数百万至数千万views）的真实帖文中逆向工程出来的规律。

---

## 核心方法论：5条铁律

### 铁律1：首帖 = 一句话定义 + 一句话价值 + 可用性状态

首帖（即timeline上直接展示的那条）的使命是让读者在3秒内搞清楚三件事：**这是什么、能干什么、我现在能不能用**。

**结构公式：**
```
[动词开头的产品定义句]
[具象化的价值描述——用动作而非形容词]
[可用性/上线状态。一句话。]
```

**优秀案例拆解：**

案例A — Computer Use 发布帖（15.9M views）:
```
You can now enable Claude to use your computer to complete tasks.

It opens your apps, navigates your browser, fills in spreadsheets—anything you'd do sitting at your desk.

Research preview in Claude Cowork and Claude Code, macOS only.
```
拆解：
- 第一句：动词开头（"You can now"），直接告诉你what
- 第二句：用三个并列动作（opens/navigates/fills）具象化价值，再用一个破折号总结（"anything you'd do"）
- 第三句：可用性状态，精确到产品线和平台

案例B — Claude Managed Agents（20.9M views）:
```
Introducing Claude Managed Agents: everything you need to build and deploy agents at scale.

It pairs an agent harness tuned for performance with production infrastructure, so you can go from prototype to launch in days.

Now in public beta on the Claude Platform.
```
拆解：
- "Introducing X: [价值定位]" 是另一种有效的开头范式
- 第二句用 "pairs A with B, so you can [结果]" 结构交代how和why
- 第三句极简可用性

案例C — Auto Mode（7.6M views）:
```
New in Claude Code: auto mode.

Instead of approving every file write and bash command, or skipping permissions entirely, auto mode lets Claude make permission decisions on your behalf.

Safeguards check each action before it runs.
```
拆解：
- "New in [产品]: [功能名]." — 适用于已有产品的增量功能发布
- 第二句用 "Instead of A or B, [功能] lets you C" 的对比结构，让读者秒懂差异
- 第三句补充安全保障，消除顾虑

**关键数据：首帖字符数控制。** @claudeai的高engagement首帖几乎全部在 **200-280个英文字符**（含空格）之间。这个长度确保在timeline上完整展示，不会被"Show more"折叠。这是硬约束，必须遵守。

### 铁律2：Thread是信息分层工具，不是注水工具

Thread的每一条都必须独立成立、有新信息。@claudeai的Thread模式如下：

**帖1（首帖）：** What + Value + Availability（按铁律1）
**帖2：** How it works — 用最简洁的方式交代机制，通常是3个短bullet或一段精简描述
**帖3：** 边界条件/补充细节 — 价格、适用范围、限制、链接

案例 — "双倍用量"活动（12.6M views）的Thread：
```
帖1: A small thank you to everyone using Claude:
We're doubling usage outside our peak hours for the next two weeks.

帖2: How it works:
- 2x usage on weekdays outside 5–11am PT / 12–6pm GMT
- 2x usage all day on weekends
- Automatic, nothing to enable

帖3: This bonus usage applies everywhere you work with Claude—including Claude Code—on the free, Pro, Max, and Team plans.
```

**Thread的黄金法则：**
- 如果一条Thread帖拿掉后不影响理解，它就不该存在
- Thread帖越少越好。能2条说清楚就不用3条
- 每条Thread帖也有自己的字符长度意识——帖2和帖3可以稍长，但单条不超过280字符仍然是最佳实践
- 帖2适合用bullet list（用短横线 `-`），帖1永远不用bullet

### 铁律3：用动作动词而非形容词来传递价值

@claudeai几乎从不用"powerful"、"revolutionary"、"game-changing"这类形容词。取而代之的是**具体的动作描述**，让读者自己得出"这很强"的结论。

**反模式（不要这样写）：**
```
❌ Introducing our revolutionary new AI agent platform with powerful capabilities.
```

**正确模式：**
```
✅ It opens your apps, navigates your browser, fills in spreadsheets—anything you'd do sitting at your desk.
```

```
✅ Pull data from spreadsheets, build out tables, and update a deck — without re-explaining a step.
```

```
✅ When a PR opens, Claude dispatches a team of agents to hunt for bugs.
```

**动作动词技巧：**
- 使用 "opens / navigates / fills / pulls / builds / dispatches / scans / hunts" 这类具象动词
- 用并列结构堆叠3个动作，形成节奏感
- 破折号（em dash）后面放一个总结性短语，收束整个句子
- "without [你原来要做的麻烦事]" 结尾是强力收束手法

### 铁律4：语气克制，像工程师在Slack里通知团队

@claudeai的品牌语气可以用四个词概括：**克制、精确、平视、自信**。

具体表现：
- **不用感叹号。** 翻遍@claudeai近3个月的帖文，感叹号出现次数接近于零
- **不用emoji。** 这是和绝大多数品牌X账号最大的差异
- **不吹嘘。** 不说"best"、"fastest"、"most advanced"（除非有直接的benchmark支撑，如Sonnet 4.5发布时的"the best coding model in the world"有benchmark数据背书）
- **不催促。** 不说"Don't miss out"、"Try it now!"、"You won't believe"
- **第二人称("you")为主，偶尔用第一人称复数("we")。** 例如 "You can now..." / "We're doubling usage..."
- **有幽默感，但点到即止。** 如 "Ads are coming to AI. But not to Claude. Keep thinking." — 三句话，最后两个字是punchline

### 铁律5：可用性信息必须精确到可执行

每条产品发布帖都必须包含足够的信息让读者判断"我能不能用"：

**必填项：**
- 上线状态（GA / public beta / research preview / limited preview）
- 适用计划（free / Pro / Max / Team / Enterprise）
- 平台限制（macOS only / API only / Claude Code only）

**可选项（视情况）：**
- 价格/定价模型
- 地区限制
- 链接（通常放在最后一条Thread帖或首帖末尾）

案例：
```
✅ Research preview in Claude Cowork and Claude Code, macOS only.
✅ Now in public beta on the Claude Platform.
✅ Now in research preview on Pro and Max plans.
✅ Now the default for Pro and Team plans.
```

---

## 帖文类型模板

### 类型A：新产品/新功能发布（Major Launch）

适用于全新产品或重大功能。这是最常见的宣发类型。

```
帖1:
[Introducing/You can now/New in 产品:] [功能名称/一句话定义]。

[2-3个具象动作描述价值，用并列结构]。

[可用性状态，精确到计划和平台]。

帖2 (Thread, 仅在需要补充how/机制时):
[How it works / 机制描述]
- [细节1]
- [细节2]
- [细节3]

帖3 (Thread, 仅在需要补充边界/链接时):
[补充适用范围/价格/链接]
```

### 类型B：增量更新（Incremental Update）

适用于已有产品的功能迭代。首帖更短，通常不需要Thread。

```
[功能名] is now [动作/状态].

[一句话说明变化带来的具体好处].

[可用性状态].
```

案例：
```
Memory is now available on the free plan.
We've also made it easier to import saved memories into Claude. You can export them whenever you want.
```

### 类型C：品牌态度/价值观声明

适用于非功能性的品牌宣发。极少见但engagement极高。

```
[引人注目的短句/判断].
[反转或补充].
[收束/punchline].
```

案例：
```
Ads are coming to AI. But not to Claude. Keep thinking.
```

Thread跟进（如有）用更正式的语气展开：
```
Claude is built to be a genuinely helpful assistant for work and for deep thinking. Advertising would be incompatible with that vision.
Read why Claude will remain ad-free: [link]
```

### 类型D：社区/用户感谢

适用于回馈用户的活动。

```
[以感谢/回馈为起点的短句].
[具体利好——用数字和动作描述].

Thread: [How it works 细节]
Thread: [适用范围]
```

---

## 写作流程

当用户给出一个产品/功能的信息，按以下步骤撰写：

### Step 1: 提取关键信息
从用户提供的材料中提取：
- **产品/功能名称**
- **核心价值（它能帮用户做什么？）**
- **工作机制（它怎么做到的？）**
- **可用性信息（谁能用？在哪用？什么状态？）**
- **边界/限制（有什么不能做的？价格？）**

如果用户提供的信息不完整，**先追问关键缺失项**（尤其是可用性信息），不要凭空编造。

### Step 2: 判断帖文类型
根据信息判断属于A/B/C/D哪种类型，选择对应模板。

### Step 3: 撰写首帖
- 严格控制在 **200-280 英文字符**（含空格）
- 用动作动词，不用形容词
- 包含 what + value + availability
- 不用emoji，不用感叹号

### Step 4: 判断是否需要Thread
- 如果首帖已经说清了所有关键信息 → 不需要Thread
- 如果有"how it works"需要解释 → 加帖2
- 如果有补充细节（价格、适用范围、链接占位） → 加帖3
- Thread总数控制在 **2-4条**（含首帖），绝大多数情况下2-3条足够

### Step 5: 自检清单
撰写完成后，逐条检查：
- [ ] 首帖是否 ≤280 字符？
- [ ] 首帖是否在3秒内让人理解 what + value + availability？
- [ ] 是否使用了动作动词而非形容词？
- [ ] 是否避免了感叹号和emoji？
- [ ] 语气是否像"工程师在Slack通知团队"而非"市场部在写广告"？
- [ ] Thread的每一条是否都有不可替代的新信息？
- [ ] 可用性信息是否精确到可执行（状态+计划+平台）？

---

## 输出格式

帖文输出使用以下格式，方便用户直接复制：

```
📎 帖1 (首帖):
[帖文内容]
[字符数: XXX]

📎 帖2 (Thread):
[帖文内容]
[字符数: XXX]

📎 帖3 (Thread):
[帖文内容]
[字符数: XXX]
```

每条帖文后附上字符计数，帮助用户确认不会被折叠。

如果用户提供的是中文产品信息但需要英文帖文，默认输出英文帖文。如果用户明确要求中文帖文，则按中文X/Twitter的展示规则调整（中文首帖建议控制在140字以内）。

---

## 注意事项

- 本技能针对的是**产品宣发类帖文**，不是通用社媒内容。对于日常互动、meme、community showcase等类型，本技能的规则不一定适用
- @claudeai的品牌人格——克制、精确、平视——和很多品牌截然不同。写作时要抵制"加点料让它更exciting"的冲动。信息密度本身就是excitement
- 如果用户的产品和Claude/Anthropic无关，仍然可以借鉴本方法论，但需要根据品牌调性做适当调整。可以主动提醒用户这一点
