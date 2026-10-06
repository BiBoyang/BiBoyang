# Hi, I'm BiBoyang 👋🏻

iOS developer (Objective-C / Swift) by trade, Rust developer by choice, AI-agent
builder by obsession. I maintain **45 public source repositories** — DeepSeek Harness
(DSH) plugins, a personal agent-skill collection with its own integrity gate, native
macOS apps, and a Rust playground where a WeChat bot and a file-based agent prototype
evolve side by side. Every plugin and skill ships with CI; every skill carries its own
declarative evals.

## 🌍 Where things live

- **GitHub** (this profile) — source and releases
- 📝 **Blog** — [biboyang.github.io](https://biboyang.github.io/) — 长文、实验与《自顶向下拆 Agent》小册

## ▶ Start here

Two repos lead the account, measured 2026-10-06:

| Repository | What it gives you | ★ |
| --- | --- | --- |
| dsh-eval-harness | DSH 插件评测工具：YAML 用例驱动真实 agent 回归评测，baseline 对比 PASS/WARN/FAIL 门禁 | 13 |
| dsh-im-bridge | DSH 插件：把 DeepSeek Harness 桥接到 IM（v0.1 微信/iLink；钉钉/飞书/Telegram 预留），turn/approval 推送 + 远程批准/注入，持久去重/收敛分段/合并窗口 | 10 |

## 🤖 Agents, plugins & skills

| Repository | One-liner | Language | License | ★ |
| --- | --- | --- | --- | --- |
| dsh-eval-harness | Regression eval harness for DSH plugins: YAML cases, real agent runs, baseline-diff gates | TypeScript | — | 13 |
| dsh-im-bridge | Bridge DeepSeek Harness into IM: push turns/approvals, approve or inject remotely | TypeScript | — | 10 |
| huohou | 个人的 AI agent skill 合集——每个 skill 是一条练到成本能的工作纪律；`SKILL.md` + `references/` 渐进加载，每 skill 内置 evals 与触发评测（P/R/F1） | Python | — | 2 |
| skill-quake | Fault-injection experiments for Agent Skills + `skill-guard`: the mechanical integrity gate (foundation accepts/rejects; grading is for judges) | Python | Apache-2.0 | 2 |
| skills | 个人 Agent Skill 注册仓：`skills.yaml` 单源真理 + symlink 同步器 + CI 对每个 pin ref 跑 skill-guard 验收 | Shell | — | — |

## 🔧 Upstream & community contributions

_Every repo below is external to `BiBoyang/*`; every entry in the first table is a
**merged** pull request, re-derived 2026-10-06 from this account's own pull-request
history. The owner column names who owns the project, because the account name alone
does not say whether that is a company or an individual._

**Merged — 6 pull requests across 3 repositories:**

| Repository | ★ | Merged PRs | 项目归属方 |
| --- | --- | --- | --- |
| awesome-dsh-plugin | 17,881 | [#12](https://github.com/awesome-dsh-plugin/awesome-dsh-plugin/pull/12), [#13](https://github.com/awesome-dsh-plugin/awesome-dsh-plugin/pull/13) — 收录 dsh-im-bridge 与 dsh-eval-harness 进精选列表 | `awesome-dsh-plugin` community org — the community catalog, no company behind it |
| Waza | 7,111 | [#26](https://github.com/tw93/Waza/pull/26) 中文技术文写作规则、[#82](https://github.com/tw93/Waza/pull/82) `check` skill 新增「质疑路线而不仅是 diff」、[#88](https://github.com/tw93/Waza/pull/88) 本地抓取层绕过系统代理——堵住隐私契约的漏洞 | tw93 — individual maintainer |
| skill-up | 493 | [#257](https://github.com/alibaba/skill-up/pull/257) 符号链接 skill 源导致零文件静默安装 + 修复 | **阿里巴巴 Alibaba** — the official `alibaba` org |

**Open — 7 pull requests across 6 repositories (measured 2026-10-06, re-checked weekly):**

_Open is open: not merged, not claimed. Two of these sit in official company orgs —
**Anthropic** and **Microsoft** — and they are listed here exactly because they are
still pending, not in spite of it._

| Repository | ★ | Open PR | 项目归属方 |
| --- | --- | --- | --- |
| skills | 179,860 | [anthropics/skills#1949](https://github.com/anthropics/skills/pull/1949) — skill-creator `quick_validate` 拒绝空 name/description 并校验引用文件存在性 | **Anthropic** — the official `anthropics` org |
| waku | 1,567 | [egoist/waku#161](https://github.com/egoist/waku/pull/161) — 修复表格内拖选复制带出整行内容（Rust 命中判定从纯垂直距离改为二维包含） | egoist — individual maintainer |
| eval-guide | 138 | [microsoft/eval-guide#16](https://github.com/microsoft/eval-guide/pull/16) — 修复重建说明里的过期路径 + 两条 frontmatter 非法 YAML | **Microsoft** — the official `microsoft` org |
| Qi_ObjcMsgHook | 135 | [QiShare/Qi_ObjcMsgHook#5](https://github.com/QiShare/Qi_ObjcMsgHook/pull/5) — fix fishhook bug | QiShare — individual maintainer |
| skill-up | 493 | [#295](https://github.com/alibaba/skill-up/pull/295) 拒绝无任何可识别 matcher 的空规则断言、[#281](https://github.com/alibaba/skill-up/pull/281) `validate --skill` 内容完整性 linter、[#265](https://github.com/alibaba/skill-up/pull/265) 截止杀掉进程后合成 session-result 产物 | **阿里巴巴 Alibaba** — the official `alibaba` org |

**The biggest merged row is a catalog and an individual's project, and the table says so
rather than letting the star count imply otherwise.** The merged company row is Alibaba's
`skill-up` — the eval engine this account's own `skill-quake` and `skills` repos build
their gates around, contributed to upstream instead of only consuming it. Three merged
pull requests in `Waza` also feed directly back into the writing and review disciplines
that `huohou` ships as skills; the open rows to Anthropic and Microsoft extend the same
line: integrity checks and correctness fixes, proposed where the ecosystem will feel them.

## 🍎 Apple platform

| Repository | One-liner | ★ |
| --- | --- | --- |
| Cove | A native macOS NAS media player (Swift, MIT) | 1 |
| NotchLauncher | A macOS launcher that lives in the notch — hover to reveal, click to launch (Swift, MIT) | — |
| ForgeLoop | Swift coding-agent project: layered architecture, streaming, tool execution, cancellation semantics (MIT) | — |
| ForgeLoopTUI | Lightweight Swift terminal UI library for streaming AI transcripts with in-place updates and tool placeholders (MIT) | 1 |
| BBYDebugTool | LogTool v0.1 — Objective-C logging utility, the account's oldest repo (last commit 2020-04) | 2 |

## 🦀 Rust experiments

| Repository | One-liner | ★ |
| --- | --- | --- |
| AMClaw | 实验场：微信 iLink Bot（扫码登录、会话合并、记忆、熔断、日报/周报回传）+ 最小文件型 Agent 原型（Plan-aware ReAct、watchdog、LLM record/replay）；破坏性演进是特性 | 2 |
| AIvsAI | Dual-AI terminal tool: Moonshot answers, DeepSeek reviews (MIT) | 1 |

*Counting note: the table above is the account's eight most-starred source repos — **32★**
together, measured 2026-10-06. The remaining 30+ source repos are learning archives,
forks-in-progress and small demos, named only in aggregate.*

## ✍️ Writing

- **Blog** — [biboyang.github.io](https://biboyang.github.io/) — AI agent 工程、流式协议故障注入、skill 完整性实验、CI 误诊纪实；写「我具体错在哪条命令上」的那种文章
- **[《自顶向下拆 Agent：从界面到地基》](https://biboyang.github.io/books/agent-ui/)** — 博客系列「自顶向下拆 Agent」全部篇目集结的网页版小册，从界面现象一路拆到上下文与协议地基

## 🚴 Beyond code

- 📚 Avid reader
- 🎮 Gaming — League of Legends
- 🚴🏻 Biking — Trek Marlin 5 👍🏻👍🏻👍🏻, Marin Four Corners 👍🏻👍🏻👍🏻👍🏻👍🏻

---

**中文介绍**

**主业 iOS（Objective-C / Swift），副业 Rust，正在 All-in AI Agent。** 这个账号维护
45 个公开源码仓：DeepSeek Harness 插件（评测门禁、IM 桥接）、一套带机械完整性闸门
的个人 agent skill 合集（火候）、原生 macOS 应用，以及一个 Rust 实验场——微信 Bot
和文件型 Agent 原型在里面一起演化。向上游也交代码：**6 条已合并的外部 PR**（阿里
skill-up、tw93 的 Waza、DSH 社区精选列表），另有 **7 条 open PR** 悬在 6 个外部仓上
——其中两条分别开在 Anthropic 官方 skills（179.9k★）和 Microsoft 官方 eval-guide，
逐条见上方 Upstream 一节。写作在博客 [biboyang.github.io](https://biboyang.github.io/)，
系列长文已集结成小册《自顶向下拆 Agent：从界面到地基》。上面的每个数字都带测量日期，
不复述第二份。

* * *

**This page is re-measured, not remembered.** Star counts, merged-pull-request counts
and repository figures were re-measured on **2026-10-06** against the GitHub API and the
account's public repository list, and each table says so. Anything that can't be measured
is labeled instead of guessed.
