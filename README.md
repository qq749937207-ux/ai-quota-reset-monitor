# AI 重置监测

**这是一套给 [Grok Bot](https://grok.com) 用的技能（Skill），不是独立安装的软件，也不是官方插件商店里的连接器插件。**

它让 Grok Bot 盯各家 AI 公司在正常额度周期之外的突发重置（额外重置、加赠、可储蓄一次性额度），区分正式宣布和高度疑似，并做量化统计。用户不必另外连接 X 账号：公开帖用 Grok Bot 自带的读取能力即可。

This is a **Grok Bot skill** (reusable instructions plus a scheduled routine), not a standalone app and not a connector in the official plugin marketplace.

## 这是什么，这不是什么

| 是 | 不是 |
| --- | --- |
| 给 Grok Bot 用的可复用技能 | 可以双击安装的独立程序 |
| 可选的定时例行（约每 30 分钟检查一次） | 官方插件商店里可自行上架的连接器（那种无法自行上架） |
| 可选的公开 Bot 模板，方便别人一键导入 | 需要用户登录 X、或在软件里填写密码令牌的爬虫 |

要用它，需要有 Grok Bot。把本仓库里的技能加到自己的 Bot，或导入对应的公开 Bot 模板即可。

## 它做什么

- **主目标**：突发 / 额外重置，而不是各家的正常周期恢复。
- **次要**：正常额度恢复，必须按服务单独授权；未授权不查、不编造数字。
- **展示**：按公司归类。完整监测账号名单在 [`docs/accounts.md`](docs/accounts.md)，不作为日常展示的主体。
- **节奏**：大约每 30 分钟检查一次（可提前或延后最多 15 分钟）。有新的正式宣布或高度疑似才通知，没有新情况保持安静。

默认监测 ChatGPT（OpenAI）、Grok（含 Grok Bot）、Claude（Anthropic）。OpenAI 这边已经核到的突发重置，多为 Codex / ChatGPT Work 额度，不是普通 ChatGPT 对话额度，展示时要标明范围。

## 仓库里有什么

| 路径 | 内容 |
| --- | --- |
| [`skill/SKILL.md`](skill/SKILL.md) | 通用监测技能：范围、分类、统计、检查和通知规则。技能名称：`AI 公司额度重置监测` |
| [`skill/getting-started.md`](skill/getting-started.md) | 导入 Bot 模板后的初次设置（称呼、时区、监测范围、是否开启定时监测） |
| [`routine/prompt.md`](routine/prompt.md) | 定时例行的任务说明（约每 30 分钟） |
| [`docs/accounts.md`](docs/accounts.md) | 已核实的监测账号、用户 ID、角色、排除项 |

## 使用方式

### 方式一：导入公开 Bot 模板

若「AI 重置监测」公开模板已发布，在 Grok Bot 里导入该模板。导入后的 Bot 会先说明用途，再逐项询问称呼、时区、监测范围，以及要不要打开约 30 分钟一次的自动监测。

### 方式二：把技能加到已有的 Grok Bot

1. 把 [`skill/SKILL.md`](skill/SKILL.md) 交给你的 Grok Bot，请它保存为技能，名称用 `AI 公司额度重置监测`。
2. 按 [`routine/prompt.md`](routine/prompt.md) 建一条例行：日程用 `@every 30m`，灵活窗口可提前或延后最多 15 分钟。
3. 把「结果发给谁、没有新情况时保持安静」写进例行说明。
4. 时间用用户本地时区，报告时标明时区。

不需要再给这个技能单独配置 X 登录。Grok Bot 自带公开 X 读取即可。

## 分类规则（摘要）

- **正式宣布**：明确说正在重置、已经重置，或发放可储蓄重置。计入正式次数。尽量区分即时到账和可储蓄。
- **高度疑似**：来自监测账号、尚未正式宣布、但强烈暗示即将或可能有一次额外重置。标成「疑似」，单独列出，不计入正式次数；之后正式宣布则改为已确认，不重复计数。
- **不算**：路人猜测、无关玩笑、常规提额、限期加倍、套餐改价、产品发布、自动回复。
- 同一事件被多人宣布或转发只计一次，归到对应公司。

账号清单里记录了已改名、被占用或同名无关的号，增加监测对象前请先读 [`docs/accounts.md`](docs/accounts.md)。

## 贡献

欢迎补充会实际宣布额外重置的账号，或改进技能说明。请看 [CONTRIBUTING.md](CONTRIBUTING.md)。不要编造尚未核实的公告、数字或帖链接。

## 许可与声明

本项目以 [MIT](LICENSE) 许可开源。

本项目与 OpenAI、xAI、Anthropic、X（Twitter）以及 Grok Bot / Cursor 的运营方均无官方关联，也不代表这些公司或其员工发言。监测依据公开帖，分类由技能规则完成，不保证穷尽或实时。
