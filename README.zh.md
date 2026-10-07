# Hi, I'm BiBoyang 👋🏻

All-in AI Agent 的全栈开发者，AI Native 开发者。
现在专攻多端 agent 应用架构、agent 记忆与评测。
曾经做 iOS 开发，主攻性能优化。热衷开源和创作，维护着 **45 个公开源码仓**：DeepSeek Harness（DSH）插件、一套自带完整性闸门的个人 agent skill 合集、原生 macOS 应用，以及一个 Rust 实验场——微信 Bot 和一个文件型 Agent 原型在里面一起演化。每个插件和 skill 都带 CI；每个 skill 都带自己的声明式评测。

## 🌍 在哪能找到我

- 📝 **博客** — [biboyang.github.io](https://biboyang.github.io/)
- 📖 **小册** — [《自顶向下拆 Agent：从界面到地基》](https://biboyang.github.io/books/agent-ui/)

## ▶ 从这里开始

两个打头项目：

| 项目 | 能给你什么 |
| --- | --- |
| dsh-eval-harness | DSH 插件评测工具：YAML 用例驱动真实 agent 回归评测，baseline 对比 PASS/WARN/FAIL 门禁 |
| dsh-im-bridge | DSH 插件：把 DeepSeek Harness 桥接到 IM（v0.1 微信/iLink；钉钉/飞书/Telegram 预留），turn/approval 推送 + 远程批准/注入，持久去重/收敛分段/合并窗口 |

## 🤖 Agent、插件与 Skill

| 项目 | 一句话 | 语言 | 许可证 |
| --- | --- | --- | --- |
| dsh-eval-harness | DSH 插件回归评测台：YAML 用例、真实 agent 运行、baseline 差异门禁 | TypeScript | — |
| dsh-im-bridge | 把 DeepSeek Harness 桥进 IM：推送 turn/审批，远程批准或注入文本 | TypeScript | — |
| huohou | 个人的 AI agent skill 合集——每个 skill 是一条练到成本能的工作纪律；`SKILL.md` + `references/` 渐进加载，每个 skill 内置 evals 与触发评测（P/R/F1） | Python | — |
| skill-quake | 面向 Agent Skill 的故障注入实验 + `skill-guard` 机械完整性闸门（地基只验收，评级是法官的事） | Python | Apache-2.0 |
| skills | 个人 Agent Skill 注册仓：`skills.yaml` 单源真理 + symlink 同步器 + CI 对每个 pin ref 跑 skill-guard 验收 | Shell | — |

## 🔧 上游与社区贡献

_下面每个仓都不属于 `BiBoyang/*`；第一张表里每一条都是**已合并**的 pull request，
2026-10-07 从本账号自己的 PR 历史重新数过。归属方一列写明项目是谁的——光看账号名
分不清那是公司还是个人。_

**已合并——3 个仓库共 6 条 PR：**

| 仓库 | ★ | 已合并 PR | 项目归属方 |
| --- | --- | --- | --- |
| awesome-dsh-plugin | 17,881 | [#12](https://github.com/awesome-dsh-plugin/awesome-dsh-plugin/pull/12)、[#13](https://github.com/awesome-dsh-plugin/awesome-dsh-plugin/pull/13) —— 把 dsh-im-bridge 和 dsh-eval-harness 收进精选列表 | `awesome-dsh-plugin` 社区组织——社区目录，背后没有公司 |
| Waza | 7,134 | [#26](https://github.com/tw93/Waza/pull/26) 中文技术文写作规则、[#82](https://github.com/tw93/Waza/pull/82) `check` skill 新增「质疑路线而不仅是 diff」、[#88](https://github.com/tw93/Waza/pull/88) 本地抓取层绕过系统代理——堵住隐私契约的漏洞 | tw93——个人维护者 |
| skill-up | 1,140 | [#257](https://github.com/alibaba/skill-up/pull/257) 修复符号链接 skill 源导致的零文件静默安装 | **阿里巴巴 Alibaba** —— 官方 `alibaba` 组织 |

**Open——5 个仓库共 6 条 PR（实测于 2026-10-07，每周复验）：**

_Open 就是 open：没合并，不吹。其中两条开在官方公司组织——**Anthropic** 和
**Microsoft**——把它们列出来恰恰因为还在 pending，而不是不管不顾。_

| 仓库 | ★ | Open PR | 项目归属方 |
| --- | --- | --- | --- |
| skills | 179,860 | [anthropics/skills#1949](https://github.com/anthropics/skills/pull/1949) —— skill-creator `quick_validate` 拒绝空 name/description 并校验引用文件存在性 | **Anthropic** —— 官方 `anthropics` 组织 |
| waku | 1,566 | [egoist/waku#161](https://github.com/egoist/waku/pull/161) —— 修复表格内拖选复制带出整行内容（Rust 命中判定从纯垂直距离改为二维包含） | egoist——个人维护者 |
| eval-guide | 138 | [microsoft/eval-guide#16](https://github.com/microsoft/eval-guide/pull/16) —— 修复重建说明里的过期路径 + 两条 frontmatter 非法 YAML | **Microsoft** —— 官方 `microsoft` 组织 |
| skill-up | 1,140 | [#295](https://github.com/alibaba/skill-up/pull/295) 拒绝无任何可识别 matcher 的空规则断言、[#281](https://github.com/alibaba/skill-up/pull/281) `validate --skill` 内容完整性 linter、[#265](https://github.com/alibaba/skill-up/pull/265) 截止杀掉进程后合成 session-result 产物 | **阿里巴巴 Alibaba** —— 官方 `alibaba` 组织 |

**已合并表里★最多的两行，一个是社区目录、一个是个人项目——表里写明了，而不是
让 star 数自己暗示。** 唯一的公司行是阿里的 `skill-up`——本账号自己的 `skill-quake`
和 `skills` 两个仓的闸门就围着这个评测引擎建，不只是用它，也给它交代码。`Waza`
的三条合并 PR 同样回流进了 `huohou` 以 skill 形式发布的写作与评审纪律；开给
Anthropic 和 Microsoft 的 open PR 把这条线延伸出去：完整性检查与正确性修复，
提在最能让生态感觉到的地方。

## 🍎 Apple 平台

| 项目 | 一句话 |
| --- | --- |
| Cove | 原生 macOS NAS 媒体播放器（Swift，MIT） |
| NotchLauncher | 住在刘海里的 macOS 启动器——悬停展开，点击启动（Swift，MIT） |
| ForgeLoop | Swift 编码 agent 项目：分层架构、流式输出、工具执行、取消语义（MIT） |
| ForgeLoopTUI | 轻量 Swift 终端 UI 库：流式 AI 输出原地更新 + 工具占位符（MIT） |
| BBYDebugTool | LogTool v0.1——Objective-C 日志工具，本账号最老的仓（最后提交于 2020-04） |

## 🦀 Rust 实验

| 项目 | 一句话 |
| --- | --- |
| AMClaw | 实验场：微信 iLink Bot（扫码登录、会话合并、记忆、熔断、日报/周报回传）+ 最小文件型 Agent 原型（Plan-aware ReAct、watchdog、LLM record/replay）；破坏性演进是特性 |
| AIvsAI | 双 AI 终端工具：Moonshot 先答，DeepSeek 审（MIT） |

_说明：上面 8 个仓是账号里★数最高的源码仓（按 star 排序，实测于 2026-10-07）。
其余 30 多个源码仓是学习档案、进行中的 fork 和小 demo，只在这里汇总点名。_

## ✍️ 写作

- **博客** — [biboyang.github.io](https://biboyang.github.io/) —— AI agent 工程、流式协议故障注入、skill 完整性实验、CI 误诊纪实；写「我具体错在哪条命令上」的那种文章
- **[《自顶向下拆 Agent：从界面到地基》](https://biboyang.github.io/books/agent-ui/)** —— 博客系列「自顶向下拆 Agent」全部篇目集结的网页版小册，从界面现象一路拆到上下文与协议地基

## 🚴 代码之外

- 📚 重度阅读者
- 🎮 游戏 —— 英雄联盟
- 🚴🏻 骑行 —— Trek Marlin 5 👍🏻👍🏻👍🏻，Marin Four Corners 👍🏻👍🏻👍🏻👍🏻👍🏻

* * *

**本页是重测出来的，不是记出来的。** Star 数、已合并 PR 数、仓库数据全部于
**2026-10-07** 对着 GitHub API 和本账号公开仓库列表重新实测，每张表都标了日期。
测不了的东西就标注清楚，不猜。
