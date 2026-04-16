---
name: x-post-writer-product-announcement
description: 撰写高质量X/Twitter帖文，覆盖产品宣发、社区showcase、tip分享、milestone庆祝、观点输出、use case分享、日常互动等多种场景。当用户要求写X帖文、Twitter帖文、推文、launch post、tweet、X post、X thread、推特文案、宣发文案、产品发布、社区帖文、里程碑庆祝、tip帖、用户作品展示，或者提到"帮我写个X"、"发布推文"、"宣发帖文"、"写个tweet"、"产品发布文案"、"写个X帖"、"Twitter分享"、"发个milestone"、"写个showcase"等任何涉及X/Twitter平台帖文撰写的请求时，必须触发本技能。即使用户只是说"帮我发个X"或"写个推文"也要触发。本技能基于对Anthropic (@claudeai), Notion (@NotionHQ), Figma (@figma), Canva (@canva), Lovable (@lovable_dev) 五家官方X账号的深度拆解，提供结构化的撰写方法论和5档语气光谱。
---

# X/Twitter 帖文撰写技能（多场景 · 多语气版）

## 方法论来源

本技能基于对5个头部品牌官方X账号的系统性逆向工程：

- **@claudeai** (Anthropic) — 克制、工程师语气、信息密度极高
- **@NotionHQ** (Notion) — 温暖、生活化专业、use case叙事驱动
- **@figma** (Figma) — 设计师语气、视觉驱动、用箭头而非bullet
- **@canva** (Canva) — 热情创作者、emoji丰富、大众化
- **@lovable_dev** (Lovable) — 快节奏、全小写、showcase驱动、开发者culture

**这不是5套方法论的拼盘**，而是：**一套通用的结构规则 + 5档可选的语气光谱**。结构规则跨品牌通用（字符限制、信息分层、Thread逻辑），语气按场景和品牌基因选择。

---

## 🚦 首要：信息充足性检查（MUST DO FIRST）

**在动笔之前，必须先检查用户提供的信息是否足够。信息不足时，必须主动询问，不能凭空编造。**

### 不同帖文类型所需的最小信息集

| 帖文类型 | 必须知道的关键信息 |
|---------|------------------|
| 产品宣发 / 功能更新 | 产品名、核心价值（能做什么）、可用性（谁能用、在哪用、什么状态） |
| Community showcase | 展示对象（用户/作品/案例）、选择标准或亮点 |
| Tip / 教程分享 | 具体技巧的操作步骤、适用场景 |
| Milestone 庆祝 | 具体数字、时间点、归因（感谢谁） |
| 观点 / 行业评论 | 明确的立场、支撑论据或对比对象 |
| Use case 分享 | 具体使用者（个人/组织）、具体用途、效果 |
| 日常互动 | 讨论主题、品牌立场 |

### 澄清追问的原则

- **一次性问完，不要挤牙膏。** 把缺失的信息打包成3-5个问题，一次性让用户回答
- **给例子。** 问"具体能做什么"时，可以举例："比如'一键生成品牌PPT'或'自动抓竞品数据'这样的具体场景"
- **可用性信息永远不能编造。** 如果用户没说"beta还是GA"、"哪些plan可用"，必须问
- **如果用户信息充足，直接跳过澄清，开始写作**

### 澄清追问示例

当用户说"帮我写个X帖文，我们上线了Skill Marketplace"时：

```
在开始前需要确认几个关键信息：

1. Skill Marketplace的核心功能是什么？是让用户浏览/安装别人做的Skills，
   还是同时包含Creator功能？
2. Skills能帮用户做什么？能举1-2个具体use case吗？（例如"一键生成品牌PPT"
   "自动抓竞品数据做周报"）
3. 可用性信息——这是GA还是beta？哪些用户计划可以使用？平台是网页端还是桌面端？
4. 是否需要在最后放引导链接？
```

---

## 📐 通用结构规则（跨品牌通用）

以下规则无论用哪种语气都适用。

### 规则1：首帖字符限制

首帖（timeline直接展示的那条）必须控制在 **200-280 英文字符**（含空格），确保不被"Show more"折叠。

中文首帖建议控制在 **80-140 字符**以内。

这是硬约束。

### 规则2：首帖三要素（不同场景的three-things）

不同帖文类型的首帖"三要素"不同：

- **产品宣发：** What（是什么）+ Value（能干什么）+ Availability（谁能用）
- **Community showcase：** Who/What（展示谁/什么）+ Why compelling（为什么值得看）+ Link/CTA
- **Tip分享：** Problem/Opportunity（什么场景）+ Solution（怎么做）+ Outcome（结果）
- **Milestone：** Number（数字）+ Context（背景）+ Thanks（归因/感谢）
- **观点：** Claim（主张）+ Reason/Evidence（论据）+ Punchline/Implication（收束）
- **Use case：** Who（谁在用）+ How（怎么用）+ Result（什么结果）

### 规则3：Thread是信息分层工具，不是注水工具

Thread的每一条必须独立成立、有新信息。黄金法则：**如果一条Thread帖拿掉后不影响理解，它就不该存在。**

标准Thread结构：
- **帖1（首帖）：** 按"首帖三要素"撰写
- **帖2：** How it works / 细节展开 / 具体例子
- **帖3：** 补充信息（价格、边界、链接、CTA）

Thread总数控制在 **2-4条**（含首帖），绝大多数情况下2-3条足够。

### 规则4：动作动词 > 形容词

这条跨品牌通用。即使是最热情的Canva语气，高质量的帖文也主要靠**动作描述**，而不是堆形容词。

```
❌ Introducing our revolutionary new AI agent platform with powerful capabilities.
✅ It opens your apps, navigates your browser, fills in spreadsheets.
```

常用手法：
- 并列3个动作堆叠形成节奏感
- 破折号（em dash）后放总结性短语收束
- "without [你原来要做的麻烦事]" 是强力收束结构

### 规则5：可用性/归因信息必须精确

- 产品宣发：上线状态（GA/beta/research preview）+ 适用计划 + 平台限制
- Milestone：具体数字 + 时间范围
- Showcase：作品/用户的具体来源
- Use case：用户的具体身份/公司

---

## 🎨 5档语气光谱

### 档位1：Restrained（克制）— 默认

**品牌原型：@claudeai**

**语气特征：**
- 无emoji
- 无感叹号（整3个月出现次数接近于零）
- 短句、信息密集
- 动作动词为主
- 第二人称"you"为主，偶尔"we"
- 不吹嘘（不说"best"、"revolutionary"，除非有benchmark硬背书）

**适用场景：** 产品宣发（默认）、技术产品增量更新、严肃品牌声明、面向开发者/专业人士的帖文

**标志性句式：**
- `You can now [do X].`
- `Introducing [Product]: [one-line value prop].`
- `New in [Product]: [feature name].`
- `[Product] is now available in [scope].`
- `Instead of [old way], [new thing] lets you [benefit].`

**范例（@claudeai Computer Use发布）：**
```
You can now enable Claude to use your computer to complete tasks.

It opens your apps, navigates your browser, fills in spreadsheets—
anything you'd do sitting at your desk.

Research preview in Claude Cowork and Claude Code, macOS only.
```

### 档位2：Warm Productivity（温暖专业）

**品牌原型：@NotionHQ**

**语气特征：**
- 偶尔emoji（点缀式：📆 💡 👍 🐝 🎉），不堆砌
- 感叹号谨慎使用，多出现在社区/感谢场景
- 允许长段落、故事化叙事
- 客户引述密集（"X at Y saved 20 minutes a day"）
- "Big news today:"、"And they're pretty different from..." 这类略带生活化的导入句
- 多用 "your team"、"teammates"、"work"，强化"协作/工作流"语境

**适用场景：** 偏专业但想要温度的产品宣发、客户故事、use case分享、团队协作类产品

**标志性句式：**
- `Big news today: [thing] are finally here!`
- `Here's what [Product] can do:`
- `[Customer Name] at [Company] uses [Product] to [outcome].`
- `Just describe what you want in plain language, and [Product] builds it for you.`

**范例（@NotionHQ Custom Agents）：**
```
Big news today: Custom Agents are finally here! And they're pretty 
different from other AI tools you've tried.

First, they're completely autonomous (no manual prompting). Just 
give them a job, set a trigger, and they'll get it done, 24/7.

[客户引述]「Each update saves me 20 minutes a day.」 
— Morgane Palomares, VP Marketing at Braintrust
```

### 档位3：Designerly（设计师感）

**品牌原型：@figma**

**语气特征：**
- 很少用emoji，但用 → 箭头做列表（视觉化）
- 喜欢用短的标题式结构（"Config 2025 Key Dates:"）
- 技术词汇精准（layers, components, tokens, auto-layout）
- 偏好设计师圈的内部梗和专业表达
- "Bookmark this"、"Did you catch them all?" 带有设计师社群感

**适用场景：** 设计工具产品、面向设计师/创意专业人士、会议/活动预告、视觉驱动的发布

**标志性句式：**
- `[Event/Product] Key Dates:`
- `Here's everything we announced at [Event]:`
- `→ [Item 1]`
- `→ [Item 2]`
- `Did you catch them all?`

**范例（@figma Config 2025 汇总）：**
```
Did you catch them all? Here's everything we announced at #Config2025

→ Figma Sites
→ CMS in Figma Sites (coming soon)
→ Grid
→ Figma Make
→ Figma Draw
→ Figma Buzz
```

### 档位4：Friendly Creator（热情创作者）

**品牌原型：@canva**

**语气特征：**
- emoji丰富（🎉 🚀 💫 🌟 💪 🙌），但不失控
- 感叹号常见
- "super excited"、"hooray"、"big news alert"
- 面向大众创作者（非专业设计师）
- 鼓励式、包容式语气
- 喜欢情感化词汇（"joyful"、"empower"、"dream"）

**适用场景：** 面向C端/大众创作者的产品、创意工具、教育/入门功能、节日/庆祝、社交媒体资产创作类

**标志性句式：**
- `🎉 Big News Alert! 🚀`
- `We're super excited to share [news]!`
- `Get ready for [benefit]!`
- `Hooray! [feature] is here!`

**⚠️ 使用警告：** 这是最容易"写崩"的语气档位。Emoji和感叹号过度使用会让帖文显得廉价。即使选择这个档位，每条帖文emoji数量也应控制在 **1-3个**，感叹号控制在 **1-2个**。

**范例（@canva Affinity联合）：**
```
🎉 Big News Alert! 🚀

We're super excited to share Canva has joined forces with 
@affinitybyserif — the creative software suite loved by millions 
of designers around the world.

Get ready for an incredible fusion of creativity and innovation.
```

### 档位5：Playful Builder（快节奏建造者）

**品牌原型：@lovable_dev**

**语气特征：**
- **全小写**（这是Lovable的品牌标识）
- 句子极短，像聊天
- 用 "-" 做破折号而非 em dash
- 大量使用 showcase 驱动的帖文
- 喜欢搞 challenge / 奖金活动
- 开发者文化梗（"vibe coding"、"ship it"、"launched"）
- "we just [did X]" 的即时感

**适用场景：** 开发者工具、面向builder/maker社区、community challenge、showcase帖、快速发布

**标志性句式：**
- `introducing [product name]`
- `we just launched [X] - and [invitation]`
- `build [thing] with us`
- `[X] is now live`
- `quote this tweet with [your build]`

**范例（@lovable_dev Lovable 2.0）：**
```
we just launched lovable 2.0 – and we want you to launch with us

build a 2.0 version of any product with lovable and quote this 
tweet with it

our favorite by monday wins $8k
```

### 📊 语气选择决策表

当用户没指定语气时，Claude根据场景推荐默认语气。**默认从Restrained开始，但在询问信息时主动提供5种语气选项让用户选择。**

| 场景 | 推荐语气 | 备选 |
|------|---------|------|
| 技术产品宣发（to开发者/企业） | Restrained | Warm Productivity |
| 工作/协作工具宣发 | Warm Productivity | Restrained |
| 设计工具 / 创意专业工具 | Designerly | Warm Productivity |
| C端创意工具 / 大众创作者 | Friendly Creator | Warm Productivity |
| 开发者工具 / Builder社区 | Playful Builder | Restrained |
| 严肃品牌声明 / 价值观 | Restrained | Warm Productivity |
| Community showcase | Playful Builder / Warm Productivity | Designerly |
| Milestone庆祝 | Warm Productivity | Friendly Creator |
| Tip分享 | Restrained / Playful Builder | - |
| 观点输出 | Restrained | - |

---

## 📝 8种帖文类型模板

### 类型1：产品宣发（Major Launch）

适用于全新产品或重大功能上线。

**标准Thread结构：**
```
帖1:
[根据语气档位选开头] + [核心价值 2-3个动作动词] + [可用性状态]

帖2 (Thread):
[How it works / 细节]
- [机制/细节1]
- [机制/细节2]
- [机制/细节3]

帖3 (Thread):
[定价/适用范围/链接]
```

### 类型2：功能增量更新（Incremental Update）

已有产品的功能迭代。通常不需要Thread。

```
[功能名] is now [动作/状态].

[一句话说明变化带来的具体好处].

[可用性状态].
```

### 类型3：Community Showcase（用户作品展示）

展示用户作品/案例。

```
帖1:
[引入语：Some delightfully specific things... / Built with [Product] this week: 
/ What our community is building]

[简短点题/一句话主旨]

帖2+ (每个作品一条Thread):
[作品名 by @creator]
[一两句描述它的特别之处]
[作品链接/媒体]
```

**范例句式：**
- `Some delightfully specific things people are building with [Product] lately.`
- `What our community shipped this week:`
- `Built with [Product]:`

### 类型4：Tip / 教程分享

分享使用技巧。

```
[场景描述：一句话说明这个tip解决什么问题]

[具体步骤，用bullet或编号]
- [Step 1]
- [Step 2]
- [Step 3]

[结果 / 为什么有效]
```

或极简版（单条）：
```
[Tip具体操作]. [一句话说明为什么有效].
```

### 类型5：Milestone / 数据庆祝

里程碑庆祝。

```
帖1:
[具体数字 + 背景，一句话说完].

帖2 (Thread, optional):
[归因 / 感谢 / use case佐证]

帖3 (Thread, optional):
[展望 / 链接]
```

**语气选择提示：** 这类帖文在@NotionHQ和@claudeai中都有，语气差异明显。选Warm Productivity更有温度，选Restrained更克制专业。

### 类型6：观点 / 行业评论

品牌发声。

```
[引人注目的短句判断].
[反转或补充论据].
[收束 / Punchline / Implication].
```

**范例（@claudeai ad-free声明）：**
```
Ads are coming to AI. But not to Claude. Keep thinking.
```

**强烈推荐：** 这类帖文几乎只适合Restrained语气。其他语气用了会削弱观点力度。

### 类型7：Use Case 分享

具体使用者/客户故事。

```
帖1:
[Who is doing what, in one sentence]

帖2 (Thread):
[How they're using it, specific workflow or quote]

帖3 (Thread):
[Result / impact, ideally with number]
```

**范例（@NotionHQ客户故事）：**
```
Morgane Palomares, VP of Marketing at Braintrust, uses Custom Agents 
to get to faster decisions.

"One competitive agent posts daily updates, and our customer reference 
agent sends a weekly summary of top new logos to me and the CEO."

Each update saves her 20 minutes a day.
```

### 类型8：日常互动 / 社群化

回答社群提问、互动、轻量内容。

```
[问题 / 观察 / 开放式提示]
[可选：附图 / @某人 / 链接]
```

**范例（@canva十周年）：**
```
Ten years later ⏳

What's changed for you and what's stayed the same? 👀
```

**这类帖文不需要严格Thread结构，首帖即本体。**

---

## 🔄 完整写作流程

### Step 1: 信息充足性检查

对照"最小信息集"表检查。信息不足则**一次性追问**所有缺失项。**不要假装有这些信息然后编造。**

### Step 2: 帖文类型判断

根据信息判断属于8种类型中的哪一种（或跨类型混合）。

### Step 3: 语气档位推荐

- 如果用户明确指定了语气偏好 → 直接用
- 如果用户提到品牌原型（"像Claude那样"/"像Canva那样"）→ 直接用对应档位
- 否则 → **主动列出5种语气选项让用户选**，同时标注你基于场景的推荐。默认是Restrained。

**向用户提供语气选项的示例格式：**
```
撰写前想和你确认一下语气偏好（5档可选）：

1. Restrained (克制工程师) — @claudeai风格，无emoji、短句密集 ← 推荐默认
2. Warm Productivity (温暖专业) — @NotionHQ风格，有温度、故事化
3. Designerly (设计师感) — @figma风格，箭头列表、视觉驱动
4. Friendly Creator (热情创作者) — @canva风格，emoji+感叹号
5. Playful Builder (快节奏建造者) — @lovable_dev风格，全小写、showcase驱动

你的场景是[XXX]，我推荐[档位N]。要用这个还是换一个？
```

### Step 4: 撰写首帖

- 严格控制字符数（英文200-280 / 中文80-140）
- 按对应帖文类型的"三要素"撰写
- 按语气档位选择句式和词汇
- 按语气档位控制emoji/感叹号数量

### Step 5: 判断Thread结构

- 首帖已经说清所有关键信息 → 不需要Thread
- 有"how it works"需要解释 → 加帖2
- 有补充信息/链接 → 加帖3
- Thread总数控制在2-4条

### Step 6: 自检清单

- [ ] 首帖字符数是否合规（英文≤280/中文≤140）？
- [ ] 首帖是否在3秒内让人理解要传达的信息？
- [ ] 动作动词是否多于形容词？
- [ ] Emoji/感叹号数量是否符合所选语气档位？
- [ ] Thread的每一条是否都有不可替代的新信息？
- [ ] 关键信息（可用性/归因/数字）是否精确，没有编造？
- [ ] 语气是否与所选档位保持一致，没有风格漂移？

---

## 📤 输出格式

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

---

## ⚠️ 注意事项

- **不凭空编造信息。** 可用性、数字、归因这三类信息缺失时必须追问
- **不随意混搭语气。** 选定一档后保持一致。Restrained中间插一个emoji会显得很奇怪，Friendly Creator全程零emoji也会显得冷淡
- **5个品牌范本不是"最佳标准"，而是"定位标尺"。** 你的品牌/产品应该基于实际定位选择最贴近的一档
- **中文帖文的结构规则通用，但语气需要本土化调整。** 例如Restrained在中文里不意味着冷淡，而是"精炼清晰"；Playful Builder在中文里不用全小写，可以用更口语化的表达替代
- 本Skill针对**单次帖文/thread撰写**。连续内容策略（如一周发几条、节奏安排）不在本Skill范围内

