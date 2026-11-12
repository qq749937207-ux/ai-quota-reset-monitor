# AI 重置监测

**这是一套给 [Grok Bot](https://grok.com) 用的技能（Skill），不是独立安装的软件，也不是官方插件商店里的连接器插件。**

它让 Grok Bot 做两件事：

1. **突发额度重置**：盯各家在正常额度周期之外的额外重置、加赠或可储蓄一次性额度，区分正式宣布和高度疑似，并做量化统计。大约每 30 分钟检查一次，有新情况才通知。
2. **新模型预告**：按用户在监测配置里勾选的模型厂，每天检查新模型、新版本和重要预告。有消息才通知，没有新消息保持安静。

用户不必另外连接 X 账号：公开帖用 Grok Bot 自带的读取能力即可。

This is a **Grok Bot skill** (reusable instructions plus scheduled routines), not a standalone app and not a connector in the official plugin marketplace.

## 这是什么，这不是什么

| 是 | 不是 |
| --- | --- |
| 给 Grok Bot 用的可复用技能 | 可以双击安装的独立程序 |
| 可选的定时例行（额度约每 30 分钟；新模型每天一次） | 官方插件商店里可自行上架的连接器（那种无法自行上架） |
| 可选的公开 Bot 模板，方便别人一键导入 | 需要用户登录 X、或在软件里填写密码令牌的爬虫 |
| 对话里的监测配置：从目录勾选要看的模型厂 | 默认监测目录里的每一家 |

要用它，需要有 Grok Bot。把本仓库里的技能加到自己的 Bot，或导入对应的公开 Bot 模板即可。

## 额度重置监测

- **主目标**：突发 / 额外重置，而不是各家的正常周期恢复。
- **次要**：正常额度恢复，必须按服务单独授权；未授权不查、不编造数字。
- **默认公司**：ChatGPT（OpenAI）、Grok（含 Grok Bot）、Claude（Anthropic）。OpenAI 这边已经核到的突发重置，多为 Codex / ChatGPT Work 额度，展示时要标明范围。
- **节奏**：大约每 30 分钟（可提前或延后最多 15 分钟）。账号清单在 [`docs/accounts.md`](docs/accounts.md)。

分类摘要：

- **正式宣布**：明确说正在重置、已经重置，或发放可储蓄重置。计入正式次数。
- **高度疑似**：来自监测账号、尚未正式宣布、但强烈暗示即将或可能有一次额外重置。标成「疑似」，不计入正式次数；之后正式宣布则改为已确认，不重复计数。
- **不算**：路人猜测、无关玩笑、常规提额、限期加倍、套餐改价、产品发布、自动回复。同一事件只计一次，按公司归类。

## 新模型预告监测

- **目标**：新模型、新版本、公开预览，或已经公开档期的正式预告。
- **节奏**：每天一次（默认用户本地时区上午 9 点，灵活窗口）。
- **配置**：完整目录可以比较长，所以实际监测哪些公司由用户在监测配置里勾选，不要默认全开。初次设置会列出目录；之后对 Bot 说「改监测配置」即可增删。
- **默认可选目录**：美国为 OpenAI、Google DeepMind、Anthropic、xAI、Meta、Microsoft、Amazon；中国为阿里（通义）、字节（豆包）、百度（文心）、腾讯（混元）、华为、DeepSeek、月之暗面（Kimi）、智谱、MiniMax。
- **账号与渠道**：已核实的账号、排除项和官网补充在 [`docs/model-watch.md`](docs/model-watch.md)。华为的正式发布主要在官网新闻站；字节跳动尚未核实到可信的豆包消费级官方 X 号。本技能不能监测微博或微信公众号。

分类同样区分正式发布/预告和高度疑似；额度重置属于另一条监测线，不要混进来。

## 仓库里有什么

| 路径 | 内容 |
| --- | --- |
| [`skill/SKILL.md`](skill/SKILL.md) | 额度重置技能。名称：`AI 公司额度重置监测` |
| [`skill/model-watch.md`](skill/model-watch.md) | 新模型预告技能。名称：`AI 新模型预告监测` |
| [`skill/getting-started.md`](skill/getting-started.md) | 导入模板或新建监测 Bot 后的初次设置（含监测配置） |
| [`routine/prompt.md`](routine/prompt.md) | 额度重置例行（约每 30 分钟） |
| [`routine/model-watch.md`](routine/model-watch.md) | 新模型预告例行（每天一次） |
| [`docs/accounts.md`](docs/accounts.md) | 额度重置：已核实的监测账号 |
| [`docs/model-watch.md`](docs/model-watch.md) | 新模型预告：已核实的账号、排除项和官网补充 |

## 使用方式

### 方式一：导入公开 Bot 模板

若「AI 重置监测」公开模板已发布，在 Grok Bot 里导入该模板（也可以建一个专用 Bot，例如「重置记者」）。导入后会先说明用途，再逐项询问称呼、时区、额度重置范围，并用监测配置让你勾选要看新模型预告的公司，以及要不要打开自动监测。

### 方式二：把技能加到已有的 Grok Bot

1. 把 [`skill/SKILL.md`](skill/SKILL.md) 交给你的 Grok Bot，保存为技能 `AI 公司额度重置监测`。
2. 把 [`skill/model-watch.md`](skill/model-watch.md) 保存为技能 `AI 新模型预告监测`。
3. 按 [`routine/prompt.md`](routine/prompt.md) 建额度例行（`@every 30m`，灵活窗口 ±15 分钟）。
4. 按 [`routine/model-watch.md`](routine/model-watch.md) 建新模型例行（用户本地时区 `0 9 * * *`，灵活窗口），并且只看监测配置里已勾选的公司。
5. 把「结果发给谁、没有新情况时保持安静」写进例行说明。时间用用户本地时区，报告时标明时区。

不需要再给这些技能单独配置 X 登录。

## 贡献

欢迎补充会实际宣布额外重置或新模型的账号，或改进技能说明。请看 [CONTRIBUTING.md](CONTRIBUTING.md)。不要编造尚未核实的公告、数字或帖链接。

## 许可与声明

本项目以 [MIT](LICENSE) 许可开源。

本项目与 OpenAI、Google、Anthropic、xAI、Meta、Microsoft、Amazon、阿里巴巴、字节跳动、百度、腾讯、华为、DeepSeek、月之暗面、智谱、MiniMax、X（Twitter）以及 Grok Bot / Cursor 的运营方均无官方关联，也不代表这些公司或其员工发言。监测依据公开帖和已确认的官方页面，分类由技能规则完成，不保证穷尽或实时。不能监测微博或微信公众号。
