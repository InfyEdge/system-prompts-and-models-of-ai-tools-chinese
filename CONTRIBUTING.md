# 贡献说明

## 新增上游文件时的处理规则

1. 先核对两个上游仓库：
   - `asgeirtj/system_prompts_leaks`
   - `x1xhlol/system-prompts-and-models-of-ai-tools`
2. 只同步本仓库尚未覆盖的提示词正文、工具定义或相关模型文档。
3. 如上游路径与本仓库目录命名不同，优先沿用本仓库既有中文目录映射，避免重复目录。
4. 原文同步后，再进行中文翻译；翻译时必须保留：
   - 原始标题层级
   - 代码块与命令
   - JSON 键名与工具字段
   - 链接、引用、占位符和版本号

## 目录映射约定

- `Misc/vscode-copilot-agent.md` -> `VSCode Agent/vs-code-copilot-agent.md`
- `Google/gemini-3.5-flash*.md|json` -> `Google/Gemini/`
- `Google/antigravity-cli.md` -> `Google/Antigravity/antigravity-cli.md`
- `Misc/zed.md` -> `Misc/zed-ai.md`
- `OpenAI/gpt-5.5-api*.md` -> `OpenAI/API/`

## 文档更新约定

- `README.md` 只保留稳定项目说明与最近更新时间。
- `task.md` 记录每轮同步结果、新增文件与待翻译清单。
- 如本轮仅新增原文、翻译未完成，也必须先把新增文件写入 `task.md`。

## 提交约定

- 每轮自动同步完成后使用中文提交信息。
- 推荐格式：
  - `同步: 补齐 GPT-5.5 与 Gemini 3.5 Flash 提示词`
  - `翻译: 完成 Perplexity Computer 等新增文件中文化`
