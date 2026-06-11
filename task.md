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
- 继续补译既有待处理文件：`Amp/amp-code.md`、`Microsoft Copilot/copilot-cli.md`、`Anthropic/visualize.md`、`Grok（xAI）/Features/grok-build.md`。

### 状态

- `✅ 已完成`：`Perplexity/perplexity-computer.md`、`Misc/docker-gordon-ai.md`、`Misc/zed-ai.md`、`VSCode Agent/vs-code-copilot-agent.md`、`Google/Gemini/gemini-3.5-flash-tools.json` 已完成中文翻译并提交。
- `⚠️ 待处理`：OpenAI / Gemini Markdown / Antigravity 本轮新增文件仍保留原文，待下一批翻译。

### 本轮待合并的翻译批次
- Anthropic 4.6 主提示词：`Anthropic/claude-opus-4.6.md`、`Anthropic/claude-opus-4.6-no-tools.md`
- Anthropic 4.6 Sonnet 系列：`Anthropic/claude-sonnet-4.6.md`、`Anthropic/claude-sonnet-4.6-no-tools.md`
- Anthropic raw：`Anthropic/raw/claude-opus-4.6-raw.md`、`Anthropic/raw/claude-sonnet-4.6-raw.md`

### 下一步处理原则
- 继续维持先补齐缺失原文再就地覆盖中文译文的策略，避免上游新增文件漏收。

## 2026-06-11 全英文文件扫描与补译

### 扫描方式

- 使用脚本遍历仓库内所有普通文件，跳过 `.git`，统计中文字符与英文字母数量。
- 判定标准：中文字符数为 0，且英文字母数大于 50 的文件视为“全英文待复核文件”。
- 工具定义 JSON 文件暂按原始结构保留，避免误翻译键名、工具字段或 schema。

### 本轮已完成翻译

- `Devin AI/后端开发与部署工作流程.txt`
- `Devin AI/前端部署工作流程.txt`
- `Devin AI/网络爬虫工作流程.txt`
- `VSCode Agent/vs-code-copilot-agent.md`

### 仍待后续分批处理的全英文文件

- `Misc/meta-ai.md`
- `Meta/meta-ai.md`
- `Microsoft Copilot/copilot-cli.md`
- `OpenAI/gpt-5.3-instant.md`
- `NotionAi/Notion-AI.md`
- `Amp/amp-code.md`
- `Bolt.new/prompts.txt`
- `Anthropic/claude-opus-4.6.md`
- `Anthropic/claude-desktop-code.md`
- `Anthropic/claude-sonnet-4.6.md`
- `Anthropic/claude-cowork.md`
- `Anthropic/Claude Sonnet 4.6.txt`
- `Anthropic/claude-sonnet-4.6-no-tools.md`
- `Anthropic/claude-opus-4.6-no-tools.md`
- `Anthropic/Features/claude-desktop-code.md`
- `Anthropic/Features/claude-cowork.md`
- `Anthropic/raw/claude-opus-4.6-raw.md`
- `Anthropic/raw/claude-sonnet-4.6-raw.md`
- `Anthropic/Core_Models/claude-3.7-full-system-message-with-all-tools.md`
- `Anthropic/Core_Models/claude-opus-4.6.md`
- `Anthropic/Core_Models/claude-sonnet-4.6.md`
- `Anthropic/Core_Models/Claude Sonnet 4.6.txt`
- `Anthropic/Core_Models/claude-sonnet-4.6-no-tools.md`
- `Anthropic/Core_Models/claude-opus-4.6-no-tools.md`
- `Anthropic/old/claude-3.7-full-system-message-with-all-tools.md`
- `Anthropic/Core_Models/raw/claude-opus-4.6-raw.md`
- `Anthropic/Core_Models/raw/claude-sonnet-4.6-raw.md`
- `Anthropic/Core_Models/old/claude-3.7-sonnet.md`
- `Anthropic/Core_Models/old/claude-opus-4.5.md`
- `OpenAI/Core_Models/gpt-5.4-thinking.md`
- `OpenAI/Core_Models/gpt-5.3-instant.md`
- `Cursor Prompts/Agents_Composer/Agent Prompt 2.0.txt`
- `Grok（xAI）/Features/grok-build.md`
- `Grok（xAI）/Features/grok-expert.md`
- `Grok（xAI）/Personalities/grok-personas.md`

### 暂不翻译的全英文工具定义文件

- `Bolt.new/tools.json`

## 2026-06-11 继续补译

### 本轮已完成

- `Google/Gemini/gemini-3.5-flash-tools.json`：翻译工具说明、参数说明与用法描述，保留 `name`、`type`、`required`、`enum` 等 JSON 结构字段和值。

### 说明

- 工具定义类文件仅翻译自然语言说明，保留函数名、参数名、枚举值、类型字段与 schema 结构，避免影响工具定义可读性与原始语义。
