# 上游同步任务（2026-04-13）

## 检查范围
- `upstream-x1xhlol/main`
- `upstream-asgeirtj/main`
- 对比基线：`origin/main`

## upstream-x1xhlol/main

### 主要更新
- 新增英文目录并迁移文件：`CodeBuddy Prompts/`、`Qoder/`、`Trae/`、`Z.ai Code/`。
- 多产品提示词与工具定义有批量更新（如 `Anthropic/`、`OpenAI/`、`Google/`、`VSCode Agent/`、`Windsurf/` 等）。
- 存在目录结构重排（如 Cursor 子目录上提、部分文件重命名/移动）。

### 本地已覆盖（含中文映射目录）
- `CodeBuddy Prompts/Chat Prompt.txt` -> `腾讯 CodeBuddy Prompts/Chat Prompt.txt`（已覆盖）
- `CodeBuddy Prompts/Craft Prompt.txt` -> `腾讯 CodeBuddy Prompts/Craft Prompt.txt`（已覆盖）
- `Qoder/prompt.txt` -> `阿里 Qoder/Qoder/prompt.txt`（已覆盖）
- `Qoder/Quest Action.txt` -> `阿里 Qoder/Qoder/Quest Action.txt`（已覆盖）
- `Qoder/Quest Design.txt` -> `阿里 Qoder/Qoder/Quest Design.txt`（已覆盖）
- `Trae/Builder Prompt.txt` -> `字节跳动（ByteDance）/Trae.ai/Builder Prompt.txt`（已覆盖）
- `Trae/Builder Tools.json` -> `字节跳动（ByteDance）/Trae.ai/Builder Tools.json`（已覆盖）
- `Trae/Chat Prompt.txt` -> `字节跳动（ByteDance）/Trae.ai/Chat Prompt.txt`（已覆盖）
- `Z.ai Code/prompt.txt` -> `智谱清言（Z.ai）/code-cli-prompt.txt`（已覆盖，文件名存在本地约定差异）

### 本次新增落地
- 文档侧新增：`task.md`、`CONTRIBUTING.md`。
- 提示词文件新增：`Anthropic/Claude Code 2.0.txt`、`Anthropic/Claude Code/Prompt.txt`、`Anthropic/Claude Code/Tools.json`、`Anthropic/Claude for Chrome/Prompt.txt`、`Anthropic/Claude for Chrome/Tools.json`、`Anthropic/Sonnet 4.5 Prompt.txt`、`Cursor Prompts/Agent CLI Prompt 2025-08-07.txt`、`Cursor Prompts/Agent Prompt 2.0.txt`、`Cursor Prompts/Agent Prompt 2025-09-03.txt`、`Cursor Prompts/Agent Prompt v1.0.txt`、`Cursor Prompts/Agent Prompt v1.2.txt`、`Cursor Prompts/Agent Tools v1.0.json`、`Cursor Prompts/Chat Prompt.txt`。

### 待后续处理
- 对 `Anthropic/Claude Sonnet 4.6.txt`、`Anthropic/`、`OpenAI/`、`Google/` 等大批量更新做逐文件差异核对与翻译同步。
- 评估是否引入上游英文目录重排，或继续维持本仓库中文目录映射策略。

## upstream-asgeirtj/main

### 主要更新
- 新增英文贡献指南：`CONTRIBUTING.md`。
- 大规模目录扁平化与重组：`OpenAI/`、`Google/`、`xAI/`、`Misc/` 增补/迁移明显。
- 模型版本文件更新密集（尤其 OpenAI Codex/GPT-5.x 与 Google Gemini 系列）。

### 本地已覆盖（含中文映射目录）
- `xAI/grok-3.md`、`xAI/grok-4.md` 等可映射到 `Grok（xAI）/Core_Models/`（已覆盖）
- `OpenAI/codex/gpt-5.md`、`OpenAI/codex/gpt-5.4.md` 等可映射到 `OpenAI/Codex/`（已覆盖）
- `Google/gemini-3-pro.md`、`Google/gemini-3-flash.md`、`Google/gemini-diffusion.md` 可映射到 `Google/Gemini/`（已覆盖）

### 本次新增落地
- 基于上游贡献规范新增本仓库中文版 `CONTRIBUTING.md`（见同目录文件）。

### 待后续处理
- `Misc/` 新增条目（如 `meta-ai.md`、`t3.chat.md` 等）本地尚未建立对应中文收录策略。
- 上游路径规范（如 `OpenAI/codex/` 小写子目录）与本地既有目录大小写/层级不一致，需统一规则后再批量同步。

## 本轮同步（2026-04-15）

### 已确认并从上游补齐的缺失文件
- `Anthropic/Claude Sonnet 4.6.txt`（来自 `upstream-x1xhlol/main`）
- `Anthropic/claude.ai-human-readable.md`
- `Anthropic/claude-cowork.md`
- `Anthropic/claude-desktop-code.md`
- `Anthropic/claude-opus-4.6.md`
- `Anthropic/claude-opus-4.6-no-tools.md`
- `Anthropic/claude-sonnet-4.6.md`
- `Anthropic/claude-sonnet-4.6-no-tools.md`
- `Anthropic/raw/claude-opus-4.6-raw.md`
- `Anthropic/raw/claude-sonnet-4.6-raw.md`
- `OpenAI/gpt-5.3-instant.md`
- `OpenAI/gpt-5.4-thinking.md`
- `Google/nano-banana-2-api.md`
- `Misc/meta-ai.md`

### 已有本地等价内容，暂不重复新建
- `OpenAI/`、`Google/`、`xAI/`、`Misc/` 中其余大部分新增路径，本地已有旧层级或中文映射版本，可在后续批次中按“是否需要保留上游新扁平路径”再决定是否补新文件。
- `Misc/Notion-AI.md`、`Misc/qwen-3.6-plus.md` 等条目已有本地同名或近似同名中文内容，优先在后续批次中决定是否保留双路径。

### 翻译批次状态
- 已启动子代理并行处理 Anthropic 4.6 系列、Anthropic 说明类文档、OpenAI/Google/Misc 增量翻译。
- 本轮先完成原文同步入库，避免遗漏；子代理产出的中文版本在下一步直接覆盖这些新文件。

### 待下一步处理
- 校对并落地 `Anthropic/Claude Sonnet 4.6.txt`、`Anthropic/claude-opus-4.6.md`、`Anthropic/claude-sonnet-4.6.md` 的完整中文译文。
- 评估是否补齐 `Anthropic/old/` 历史文件到本地，以便与 upstream-asgeirtj 的新结构对齐。
- 决定是否为 `OpenAI/`、`Google/`、`Misc/` 新扁平路径保留与旧层级并存的双轨收录策略。
## 本轮同步（2026-04-17）

### 上游增量检查结果
- 已重新抓取 `upstream-x1xhlol/main` 与 `upstream-asgeirtj/main`。
- 与上次自动化记录相比，`upstream-asgeirtj/main` 新增了 `Anthropic/Official/claude-opus-4.7.md`，并继续更新 `Anthropic/claude-opus-4.6.md`、`Anthropic/claude-sonnet-4.6.md`、`OpenAI/gpt-5.4-thinking.md` 等既有文件。
- `Anthropic/Official/README.md` 仅为上游档案链接说明，不属于新的提示词正文文件，当前先记录来源，不在本地单独建立对应中文文件。

### 本地缺失并已补齐的文件
- `Anthropic/Official/claude-opus-4.7.md` -> `Anthropic/claude-opus-4.7.md`

### 本轮待合并的翻译批次
- Anthropic 4.6 主提示词：`Anthropic/claude-opus-4.6.md`、`Anthropic/claude-opus-4.6-no-tools.md`
- Anthropic 4.6 Sonnet 系列：`Anthropic/claude-sonnet-4.6.md`、`Anthropic/claude-sonnet-4.6-no-tools.md`、`Anthropic/Claude Sonnet 4.6.txt`
- Anthropic 说明与辅助文档：`Anthropic/claude.ai-human-readable.md`、`Anthropic/claude-cowork.md`、`Anthropic/claude-desktop-code.md`、`Anthropic/claude-opus-4.7.md`
- Anthropic raw：`Anthropic/raw/claude-opus-4.6-raw.md`、`Anthropic/raw/claude-sonnet-4.6-raw.md`
- OpenAI / Google / Misc：`OpenAI/gpt-5.3-instant.md`、`OpenAI/gpt-5.4-thinking.md`、`Google/nano-banana-2-api.md`、`Misc/meta-ai.md`

### 下一步处理原则
- 继续维持“先补齐缺失原文，再就地覆盖中文译文”的策略，避免上游新增文件漏收。
- 对上游目录重排但本地已有稳定中文映射的路径，优先记录映射关系，不重复制造双份同义文件。

## 本轮同步（2026-05-06）

### 上游增量检查结果
- 已重新抓取 `upstream-x1xhlol/main`、`upstream-asgeirtj/main` 与 `origin/main`。
- 相比 2026-04-17 的自动化记录，`upstream-asgeirtj/main` 新增了 `Misc/cursor.md`，并更新了上游 `README.md`。
- `upstream-x1xhlol/main` 本轮未发现新的本地未覆盖提示词文件；仍以既有中文目录映射规则为准，不因上游重排重复落地同义路径。

### 本地缺失并已补齐的文件
- `upstream-asgeirtj/main:Misc/cursor.md` -> `Cursor Prompts/cursor.md`

### 本轮翻译批次
- Anthropic Opus 4.6：`Anthropic/claude-opus-4.6.md`、`Anthropic/claude-opus-4.6-no-tools.md`
- Anthropic Sonnet 4.6：`Anthropic/claude-sonnet-4.6.md`、`Anthropic/claude-sonnet-4.6-no-tools.md`、`Anthropic/Claude Sonnet 4.6.txt`
- Anthropic 辅助文档与 raw：`Anthropic/claude.ai-human-readable.md`、`Anthropic/claude-cowork.md`、`Anthropic/claude-desktop-code.md`、`Anthropic/raw/claude-opus-4.6-raw.md`、`Anthropic/raw/claude-sonnet-4.6-raw.md`
- OpenAI / Misc：`OpenAI/gpt-5.3-instant.md`、`OpenAI/gpt-5.4-thinking.md`、`Misc/meta-ai.md`
- Cursor：`Cursor Prompts/cursor.md`

### 下一步处理
- 合并本轮子代理产出的中文译文，并做 UTF-8 可读性、代码围栏与标签结构校验。
- 后续若 `upstream-asgeirtj/main` 的 `README.md` 再出现索引级变更，优先只同步本仓库需要的状态说明，不镜像无关英文说明。
- 对 `Misc/` 这类上游扁平目录新增文件，若本仓库已有稳定产品目录，应优先落入既有中文分类，不保留与现有结构冲突的双轨路径。

## 本轮同步（2026-05-15）

### 上游增量检查结果
- 已重新抓取 `origin/main`、`upstream-x1xhlol/main` 与 `upstream-asgeirtj/main`。
- `upstream-x1xhlol/main` 本轮相对 `origin/main` 仍以素材、目录重排和已覆盖文件为主；未发现新的本地未覆盖提示词正文文件。`Google/Gemini/AI Studio vibe-coder.txt` 这类大小写差异条目继续视作已被本地同名文件覆盖。
- `upstream-asgeirtj/main` 在 `4633f00..8affcd4` 间新增了大量扁平路径；按本仓库既有语义映射和文件名覆盖规则压缩后，真正需要补入的仅为少量新文件，而不是整批重复镜像。

### 已有本地等价内容，继续不重复新建
- `Google/gemini-in-chrome.md` -> `Google/Gemini/gemini_in_chrome.md`
- `Misc/kagi-assistant.md` -> `Kagi/Kagi Assistant.md`
- `Misc/notion-ai.md` -> `NotionAi/Notion AI.md`
- 其余 `OpenAI/`、`Anthropic/Features/`、`Anthropic/Tools_Plugins/`、`xAI/Personalities/` 等多数新增扁平路径，已可由本地旧层级同名文件承接，不再重复制造双轨文件。

### 本地缺失并已补齐的文件
- `upstream-asgeirtj/main:Anthropic/old/claude-3.7-full-system-message-with-all-tools.md` -> `Anthropic/old/claude-3.7-full-system-message-with-all-tools.md`
- `upstream-asgeirtj/main:Anthropic/visualize.md` -> `Anthropic/visualize.md`
- `upstream-asgeirtj/main:Google/gemini-youtube.md` -> `Google/Gemini/gemini-youtube.md`
- `upstream-asgeirtj/main:Misc/amp-code.md` -> `Amp/amp-code.md`
- `upstream-asgeirtj/main:Misc/copilot-cli.md` -> `Microsoft Copilot/copilot-cli.md`
- `upstream-asgeirtj/main:Misc/opencode.md` -> `Open Source prompts/OpenCode/opencode.md`
- `upstream-asgeirtj/main:Misc/t3-code.md` -> `t3.chat/t3-code.md`
- `upstream-asgeirtj/main:OpenAI/codex/gpt-5.3-codex-spark.md` -> `OpenAI/Codex/gpt-5.3-codex-spark.md`
- `upstream-asgeirtj/main:OpenAI/codex/plan_mode.md` -> `OpenAI/Codex/plan_mode.md`
- `upstream-asgeirtj/main:xAI/grok-expert.md` -> `Grok（xAI）/Features/grok-expert.md`

### 本轮翻译批次
- Anthropic 历史/辅助：`Anthropic/old/claude-3.7-full-system-message-with-all-tools.md`、`Anthropic/visualize.md`
- 产品文档：`Amp/amp-code.md`、`Microsoft Copilot/copilot-cli.md`、`Grok（xAI）/Features/grok-expert.md`
- 新增小批次：`Google/Gemini/gemini-youtube.md`、`Open Source prompts/OpenCode/opencode.md`、`t3.chat/t3-code.md`
- OpenAI Codex：`OpenAI/Codex/gpt-5.3-codex-spark.md`、`OpenAI/Codex/plan_mode.md`

### 下一步处理
- 本轮已完成中文落地：`Google/Gemini/gemini-youtube.md`、`Open Source prompts/OpenCode/opencode.md`、`t3.chat/t3-code.md`、`OpenAI/Codex/gpt-5.3-codex-spark.md`、`OpenAI/Codex/plan_mode.md`。
- 本轮仍待后续继续翻译：`Anthropic/old/claude-3.7-full-system-message-with-all-tools.md`、`Anthropic/visualize.md`、`Amp/amp-code.md`、`Microsoft Copilot/copilot-cli.md`、`Grok（xAI）/Features/grok-expert.md`。阻塞原因是部分子代理所在 worktree 继续命中 `windows sandbox: setup refresh failed with status exit code: 1`。
- 若后续继续追 `upstream-asgeirtj/main` 的扁平目录扩张，默认先做文件名/语义覆盖判断，再决定是否需要新增文件。

## 本轮同步（2026-05-24）

### 本轮判断
- `README.md` 只保留稳定项目说明、目录结构、贡献入口和正式上游来源，不再记录“本轮同步”“待处理”“结构清理中”这类运行态信息。
- `task.md` 继续作为自动同步记录、缺失文件判断、翻译批次和阻塞信息的唯一任务面。
- `.gitignore` 已明确忽略 `task.md` 与 `CONTRIBUTING.md`；同步时不把这些协作文件当作对外公开收录内容，也不要求在 `README.md` 中维护运行日志。
- `asgeirtj/system_prompts_leaks` 继续视为正式上游来源，与 `x1xhlol/system-prompts-and-models-of-ai-tools` 并行核对。

### 本轮覆盖核对
- 基于本地只读检查，`Amp/amp-code.md`、`Microsoft Copilot/copilot-cli.md`、`Open Source prompts/OpenCode/opencode.md`、`t3.chat/t3-code.md` 等 2026-05-15 已记录的新增文件仍已落地。
- 由于本轮 `git fetch` 受限于 worktree 下 `FETCH_HEAD` 写权限，无法安全刷新远端引用并确认 2026-05-24 时点是否还有新的未覆盖提示词正文文件。

### 当前阻塞
- `git -c safe.directory=... fetch --all --prune` 失败于 `C:/code/system-prompts-and-models-of-ai-tools-chinese/.git/worktrees/system-prompts-and-models-of-ai-tools-chinese4/FETCH_HEAD: Permission denied`。
- 在该阻塞解除前，本轮不能真实完成上游抓取、缺失文件下载、子代理翻译、提交和推送。

### 下轮继续
- 先恢复该 worktree 对 `.git/worktrees/.../FETCH_HEAD` 的写权限，随后重新执行 `git fetch --all --prune`。
- fetch 恢复后，优先核对 `upstream-asgeirtj/main` 与 `upstream-x1xhlol/main` 新增提示词正文，再决定是否需要补新文件和开启新一轮批量翻译。

## 本轮同步（2026-05-26）

### 本轮核对结果
- 已重新执行 `git fetch --all --prune`，确认 `upstream-x1xhlol/main` 仍为 `b8e95891fe6c8f1db651a8ca4d8217f22c73849b`，本轮没有新的远端前进。
- 已重新执行 `git fetch --all --prune`，确认 `upstream-asgeirtj/main` 前进到 `18516b700f2a4d135cbf5e6df3844d9d26d0e065`。
- 对 `6565e659072d371fb02a01e36d5e478a5fb6e58c..18516b700f2a4d135cbf5e6df3844d9d26d0e065` 做逐文件差异核对后，提示词正文层面实际新增/变更仅有 `xAI/grok-build.md` 这一项；此前公开 README 中出现的其他较新条目，本轮并不属于这段新增提交。
- 已按本仓库目录映射将 `upstream-asgeirtj/main:xAI/grok-build.md` 同步落地到 `Grok（xAI）/Features/grok-build.md`。

### 主仓库现状
- 主仓库 `C:/code/system-prompts-and-models-of-ai-tools-chinese` 处于 `main...origin/main [behind 4]`，且已经存在多处已修改/未跟踪文件，包含 `Anthropic/Claude_Code_CLI/claude-code.js`、`NotionAi/Notion AI.md`、`OpenAI/Codex/personality_friendly*.md` 以及一批未跟踪的 Anthropic / OpenAI / Meta 文件。
- 在这些现有改动未经人工确认前，本轮不应直接在主仓库执行拉取、覆盖或整理，以免把用户现有工作与自动同步内容混在一起。

### 当前状态
- 当前 worktree 的 fetch 阻塞已解除，本轮已完成上游增量核对与缺失文件补入。
- `Grok（xAI）/Features/grok-build.md` 当前先以同步上游原文入库，待下一轮按既有流程补齐中文译文。

### 下轮继续
- 优先补译 `Grok（xAI）/Features/grok-build.md`，并与 `Amp/amp-code.md`、`Microsoft Copilot/copilot-cli.md`、`Anthropic/visualize.md` 等历史待译文件一起纳入下一轮翻译批次。
- 若主仓库仍保留现有未提交改动，继续优先在独立 worktree 完成同步与翻译，避免污染用户当前 `main` 工作区。
