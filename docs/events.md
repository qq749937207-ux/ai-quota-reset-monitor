# 突发额度重置事件时间线

这是一份可核对、可贡献的公开事件时间线，记录各 AI 公司在**正常额度周期之外**的突发或额外重置、加赠、可储蓄一次性额度。

机器可读数据在 [`data/resets.yaml`](../data/resets.yaml)。两份文件保持同步：新增、修改或转正一条事件时，请同时改 YAML 和本页。

## 收录标准

- 只收录有可打开、可当场核对来源的突发或额外重置。没有原帖或官方链接的事件不写。
- **正式宣布**：官方或监测名单中的授权账号明确表示正在重置、已经重置，或发放可储蓄重置。计入下方「正式次数」。
- **高度疑似**：来自监测账号，尚未正式宣布，但强烈暗示即将或可能有一次额外重置。单独标记，**不计入正式次数**。
- 若疑似之后出现对应的正式宣布：只把原条目改为正式并注明确认来源，**不要再写一条正式事件重复计数**。
- 不算：路人猜测、无关玩笑、常规提额、限期加倍、套餐改价、单纯的产品发布、正常周期恢复、自动回复，以及仅向故障受影响用户发放的小范围补偿（除非来源明确向更大范围用户发放了额外重置）。
- 同一事件被多人宣布或转发只保留一条。产品线只写来源里明确说明的；未写明就标明不确定，不猜测。
- 通知和本页都用短结构：分类、北京时间、产品线与一句话要点、来源链接。不贴原文，不嵌帖卡。

## 时区

所有时间均为**北京时间（Asia/Shanghai，UTC+8）**。X 帖或官方页面若带 `Z` 或其他时区，已换算后再写入，不原样粘贴来源时区。

## 覆盖范围（初版）

本初版只写入 2026-11-12 当场用公开 X 读取能力核对过的事件，**不保证历史完整**。更早或遗漏的事件，欢迎按同样格式附可打开的来源补交。

检索与核对此窗口大致如下：

- **账号**：按 [`docs/accounts.md`](accounts.md) 的默认三家名单检索。重点核对实际会宣布额外重置的账号：OpenAI 以 @thsottiaux 为主，并检索了 @OpenAI、@OpenAIDevs、@OpenAINewsroom、@ChatGPT；xAI 以 @bot 原创公告为主，并检索了 @SpaceXSI、@grok、@SuperGrok、@elonmusk 中与重置相关的原创或短语匹配；Anthropic 以 @ClaudeDevs、@claudeai、@lydiahallie、@alexalbert__ 为主，并检索了 @AnthropicAI。
- **OpenAI**：已逐条核对 @thsottiaux 与重置相关的公开帖，窗口约为 **2026-05-16 至 2026-11-12**。该关键词检索在 2026-05-16 之前仍可能有更早结果，本版未继续逐条收录。公司官方号（@OpenAI、@OpenAIDevs、@OpenAINewsroom、@ChatGPT）的同类关键词全库检索未发现可单独计次的突发重置宣布，实际宣布主要来自 @thsottiaux。
- **xAI / Grok Bot**：已翻阅 @bot 排除回复与转帖后的原创时间线，从可翻到的最早原创帖（约 2026-08-21）至 2026-11-12；其中核对到 4 次面向用户的正式额外重置。对 @grok、@SpaceXSI、@SuperGrok 的原创（非回复）重置短语检索，以及 @elonmusk、@cursor_ai 中与 Grok 或重置相关的短语检索，未发现可另计的正式突发重置；@grok 的大量自动回复不收录。
- **Anthropic**：已逐条核对上述官方与员工号与重置相关的公开帖，窗口约为 **2026-05-15 至 2026-11-12**。该关键词检索在 2026-05-15 之前仍可能有更早结果，本版未继续逐条收录。2026-05-06 前后见到的是常规或限期提额，已排除。

核对过程中明确排除、因此未写入本时间线的例子包括：把付费档用量整体加倍等常规提额或套餐调整；限期提高每周或 Cowork 额度；仅提升 5 小时额度或 API 速率；效率优化使「同样额度用得更久」；仅向账单或展示错误所影响的用户补偿（例如约 4 万个限额不一致账户补发点数、某次可储蓄重置在两小时窗口内未生效而只向当时按下按钮的用户补发、约 3% 用户周额度显示错误后的小范围重置、把用量恢复到故障前状态）；第三方客户端攻击后的 API 点数退款；未见到落地宣布的重置预告（例如 2026-09-22 一则「周二会有重置」的预告，同窗口未见正式落地帖）；以及监测范围外路人或自动回复。

下方每家的「正式次数」和「最近一次」只统计本时间线里已经核对的正式条目，不是某家的历史全部次数，也不是会话里流传过、但未在本仓库逐条核对的数字。

## OpenAI（ChatGPT）

本时间线已核对的正式宣布：48 次，最近一次 2026-11-02。

　**高度疑似** · 2026-11-11 14:57（北京时间，Asia/Shanghai）
Codex · Tibo 暗示周四可能适合发放一次可储蓄重置，并点到 Codex；截至本条收录时尚未见到正式落地宣布。
[来源](https://x.com/thsottiaux/status/2120410480204525936)

　**正式宣布** · 2026-11-02 07:27（北京时间，Asia/Shanghai）
来源未写明产品线 · Tibo 宣布发放本轮可储蓄重置的第 2 张（共 2 张）。
[来源](https://x.com/thsottiaux/status/2117035794678546764)

　**正式宣布** · 2026-11-01 08:43（北京时间，Asia/Shanghai）
来源未写明产品线 · Tibo 宣布发放本轮可储蓄重置的第 1 张（共 2 张）。
[来源](https://x.com/thsottiaux/status/2116692529970311254)

　**正式宣布** · 2026-10-28 10:42（北京时间，Asia/Shanghai）
来源未写明产品线 · Tibo 在「第 23 天」更新中宣布当天进行一次额度重置。
[来源](https://x.com/thsottiaux/status/2115273064481218829)

　**正式宣布** · 2026-10-26 13:21（北京时间，Asia/Shanghai）
来源未写明产品线 · Tibo 在「第 21 天」更新中宣布当天进行一次额度重置。
[来源](https://x.com/thsottiaux/status/2114588174249071102)

　**正式宣布** · 2026-10-25 11:39（北京时间，Asia/Shanghai）
来源未写明产品线 · Tibo 在「第 20 天」更新中宣布进行一次额度重置。
[来源](https://x.com/thsottiaux/status/2114200152701575656)

　**正式宣布** · 2026-10-23 12:46（北京时间，Asia/Shanghai）
来源未写明产品线 · Tibo 在「第 18 天」更新中宣布进行一次额度重置。
[来源](https://x.com/thsottiaux/status/2113492187770175603)

　**正式宣布** · 2026-10-22 14:55（北京时间，Asia/Shanghai）
来源未写明产品线 · Tibo 在「第 17 天」更新中宣布当天为重置日。
[来源](https://x.com/thsottiaux/status/2113162277688070445)

　**正式宣布** · 2026-10-20 14:33（北京时间，Asia/Shanghai）
来源未写明产品线 · Tibo 在「第 15 天」更新中宣布进行一次额度重置。
[来源](https://x.com/thsottiaux/status/2112432076767289678)

　**正式宣布** · 2026-10-18 00:20（北京时间，Asia/Shanghai）
来源未写明产品线 · Tibo 在「第 13 天」更新中宣布进行一次额度重置。
[来源](https://x.com/thsottiaux/status/2111492673890824348)

　**正式宣布** · 2026-10-15 12:55（北京时间，Asia/Shanghai）
来源未写明产品线 · Tibo 在「第 10 天」更新中宣布进行一次额度重置。
[来源](https://x.com/thsottiaux/status/2110595484180214059)

　**正式宣布** · 2026-10-13 09:03（北京时间，Asia/Shanghai）
来源未写明产品线 · Tibo 在「第 8 天」更新中宣布进行一次全局额度重置，并说明将于当天美西时间结束前落地。
[来源](https://x.com/thsottiaux/status/2109812216212099456)

　**正式宣布** · 2026-10-11 06:15（北京时间，Asia/Shanghai）
来源未写明产品线 · Tibo 在「第 6 天」更新中宣布进行一次全局额度重置，并说明将于当天结束前落地。
[来源](https://x.com/thsottiaux/status/2109045220411351517)

　**正式宣布** · 2026-10-08 03:19（北京时间，Asia/Shanghai）
来源未写明产品线 · Tibo 宣布向所有付费账户发放一张可储蓄重置。
[来源](https://x.com/thsottiaux/status/2107913674593644711)

　**正式宣布** · 2026-10-07 11:35（北京时间，Asia/Shanghai）
来源未写明产品线 · Tibo 宣布已根据社区投票完成一次额度重置。
[来源](https://x.com/thsottiaux/status/2107676072871600470)

　**正式宣布** · 2026-10-02 10:14（北京时间，Asia/Shanghai）
ChatGPT · Tibo 宣布将于次日 10:00 PST 为所有付费 ChatGPT 账户进行一次全局额度重置。
[来源](https://x.com/thsottiaux/status/2105843926221660585)

　**正式宣布** · 2026-09-26 08:07（北京时间，Asia/Shanghai）
Codex、ChatGPT Work · Tibo 宣布将为 Codex 与 ChatGPT Work 的所有付费用户重置用量额度。
[来源](https://x.com/thsottiaux/status/2103637477760311522)

　**正式宣布** · 2026-09-12 11:20（北京时间，Asia/Shanghai）
ChatGPT · Tibo 向 Astra 用户宣布将在当天午夜前落地一次额度重置，并说明已修复若干质量问题。
[来源](https://x.com/thsottiaux/status/2098612714704891959)

　**正式宣布** · 2026-09-08 03:24（北京时间，Asia/Shanghai）
来源未写明产品线 · Tibo 宣布将为所有付费订阅做一次全局用量重置，计划于当天 18:00 PST 左右落地。
[来源](https://x.com/thsottiaux/status/2097043464538264003)

　**正式宣布** · 2026-09-05 08:39（北京时间，Asia/Shanghai）
ChatGPT · Tibo 宣布当天再为所有 Plus、Pro 与 Business 用户发放一次完整的可储蓄重置，于当天结束前落地。
[来源](https://x.com/thsottiaux/status/2096035437299237298)

　**正式宣布** · 2026-09-04 07:12（北京时间，Asia/Shanghai）
ChatGPT · Tibo 宣布：付费 ChatGPT 方案中尚未获得 Astra 的用户，每缺一天将获发一张可储蓄重置，首张约三小时内到账。
[来源](https://x.com/thsottiaux/status/2095651088502591861)

　**正式宣布** · 2026-08-31 03:24（北京时间，Asia/Shanghai）
Codex、ChatGPT Work · Tibo 宣布 Codex 与 ChatGPT Work 的额度重置将于 18:00 PST 落地，次日确认已为所有付费订阅完成，以庆祝活跃用户达到 2500 万。
[来源](https://x.com/thsottiaux/status/2094144275957350900)

　**正式宣布** · 2026-08-30 04:43（北京时间，Asia/Shanghai）
Codex、ChatGPT Work · Tibo 宣布为 Codex 与 ChatGPT Work 的所有付费用户重置用量，并说明近期修复了多项导致额外耗用的问题。
[来源](https://x.com/thsottiaux/status/2093801758665715784)

　**正式宣布** · 2026-08-23 14:11（北京时间，Asia/Shanghai）
来源未写明产品线 · Tibo 宣布将在次日修复 Codex 用量问题的同时，为所有付费订阅做一次完整用量重置。
[来源](https://x.com/thsottiaux/status/2091407991736332689)

　**正式宣布** · 2026-08-21 19:43（北京时间，Asia/Shanghai）
Codex、ChatGPT Work · Tibo 宣布为庆祝 Codex 活跃用户达到 2000 万，将在当天向每名 Codex 与 ChatGPT Work 用户发放一张可自行使用的可储蓄重置。
[来源](https://x.com/thsottiaux/status/2090766694897619318)

　**正式宣布** · 2026-08-13 09:01（北京时间，Asia/Shanghai）
来源未写明产品线 · Tibo 在提到 Codex 活跃用户已超过 1500 万的同时，宣布将在约一小时内为大家落地一次额度重置。
[来源](https://x.com/thsottiaux/status/2087706104814023111)

　**正式宣布** · 2026-08-11 08:28（北京时间，Asia/Shanghai）
ChatGPT Work、Codex · Tibo 宣布已为所有付费 ChatGPT Work 与 Codex 用户重置用量额度。
[来源](https://x.com/thsottiaux/status/2086972933566857393)

　**正式宣布** · 2026-08-09 04:29（北京时间，Asia/Shanghai）
ChatGPT Work、Codex · Tibo 宣布已为 ChatGPT Work 与 Codex 的所有付费用户重置用量额度。
[来源](https://x.com/thsottiaux/status/2086188036493344823)

　**正式宣布** · 2026-08-01 11:32（北京时间，Asia/Shanghai）
Codex、ChatGPT Work · Tibo 宣布已为 Codex 与 ChatGPT Work 重置用量额度。
[来源](https://x.com/thsottiaux/status/2083395449814229287)

　**正式宣布** · 2026-07-29 12:09（北京时间，Asia/Shanghai）
ChatGPT Work、Codex · Tibo 宣布已为所有 ChatGPT Work 与 Codex 用户重置用量，并说明针对 GPT-5.6 Sol 耗用偏快做了效率修复。
[来源](https://x.com/thsottiaux/status/2082317452755751098)

　**正式宣布** · 2026-07-28 11:09（北京时间，Asia/Shanghai）
Codex、ChatGPT Work · Tibo 宣布已为 Codex 与 ChatGPT Work 的所有付费用户重置用量额度。
[来源](https://x.com/thsottiaux/status/2081940052154933696)

　**正式宣布** · 2026-07-26 03:17（北京时间，Asia/Shanghai）
Codex、ChatGPT Work · Tibo 在说明前一晚发生过全局故障并已恢复后，宣布已为所有 Codex 与 ChatGPT Work 用户重置用量。
[来源](https://x.com/thsottiaux/status/2081096447718723984)

　**正式宣布** · 2026-07-22 00:47（北京时间，Asia/Shanghai）
Codex、ChatGPT Work · Tibo 为庆祝活跃用户达到 1000 万，宣布将为 Codex 与 ChatGPT Work 的付费用户再做一次用量重置，约一小时内落地。
[来源](https://x.com/thsottiaux/status/2079609157934886975)

　**正式宣布** · 2026-07-18 11:28（北京时间，Asia/Shanghai）
Codex、ChatGPT Work · Tibo 宣布为 Codex 与 ChatGPT Work 的所有付费用户重置用量额度。
[来源](https://x.com/thsottiaux/status/2078320950488297917)

　**正式宣布** · 2026-07-16 12:14（北京时间，Asia/Shanghai）
Codex、ChatGPT Work · Tibo 宣布为庆祝较早达到 900 万活跃用户，再为 Codex 与 ChatGPT Work 用户做一次用量重置，并称周额度将很快恢复满额。
[来源](https://x.com/thsottiaux/status/2077607697487188198)

　**正式宣布** · 2026-07-15 03:34（北京时间，Asia/Shanghai）
Codex、ChatGPT Work · Tibo 宣布 Codex 与 ChatGPT Work 活跃用户达到 800 万，并再次为所有用户重置用量额度。
[来源](https://x.com/thsottiaux/status/2077114635308986427)

　**正式宣布** · 2026-07-14 02:29（北京时间，Asia/Shanghai）
Codex、ChatGPT Work · Tibo 为庆祝 700 万活跃用户，宣布已向每名用户账户发放一张可储蓄重置，可在桌面应用或网页端使用以补满周用量。
[来源](https://x.com/thsottiaux/status/2076735790567338203)

　**正式宣布** · 2026-07-13 01:59（北京时间，Asia/Shanghai）
Codex、ChatGPT Work · Tibo 宣布活跃用户达到 600 万，并将在约一小时内落地一次用量重置。
[来源](https://x.com/thsottiaux/status/2076365965915467978)

　**正式宣布** · 2026-07-11 13:54（北京时间，Asia/Shanghai）
ChatGPT Work、Codex · Tibo 宣布再为所有 ChatGPT Work 与 Codex 用户做一次用量重置，约 30 分钟内落地。
[来源](https://x.com/thsottiaux/status/2075820987833274448)

　**正式宣布** · 2026-07-11 01:59（北京时间，Asia/Shanghai）
Codex、ChatGPT Work · Tibo 宣布已为 Codex 与 ChatGPT Work 重置用量，并预告当天稍后还有一次。
[来源](https://x.com/thsottiaux/status/2075641131002700120)

　**正式宣布** · 2026-07-10 05:24（北京时间，Asia/Shanghai）
ChatGPT Work、Codex · Tibo 宣布为 ChatGPT Work 与 Codex 做一次完整用量重置，约一小时内传播到位。
[来源](https://x.com/thsottiaux/status/2075330198887940337)

　**正式宣布** · 2026-06-30 07:39（北京时间，Asia/Shanghai）
Codex · Tibo 在公布 Codex 耗用调查结果的同时，宣布将再做一次完整用量重置，并额外向重置库发放一张可在 24 小时内自行使用的重置。
[来源](https://x.com/thsottiaux/status/2071740419030053227)

　**正式宣布** · 2026-06-29 07:54（北京时间，Asia/Shanghai）
Codex · Tibo 在调查仍在进行时宣布，已对所有人的 Codex 用量做一次硬重置。
[来源](https://x.com/thsottiaux/status/2071381664853319742)

　**正式宣布** · 2026-06-27 07:39（北京时间，Asia/Shanghai）
Codex · Tibo 宣布向所有 Codex 用户发放一次用量重置，并称将在数小时内显示到账户中。
[来源](https://x.com/thsottiaux/status/2070653282440405046)

　**正式宣布** · 2026-06-18 08:10（北京时间，Asia/Shanghai）
Codex · Tibo 宣布为 Codex 用户同时发放一次即时完整重置，以及一张可自行使用的可储蓄重置。
[来源](https://x.com/thsottiaux/status/2067399435009622521)

　**正式宣布** · 2026-06-04 08:25（北京时间，Asia/Shanghai）
Codex · Tibo 在说明 Codex 近 24 小时发生过多次可靠性故障后，宣布已为所有付费方案重置 Codex 用量。
[来源](https://x.com/thsottiaux/status/2062329981548802523)

　**正式宣布** · 2026-05-31 23:25（北京时间，Asia/Shanghai）
Codex · Tibo 宣布已为所有付费 ChatGPT 订阅重置 Codex 用量，周额度与小时额度均恢复满额。
[来源](https://x.com/thsottiaux/status/2061106703446450392)

　**正式宣布** · 2026-05-24 04:14（北京时间，Asia/Shanghai）
Codex · Tibo 宣布已回滚一项影响长会话缓存命中率的优化，并为所有账户重置了用量。
[来源](https://x.com/thsottiaux/status/2058280452851638313)

　**正式宣布** · 2026-05-17 01:51（北京时间，Asia/Shanghai）
Codex · Tibo 宣布已为所有付费方案重置 Codex 用量。
[来源](https://x.com/thsottiaux/status/2055707616605835333)

## xAI（Grok，含 Grok Bot）

本时间线已核对的正式宣布：4 次，最近一次 2026-11-10。

　**正式宣布** · 2026-11-10 03:17（北京时间，Asia/Shanghai）
Grok Bot · Grok Bot 官方账号宣布已为所有 Grok Bot 用户重置每周额度。
[来源](https://x.com/bot/status/2119871982946971659)

　**正式宣布** · 2026-10-03 02:05（北京时间，Asia/Shanghai）
Grok Bot · Grok Bot 官方账号宣布已为所有 Grok Bot 用户重置用量额度。
[来源](https://x.com/bot/status/2106083136002310193)

　**正式宣布** · 2026-09-06 02:24（北京时间，Asia/Shanghai）
Grok Bot · Grok Bot 官方账号宣布已为所有 Grok Bot 用户重置用量额度。
[来源](https://x.com/bot/status/2096303514230423629)

　**正式宣布** · 2026-08-27 01:23（北京时间，Asia/Shanghai）
Grok Bot · Grok Bot 官方账号在扩大订阅准入的同时，宣布也为所有用户重置每周用量额度。
[来源](https://x.com/bot/status/2092664183334846840)

## Anthropic（Claude）

本时间线已核对的正式宣布：13 次，最近一次 2026-11-11。

　**正式宣布** · 2026-11-11 05:59（北京时间，Asia/Shanghai）
Claude · ClaudeDevs 宣布已向所有 Pro、Max、Ultra 与 Team 用户发放一次覆盖全部模型与额度的免费完整重置，可在 12 月 10 日 14:00 PT 前随时使用。
[来源](https://x.com/ClaudeDevs/status/2120275296637321476)

　**正式宣布** · 2026-11-10 03:04（北京时间，Asia/Shanghai）
Claude · ClaudeDevs 宣布随 Fable 5.2 上线发放专项重置：Ultra 与 Team Premium 按订阅时长获 1 至 3 次、须在 3 月 8 日前使用；Pro 与 Team Standard 另有一周试用并附一次重置。
[来源](https://x.com/ClaudeDevs/status/2119868704544711108)

　**正式宣布** · 2026-09-23 00:31（北京时间，Asia/Shanghai）
Claude · Claude 官方账号宣布向订阅用户发放一次可储蓄的速率限制重置，可自行选择使用时间；同线程开发者账号写明对象为 Pro、Max 与 Team，并可使用至 10 月 22 日。
[来源](https://x.com/claudeai/status/2102435538120691886)

　**正式宣布** · 2026-09-05 04:08（北京时间，Asia/Shanghai）
Claude Max · Lydia Hallie 宣布刚为所有 Claude Max 方案用户重置了每周额度。
[来源](https://x.com/lydiahallie/status/2095967323412930677)

　**正式宣布** · 2026-09-02 02:35（北京时间，Asia/Shanghai）
Claude · ClaudeDevs 宣布在 Fable 5.1 发布的同时，已为所有用户重置 5 小时额度与每周额度。
[来源](https://x.com/ClaudeDevs/status/2094856679250919746)

　**正式宣布** · 2026-07-16 11:58（北京时间，Asia/Shanghai）
Claude · ClaudeDevs 宣布已为所有用户重置 5 小时与每周速率限制。
[来源](https://x.com/ClaudeDevs/status/2077603834453770467)

　**正式宣布** · 2026-07-10 02:01（北京时间，Asia/Shanghai）
Claude · ClaudeDevs 宣布已为所有用户重置 5 小时与每周速率限制。
[来源](https://x.com/ClaudeDevs/status/2075279141352706215)

　**正式宣布** · 2026-07-02 05:16（北京时间，Asia/Shanghai）
Claude · ClaudeDevs 宣布已再次为所有人重置 5 小时与每周速率限制。
[来源](https://x.com/ClaudeDevs/status/2072429181565288665)

　**正式宣布** · 2026-06-20 08:05（北京时间，Asia/Shanghai）
Claude · ClaudeDevs 宣布已为所有方案的所有用户重置 5 小时与每周用量限制。
[来源](https://x.com/ClaudeDevs/status/2068122937308426676)

　**正式宣布** · 2026-06-13 10:24（北京时间，Asia/Shanghai）
Claude · ClaudeDevs 宣布已为所有用户重置 5 小时与每周速率限制。
[来源](https://x.com/ClaudeDevs/status/2065621176735646006)

　**正式宣布** · 2026-06-10 05:48（北京时间，Asia/Shanghai）
Claude · ClaudeDevs 宣布已为所有用户重置 5 小时与每周速率限制。
[来源](https://x.com/ClaudeDevs/status/2064464557951852643)

　**正式宣布** · 2026-06-02 01:35（北京时间，Asia/Shanghai）
Claude · ClaudeDevs 宣布已为所有 Pro 与 Max 方案用户重置 5 小时与每周速率限制，并说明修复了部分 Claude Code 会话过度并行子代理、耗用偏快的问题。
[来源](https://x.com/ClaudeDevs/status/2061501787769893055)

　**正式宣布** · 2026-05-16 02:00（北京时间，Asia/Shanghai）
Claude · ClaudeDevs 宣布已为所有人重置 5 小时与每周速率限制。
[来源](https://x.com/ClaudeDevs/status/2055347539923308703)
