# x-post-writer-product-announcement

一个用于撰写高质量 X/Twitter 产品宣发帖文的 Claude Skill。

## 这个 Skill 做什么

输入产品/功能信息，输出可直接发布的 X 帖文，确保：

- 首帖控制在 280 字符以内（不被 "Show more" 折叠）
- 首帖在 3 秒内传达 what、value、availability
- 用动作动词而非形容词传递价值
- Thread 作为信息分层工具，每条都有不可替代的新信息
- 克制的工程师语气 —— 无 emoji、无感叹号、无营销腔

## 方法论来源

所有写作规则来自对 **@claudeai** 官方 X 账号（2025年底至2026年初）的系统性逆向工程，覆盖 5M–56M views 的高 engagement 帖文。每一条规则都有真实案例支撑，不是泛泛的社媒写作建议。

**5 条铁律：**

1. **首帖 = 定义 + 价值 + 可用性** —— 读者 3 秒内搞清楚这三件事
2. **Thread 是信息分层工具** —— 每条 reply 补充上一条装不下的信息，不是注水
3. **动作动词 > 形容词** —— "opens your apps, navigates your browser, fills in spreadsheets" 而非 "powerful AI capabilities"
4. **克制的语气** —— 像工程师在 Slack 通知团队，而非市场部在写广告
5. **可用性信息必须可执行** —— 上线状态（GA/beta/preview）+ 适用计划 + 平台限制

## 安装

从 [Releases](../../releases) 下载 `.skill` 文件并添加到你的 Claude Skills 目录。

或者手动将 `SKILL.md` 复制到你的 skills 文件夹：

```
your-skills-directory/
└── x-post-writer-product-announcement/
    └── SKILL.md
```

## 使用方法

用任何涉及 X 帖文 / 推文 / 产品宣发的表述触发本 Skill。例如：

```
帮我写一条X宣发帖文，我们刚上线了 Skill Marketplace 和 Skill Creator，
针对 Basic, Plus, Ultra 用户开放。
```

```
Write an X post announcing our new custom domain feature for the Websites product.
Available for Plus and Ultra users.
```

Claude 会按以下流程工作：
1. 提取关键信息（产品名、价值、机制、可用性）
2. 追问缺失的关键项（尤其是可用性信息）
3. 判断帖文类型（重大发布 / 增量更新 / 品牌声明 / 社区感谢）
4. 撰写帖文并附字符计数
5. 逐条执行自检清单

## 输出格式

```
📎 帖1 (首帖):
[帖文内容]
[字符数: XXX]

📎 帖2 (Thread):
[帖文内容]
[字符数: XXX]
```

## 帖文类型

| 类型 | 适用场景 | 是否需要 Thread |
|------|---------|----------------|
| **A: 重大发布** | 全新产品或重大功能上线 | 通常 2–3 条 |
| **B: 增量更新** | 已有产品的功能迭代 | 通常 1 条 |
| **C: 品牌声明** | 价值观、立场、态度 | 1 条 + 可选跟帖 |
| **D: 社区感谢** | 用户回馈、促销活动 | 2–3 条 |

## 适配其他品牌

本 Skill 的语气以 @claudeai 为原型 —— 克制、精确、不吹嘘。如果你的品牌风格不同，结构性规则（字符限制、信息分层、动作动词优先）仍然通用，语气部分按你的品牌调性调整即可。

## License

MIT
