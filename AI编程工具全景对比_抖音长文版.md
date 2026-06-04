> 说明：抖音长文发布时，直接复制正文内容（去掉本说明行），粘贴至抖音「发布长文」入口即可。
> 抖音长文格式要求：每段不超过3-4行，善用空行和emoji分隔，话题标签统一置于文末。

---

你用会员刷视频，却不知道它能帮你写代码？

我在 Windows 上同时开了四个 AI 编程 CLI，实测了一圈，发现一个很多人都不知道的事：

手上的会员，大概率已经够用了。

· · ·

【四大 CLI 同屏跑，这是我的配置】

🟦 左上：Claude Code × Claude Opus 4.8
→ Claude Pro / Max 会员 或 Anthropic API Key，二选一

🟧 右上：Grok CLI × Grok 3 Mini
→ SuperGrok 订阅 或 xAI API Key，二选一

🟩 左下：Gemini CLI × Gemini Advanced
→ Google One AI Premium 会员 或 Gemini API Key，二选一

🟥 右下：Codex CLI × GPT-5.5 medium
→ ChatGPT Plus 会员 或 OpenAI API Key，二选一

· · ·

【最关键的结论，一条就够】

✅ 四款 CLI 全部同时支持：订阅/会员 和 API Key 两种接入方式

有哪个会员，就直接用哪个会员跑；
没有订阅、或者想要更大用量，买对应的 API Key 接上就行。

两条路都通，不存在只能选一种的情况。

· · ·

【四个 CLI 怎么选？我的实际体感】

🥇 Claude Code —— 日常编码、大项目首选
上下文窗口最大、推理最稳，复杂任务交给它最放心

🥈 Gemini CLI —— 轻量问答、快速验证
免费额度慷慨，随手一问不心疼

🥉 Grok CLI —— 快速响应、多任务并行
Plan Mode + 多 Agent 并行，节奏感强

🏅 Codex CLI —— 追求最新模型的选择
GPT-5.5 加持，内核已用 Rust 重写，性能不含糊

· · ·

【装好了怎么启动？一行命令速查】

Claude Code：
npm install -g @anthropic-ai/claude-code → 启动：claude

Gemini CLI：
npm install -g @google/gemini-cli → 启动：gemini

Codex CLI：
npm install -g @openai/codex → 启动：codex
⚠️ 包名必须带 @openai/ 前缀，裸 codex 是无关旧包

Grok Build：
Mac/Linux：curl -fsSL https://x.ai/cli/install.sh | bash → 启动：grok
Windows：irm https://x.ai/cli/install.ps1 | iex

前置要求：Node.js ≥ 20（Codex 要求 22+，Claude Code 要求 18+）

· · ·

【除了这四个，还有哪些选择？】

国外还有：
· Cursor —— 最流行的 AI IDE，$20/月，图形界面最友好
· Devin Desktop（原 Windsurf）—— 多 Agent 指挥中心，可同时管理多个 AI 任务
· 以上两个是 IDE，不是纯 CLI，适合不喜欢命令行的人

国内这几个也很能打：

🔶 CodeBuddy（腾讯）
插件 + IDE + CLI 三形态全覆盖，微信扫码登录，国内网络丝滑

🔶 Trae（字节）
原 MarsCode 改名，有 SOLO 模式，还开源了 Trae Agent

🔶 Qoder（阿里）
有独立 IDE 和 CLI，Quest 工作台可以跨项目并行跑 Agent

🔶 Kimi Code（月之暗面）
纯工具流派，CLI + 插件，API Key 还能接入 Claude Code 等第三方

· · ·

【一句话选型指南】

命令行重度用户：Claude Code > Codex CLI > Gemini CLI > Grok Build

想要图形界面：Cursor / Trae / CodeBuddy IDE

多 Agent 并行管理：Devin Desktop / Qoder Quest

国内网络不想折腾：CodeBuddy（微信登录最省事）

已有会员，直接接上对应 CLI：
Claude Pro / Max → Claude Code
Google One AI Premium → Gemini CLI
ChatGPT Plus → Codex CLI
SuperGrok → Grok Build

没有订阅也没关系，买 API Key 同样能跑：
Anthropic API Key → Claude Code
Gemini API Key → Gemini CLI
OpenAI API Key → Codex CLI
xAI API Key → Grok Build

· · ·

【官网/文档地址整理】

国外：
· Claude Code → code.claude.com/docs
· Gemini CLI → geminicli.com
· Codex → developers.openai.com/codex
· Grok Build → x.ai/cli
· Cursor → cursor.com
· Devin Desktop → devin.ai

国内：
· CodeBuddy → copilot.tencent.com
· Trae → trae.cn
· Qoder → qoder.com
· Kimi Code → kimi.com/code

· · ·

你手上有哪几个会员？

评论区报一下，我帮你看看现在的配置能接哪几套 CLI，怎么搭最划算👇

#AI编程 #程序员 #ClaudeCode #命令行工具 #开发者工具 #Gemini #ChatGPT #编程效率 #AI工具 #码农日常
