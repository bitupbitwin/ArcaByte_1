# 2026 年 AI 编程工具全景对比（国内 + 国外）

> 整理时间：2026 年 6 月
> 维度：形态（IDE / 插件 / CLI / 云端 Agent）+ CLI 安装启动命令 + 实测会员可用性

---

## 0. 实测：Windows 上四大 AI CLI 同屏运行

在 Windows 上同时运行四个 AI CLI 的真实配置：

| 位置 | 工具 | 模型 | 计费方式 |
|---|---|---|---|
| 左上 | **Claude Code** | Claude Opus 4.8 | Claude Pro / Max 会员额度 |
| 右上 | **Grok CLI** | Grok 3 Mini | SuperGrok 订阅 **或** xAI API Key |
| 左下 | **Gemini CLI** | Gemini Advanced | Google One AI Premium 会员 |
| 右下 | **Codex CLI** | GPT-5.5 medium | ChatGPT Plus 会员 |

**关键结论：**

- **Claude、Gemini、ChatGPT（Codex）三家都能直接用各自的会员额度，无需额外充值 API。**
- **Grok 支持两种方式：开通 SuperGrok 订阅可直接使用；也可以单独购买 xAI API Key。**

**基于这套配置的快速推荐：**

- 日常编码 / 大项目：优先 **Claude Code**（上下文最强、推理最稳）
- 快速问答 / 轻量任务：**Gemini CLI** 或 **Grok CLI**
- 需要最新模型 / 极致性能：**Codex CLI**（GPT-5.5）

---

## 一、国外产品

### Cursor（Anysphere）
- **形态**：AI 原生 IDE（VS Code 分支），当前最流行
- **特点**：内置 Agent 模式，可自主多步执行；$20/月
- **CLI**：另有 Cursor CLI / Agent，主力仍是 IDE

### Devin Desktop（Cognition，原 Windsurf）
- **形态**：AI IDE + 多 Agent 指挥中心
- **特点**：2026 年 6 月 2 日由 Windsurf 正式更名为 Devin Desktop，OTA 更新，配置/插件无缝迁移；默认界面变为 Agent Command Center（看板式管理本地 + 云端 Agent）；支持 ACP 协议，可接入 Claude Agent、Codex 等
- **关联产品**：Devin Cloud（云 Agent）、Devin CLI、Devin Review
- **注**：旧的 Cascade 已弃用，2026 年 7 月 1 日彻底移除，由 Devin Local 取代

### Claude Code（Anthropic）
- **形态**：纯终端 Agent
- **特点**：命令行编程 Agent，另有 VS Code / JetBrains 插件和桌面 App
- **计费**：Claude Pro / Max 会员额度直接可用，无需单独购买 API

### Gemini CLI（Google）
- **形态**：开源终端 Agent（Apache 2.0）
- **特点**：有免费额度，VS Code 配套插件，支持 MCP
- **计费**：Google One AI Premium 会员直接可用

### Codex（OpenAI）
- **形态**：CLI + 插件 + 桌面 App + 云端，全形态
- **特点**：Codex CLI（终端）、Codex IDE 插件（VS Code/Cursor 等）、Codex 桌面 App、Codex Web（云端）；内核已由 Node 重写为 Rust
- **计费**：ChatGPT Plus 会员直接可用

### Grok Build（xAI）
- **形态**：官方终端 Agent
- **特点**：2026 年 5 月 14 日早期 beta；多 Agent 并行、Plan Mode、支持 ACP / MCP / 技能市场
- **计费**：**SuperGrok 订阅**可直接使用；也支持单独购买 xAI API Key
- **注**：另有第三方社区版 grok-cli（非 xAI 官方）

---

## 二、国内产品

### Qoder（阿里巴巴）
- **形态**：AI IDE + CLI + Agent 工作台
- **特点**：基于 VS Code 改造的独立编辑器；Quest 由 IDE 内 Agent 模式升级为独立的智能体自主开发工作台（Qoder 1.0），可跨项目并行；Qoder CLI 于 2025 年 10 月发布

### CodeBuddy（腾讯云）
- **形态**：插件 + IDE + CLI，业内首个三形态全覆盖
- **特点**：CodeBuddy 插件（VSCode/JetBrains，含 Craft 智能体）、CodeBuddy IDE（对话即编程，面向产/设/研及零基础）、CodeBuddy Code（CLI）；微信登录，国内网络友好

### Trae（字节跳动）
- **形态**：IDE + 插件 + CLI + 开源 Agent
- **特点**：Trae IDE（原 MarsCode，含 SOLO 模式）、Trae 插件、企业版 CLI 接入、开源的 Trae Agent（GitHub）

### Kimi Code（月之暗面）
- **形态**：CLI + 插件，纯工具非 IDE
- **特点**：Kimi Code CLI（已从 Python 迁移至 Node.js）、VS Code 插件；提供 API Key 可接入 Claude Code 等第三方工具

---

## 三、CLI 安装与启动命令速查表

| 产品 | 安装命令 | 启动命令 |
|---|---|---|
| **Claude Code** | `npm install -g @anthropic-ai/claude-code` | `claude` |
| **Gemini CLI** | `npm install -g @google/gemini-cli`<br>或 `brew install gemini-cli` | `gemini` |
| **Codex CLI** | `npm install -g @openai/codex`<br>或 `brew install --cask codex`<br>或 Mac/Linux：`curl -fsSL https://chatgpt.com/codex/install.sh \| sh` | `codex` |
| **Grok Build（xAI 官方）** | Mac/Linux：`curl -fsSL https://x.ai/cli/install.sh \| bash`<br>Windows：`irm https://x.ai/cli/install.ps1 \| iex` | `grok` |
| **Qoder CLI（阿里）** | `npm install -g @qoder-ai/qodercli`<br>或 Mac/Linux：`curl -fsSL https://qoder.com/install \| bash`<br>或 `brew install qoderai/qoder/qodercli --cask` | `qodercli` |
| **CodeBuddy Code（腾讯）** | `npm install -g @tencent-ai/codebuddy-code`<br>或 `brew install Tencent-CodeBuddy/tap/codebuddy-code` | `codebuddy` |
| **Kimi Code CLI** | 见官网 kimi.com/code（Node.js 全局安装） | `kimi` |
| **Trae CLI（字节）** | 企业版提供，以官方文档为准 | — |

> **通用前置**：npm 安装的 CLI 基本要求 Node.js ≥ 20/22（Codex 要求 22+，Claude Code 要求 18+）。
> **避坑**：Codex 包名务必是 `@openai/codex`，不带 scope 的 `codex` 是无关旧包。
> **Windows**：Qoder CLI 在 Git Bash 报错，需用 Windows Terminal；CodeBuddy 同理推荐 npm 方式。
> **验证安装**：装好后用 `xxx --version` 看版本号，能输出即成功。

---

## 三点五、官网 / CLI 文档地址

**国外**

| 产品 | 官网 | 文档 / 仓库 |
|---|---|---|
| Cursor | cursor.com | — |
| Devin Desktop（原 Windsurf） | devin.ai | docs.devin.ai |
| Claude Code | claude.com/product/claude-code | code.claude.com/docs |
| Gemini CLI | geminicli.com | github.com/google-gemini/gemini-cli |
| Codex | developers.openai.com/codex | github.com/openai/codex |
| Grok Build | x.ai/cli | — |

**国内**

| 产品 | 官网 | 文档 |
|---|---|---|
| Qoder | qoder.com | qoder.com/install |
| CodeBuddy（腾讯） | copilot.tencent.com | codebuddy.ai/docs/zh/cli/installation |
| Trae（字节） | trae.cn | — |
| Kimi Code（月之暗面） | kimi.com/code | kimi.com/code/docs |

---

## 四、形态总览对比

| 产品 | 厂商 | IDE | 插件 | CLI | 云/Web Agent | 核心定位 |
|---|---|---|---|---|---|---|
| Cursor | Anysphere | ✅ 原生 | — | ✅ | — | 最流行 AI IDE |
| Devin Desktop | Cognition | ✅ 原生 | — | ✅ | ✅ Devin Cloud | IDE+多 Agent 指挥中心 |
| Claude Code | Anthropic | — | ✅ | ✅ 主 | — | 纯终端 Agent |
| Gemini CLI | Google | — | ✅ | ✅ 主 | — | 开源终端 Agent |
| Codex | OpenAI | — | ✅ | ✅ | ✅ Codex Web | 全形态 |
| Grok Build | xAI | — | — | ✅ 主 | — | 官方终端 Agent |
| Qoder | 阿里 | ✅ 原生 | — | ✅ | ✅ Quest | IDE+Agent 工作台 |
| CodeBuddy | 腾讯 | ✅ 原生 | ✅ | ✅ | — | 全形态（首家） |
| Trae | 字节 | ✅ 原生 | ✅ | ✅ | — | IDE+开源 Agent |
| Kimi Code | 月之暗面 | — | ✅ | ✅ | — | CLI+插件 |

---

## 五、会员可用性速查

| 工具 | 是否可用现有订阅 | 说明 |
|---|---|---|
| Claude Code | ✅ | Claude Pro / Max 会员直接可用 |
| Gemini CLI | ✅ | Google One AI Premium 会员直接可用 |
| Codex CLI | ✅ | ChatGPT Plus 会员直接可用 |
| Grok Build | ✅ / 可选 | SuperGrok 订阅可用；或单独购买 xAI API Key |
| 其他国内工具 | 各有不同 | 以各官网最新计费说明为准 |

---

## 六、选型速记

- **想要图形界面、上手最快**：Cursor / Trae / CodeBuddy IDE
- **重度命令行、追求自动化**：Claude Code / Codex CLI / Gemini CLI / Grok Build
- **多 Agent 并行管理**：Devin Desktop / Qoder Quest
- **国内网络环境友好、免登录门槛低**：CodeBuddy（微信登录）/ Qoder / Trae / Kimi Code
- **全形态都要、灵活切换**：CodeBuddy（首家插件+IDE+CLI）
- **已有会员想最大化利用**：Claude Pro → Claude Code；Google One → Gemini CLI；ChatGPT Plus → Codex CLI；SuperGrok → Grok Build
