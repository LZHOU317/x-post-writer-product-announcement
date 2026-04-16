# x-post-writer-product-announcement

一个用于撰写高质量 X/Twitter 帖文的 Claude Skill。覆盖产品宣发、社区 showcase、tip 分享、milestone 庆祝、观点输出、use case 分享等多种场景，提供 5 档可选语气光谱。

## 这个 Skill 做什么

输入帖文主题/素材信息，输出可直接发布的 X 帖文，确保：

- 首帖控制在 280 字符以内（不被 "Show more" 折叠）
- 首帖在 3 秒内传达该场景的三要素
- Thread 作为信息分层工具，每条都有不可替代的新信息
- 语气与所选档位保持一致，不漂移
- 信息不足时主动追问，不凭空编造

## 方法论来源

所有写作规则来自对 5 个头部品牌官方 X 账号的系统性逆向工程：

| 品牌 | 账号 | 语气特征 |
|------|------|---------|
| Anthropic | @claudeai | 克制、工程师语气、信息密度极高 |
| Notion | @NotionHQ | 温暖、生活化专业、use case 叙事 |
| Figma | @figma | 设计师语气、视觉驱动、箭头列表 |
| Canva | @canva | 热情创作者、emoji 丰富、大众化 |
| Lovable | @lovable_dev | 快节奏、全小写、showcase 驱动 |

**核心架构：** 一套通用结构规则 + 5 档可选语气光谱。结构规则跨品牌通用，语气按场景和品牌基因选择。

## 核心结构规则

无论选哪档语气，以下规则通用：

1. **首帖字符限制** —— 英文 200-280 字符 / 中文 80-140 字符
2. **首帖三要素** —— 不同场景的 three-things 各不相同（产品宣发 = What + Value + Availability；Showcase = Who + Why compelling + Link；Milestone = Number + Context + Thanks；以此类推）
3. **Thread 是信息分层工具** —— 每条 reply 补充上一条装不下的信息，不是注水
4. **动作动词 > 形容词** —— "opens your apps, navigates your browser, fills in spreadsheets" 而非 "powerful AI capabilities"
5. **关键信息必须精确** —— 可用性、数字、归因三类信息不能编造

## 5 档语气光谱

- **Restrained（克制工程师）** — @claudeai 风格。无 emoji、无感叹号、短句密集。默认档位
- **Warm Productivity（温暖专业）** — @NotionHQ 风格。偶尔 emoji 点缀、故事化叙事、客户引述
- **Designerly（设计师感）** — @figma 风格。箭头 → 列表、视觉驱动、设计师圈词汇
- **Friendly Creator（热情创作者）** — @canva 风格。emoji + 感叹号、鼓励式、面向大众创作者
- **Playful Builder（快节奏建造者）** — @lovable_dev 风格。全小写、showcase 驱动、challenge/奖金文化

## 8 种帖文类型

| 类型 | 适用场景 | 是否需要 Thread |
|------|---------|----------------|
| **产品宣发（Major Launch）** | 全新产品或重大功能上线 | 通常 2–3 条 |
| **功能增量更新** | 已有产品的功能迭代 | 通常 1 条 |
| **Community Showcase** | 用户作品/案例展示 | 视作品数量 |
| **Tip / 教程分享** | 使用技巧 | 1 条或 2 条 |
| **Milestone / 数据庆祝** | 用户数、里程碑、周年 | 1–3 条 |
| **观点 / 行业评论** | 品牌发声、立场 | 1 条 + 可选跟帖 |
| **Use Case 分享** | 客户故事、具体用法 | 2–3 条 |
| **日常互动 / 社群化** | 开放式提问、轻量内容 | 通常 1 条 |

## 安装

从 [Releases](../../releases) 下载 `.skill` 文件并添加到你的 Claude Skills 目录。

或者手动将 `SKILL.md` 复制到你的 skills 文件夹：

```
your-skills-directory/
└── x-post-writer-product-announcement/
    └── SKILL.md
```

## 使用方法

用任何涉及 X 帖文 / 推文的表述触发本 Skill。Claude 会按以下流程工作：

1. **信息充足性检查** —— 对照最小信息集，信息不足则一次性追问所有缺失项
2. **帖文类型判断** —— 判断属于 8 种类型中的哪一种
3. **语气档位推荐** —— 主动列出 5 档让你选择，默认推荐 Restrained
4. **撰写首帖 + Thread** —— 严格遵循字符限制和结构规则
5. **自检清单** —— 逐条检查后输出带字符计数的帖文

### 使用示例

```
帮我写一条X宣发帖文，我们刚上线了 Skill Marketplace 和 Skill Creator，
针对 Basic, Plus, Ultra 用户开放。
```

```
我们用户数突破 10 万了，帮我写一条 milestone 帖，想要有温度一点的感觉。
```

```
帮我写一条 showcase 帖，展示用户用我们 Skills 做的有意思的作品，
要 Lovable 那种 playful 的感觉。
```

## 输出格式

```
📎 帖1 (首帖):
[帖文内容]
[字符数: XXX]

📎 帖2 (Thread):
[帖文内容]
[字符数: XXX]
```

## 适配其他品牌

5 个品牌范本不是"最佳标准"，而是"定位标尺"。你的品牌/产品应该基于实际定位选择最贴近的一档，而不是盲目追求某个风格。

对于中文帖文，结构规则通用，但语气需本土化调整：
- Restrained 在中文里 ≠ 冷淡，而是"精炼清晰"
- Playful Builder 在中文里不用全小写，可以用更口语化的表达替代
- Friendly Creator 在中文里 emoji 数量建议比英文再克制 1-2 个

## 更新记录

- **v2** — 扩展至 5 档语气光谱（原仅 @claudeai 单一风格）+ 8 种帖文类型（原仅 4 种）+ 强制澄清流程
- **v1** — 基础版，聚焦产品宣发场景，单一 Restrained 语气

## License

MIT
