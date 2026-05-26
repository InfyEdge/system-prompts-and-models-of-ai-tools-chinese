# 任务记录

## 2026-05-26 上游同步

### 已确认上游

- `asgeirtj/system_prompts_leaks`
- `x1xhlol/system-prompts-and-models-of-ai-tools`

### 本轮核对结论

- `x1xhlol/system-prompts-and-models-of-ai-tools` 本轮未发现需要新增到本仓库的未覆盖提示词正文文件。
- `asgeirtj/system_prompts_leaks` 本轮发现 11 个需要补齐到本仓库的新文件，其中正文 10 个、工具定义 1 个。
- 同步原则：优先保持本仓库现有中文目录结构与命名，不重复引入已由本地映射覆盖的英文目录。

### 本轮新增文件

- `OpenAI/gpt-5.5-instant.md`
- `OpenAI/API/gpt-5.5-api.md`
- `OpenAI/API/gpt-5.5-pro-api.md`
- `Perplexity/perplexity-computer.md`
- `VSCode Agent/vs-code-copilot-agent.md`
- `Misc/docker-gordon-ai.md`
- `Google/Gemini/gemini-3.5-flash.md`
- `Google/Gemini/gemini-3.5-flash-ai-studio.md`
- `Google/Gemini/gemini-3.5-flash-tools.json`
- `Google/Antigravity/antigravity-cli.md`
- `Misc/zed-ai.md`

### 上游到本地映射

- `OpenAI/gpt-5.5-instant.md` -> `OpenAI/gpt-5.5-instant.md`
- `OpenAI/gpt-5.5-api.md` -> `OpenAI/API/gpt-5.5-api.md`
- `OpenAI/gpt-5.5-pro-api.md` -> `OpenAI/API/gpt-5.5-pro-api.md`
- `Perplexity/perplexity-computer.md` -> `Perplexity/perplexity-computer.md`
- `Misc/vscode-copilot-agent.md` -> `VSCode Agent/vs-code-copilot-agent.md`
- `Misc/docker-gordon-ai.md` -> `Misc/docker-gordon-ai.md`
- `Google/gemini-3.5-flash.md` -> `Google/Gemini/gemini-3.5-flash.md`
- `Google/gemini-3.5-flash-ai-studio.md` -> `Google/Gemini/gemini-3.5-flash-ai-studio.md`
- `Google/gemini-3.5-flash-tools.json` -> `Google/Gemini/gemini-3.5-flash-tools.json`
- `Google/antigravity-cli.md` -> `Google/Antigravity/antigravity-cli.md`
- `Misc/zed.md` -> `Misc/zed-ai.md`

### 待下一步处理

- 完成以下新增 Markdown 文件的中文翻译，保持标题层级、列表结构、代码块和链接不变：
  - `OpenAI/gpt-5.5-instant.md`
  - `OpenAI/API/gpt-5.5-api.md`
  - `OpenAI/API/gpt-5.5-pro-api.md`
  - `Google/Gemini/gemini-3.5-flash.md`
  - `Google/Gemini/gemini-3.5-flash-ai-studio.md`
  - `Google/Antigravity/antigravity-cli.md`
- 复核 `Google/Gemini/gemini-3.5-flash-tools.json` 是否只需保留原始工具定义，避免误翻译键名。
- 继续补译既有待处理文件：`Amp/amp-code.md`、`Microsoft Copilot/copilot-cli.md`、`Anthropic/visualize.md`、`Grok（xAI）/Features/grok-build.md`。

### 状态

- `🔄 进行中`：新增文件已同步到本地。
- `✅ 已完成`：`Perplexity/perplexity-computer.md`、`Misc/docker-gordon-ai.md`、`Misc/zed-ai.md`、`VSCode Agent/vs-code-copilot-agent.md` 已完成中文翻译并提交。
- `⚠️ 待处理`：OpenAI / Gemini / Antigravity 本轮新增文件仍保留原文，待下一批翻译。
