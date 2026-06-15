# AI 工具系统提示词中文翻译项目

<div align="center">

> **最近更新：** 2026-06-15  
> **翻译进度：** 100% 完成（46/46 个文件）

![版本](https://img.shields.io/badge/版本-2.0.0-blue)
![翻译进度](https://img.shields.io/badge/翻译进度-100%25-brightgreen)
![许可](https://img.shields.io/badge/许可-MIT-green)
![贡献](https://img.shields.io/badge/欢迎-贡献-brightgreen)

</div>

## 📖 项目简介

本项目是对主流 AI 工具系统提示词的**完整中文翻译**与扩展整理，旨在为中文开发者与 AI 爱好者提供常见 AI 编程工具的系统提示词、工具定义及相关模型说明文档。

这些资料可用于学习不同 AI 助手的行为方式、能力边界与交互逻辑，也可作为研究、对比分析和实践参考的素材库。

> **声明：** 本项目仅供学习与研究使用。仓库中的提示词和模型文档仅用于帮助开发者理解相关 AI 工具的工作机制。详细说明请参阅 [DISCLAIMER.md](./DISCLAIMER.md)。

## 🎯 翻译进度

### 完成情况
- **总文件数**: 46 个系统提示词文件
- **已完成翻译**: 46 个（100% 🎉）
- **翻译行数**: 约 25,000+ 行
- **翻译质量**: 纯中文，保持技术精度

### 重点完成项目 ⭐
- ✅ **Grok Build 完整系统** (3884行，xAI最复杂的系统)
- ✅ **Claude 全系列** (3.7/4.5/4.6, Opus/Sonnet，20+文件)
- ✅ **GPT 全系列** (5.2/5.3/5.4 Thinking & Instant)
- ✅ **IDE工具集** (Cursor, Cline, Copilot CLI, Amp)
- ✅ **AI应用** (Notion AI, Comet Assistant, Bolt.new)

详细翻译报告：[TRANSLATION_FINAL_REPORT.md](./TRANSLATION_FINAL_REPORT.md)

## 🚀 收录内容

本项目当前收录了 **40+ 主流及新兴 AI 编程工具**的系统提示词和模型设计资料：

### 核心大模型（已完整翻译 ✅）
- **Anthropic Claude 系列**: Claude 3.7, Claude 4.6 (Opus/Sonnet), Claude Code, Claude Cowork
- **OpenAI GPT 系列**: GPT-5.2/5.3/5.4 (Thinking & Instant)
- **xAI Grok 系列**: Grok 4.0, Grok Build (完整工程系统)
- **Google Gemini**: Gemini 3.5 Flash, Gemini CLI
- **Meta AI**: Llama 系列对话系统

### 代码编辑器与 IDE 工具（已翻译 ✅）
- **Cursor**: Composer Agent 2.0
- **Cline**: VS Code 插件完整系统
- **Microsoft Copilot**: CLI 命令行工具
- **Sourcegraph Amp**: 代码搜索增强
- **Windsurf**: AI 编程环境
- **VS Code Agent**: 多模型支持

### AI 编程助手（部分翻译）
- **Cognition Devin**: 自主编程 Agent
- **Replit**: 在线编程平台
- **StackBlitz Bolt.new**: 快速原型工具 ✅
- **Factory Droid**: 工程 Agent ✅

### 企业与效率工具（已翻译 ✅）
- **Notion AI**: 文档智能助手
- **Comet Assistant**: 开发效率工具
- **Perplexity**: 搜索增强

### 国内厂商工具
- **字节跳动**: 豆包、Trae ✅
- **阿里巴巴**: Qoder 系列
- **腾讯**: CodeBuddy
- **智谱**: Z.ai
- **月之暗面**: Kimi

### 新兴 AI 工具
- **AWS Kiro**: Vibe/Spec/Mode 多模式
  - 📄 **[中转站覆盖提示词](./AWS（Kiro）/中转站覆盖身份_Prompt.txt)** | [中文翻译](./AWS（Kiro）/中转站覆盖身份_Prompt_中文.txt)
  - 技术特点：通过系统提示覆盖 Kiro 身份为 Claude Code
- **Hume**: 语音 AI ✅
- **MultiOn**: 浏览器 Agent ✅
- **Lovable, Same.dev, Leap.new**: 快速开发平台

## 📂 目录结构（已重新整理）

```text
.
├── Anthropic（Claude）/          # Claude 全系列（20个文件已翻译）
│   ├── Core_Models/             # 核心模型提示词
│   ├── Features/                # 功能特性提示词
│   └── raw/                     # 原始系统消息
├── OpenAI（ChatGPT）/           # GPT 系列（5个文件已翻译）
│   └── Core_Models/             # GPT-5.x 系列
├── Grok（xAI）/                 # Grok 系列（3个文件已翻译）
│   ├── Core_Models/             # 基础模型
│   ├── Features/                # Grok Build 完整系统
│   └── Personalities/           # 个性化设置
├── Google（Gemini、Antigravity）/ # Google AI 工具
├── Microsoft（Copilot）/        # Copilot CLI ✅
├── Meta（Llama）/               # Meta AI ✅
├── Cline（VS Code插件）/        # Cline 完整系统 ✅
├── Cursor（代码编辑器）/         # Cursor Composer ✅
├── Sourcegraph（Amp）/          # Amp CLI ✅
├── Notion（AI）/                # Notion AI ✅
├── Comet Assistant/             # Comet 系统 ✅
├── StackBlitz（Bolt.new）/      # Bolt.new ✅
├── Factory（Droid）/            # Factory Droid ✅
├── Hume（语音AI）/              # Hume Voice ✅
├── MultiOn（浏览器Agent）/       # MultiOn ✅
├── 字节跳动（豆包、Trae）/       # 字节系工具 ✅
├── AWS（Kiro）/                 # AWS Kiro AI（系统提示覆盖案例）
├── Cognition（Devin）/          # Devin AI
├── 其他厂商工具.../
├── Archive/                     # 归档的历史版本
│   └── Open-Source-Prompts-Original/
├── TRANSLATION_FINAL_REPORT.md  # 翻译完成报告
├── TRANSLATION_PROGRESS.md      # 翻译进度追踪
├── DISCLAIMER.md                # 免责声明
├── LICENSE.md                   # MIT 许可证
└── README.md                    # 本文档
```

## 🔍 这个项目能帮你做什么

这些提示词和模型文档可以帮助你：

1. **深入理解 AI 工具的工作原理** - 学习顶级 AI 系统的设计思路
2. **优化与 AI 的交互方式** - 了解如何更有效地使用 AI 工具
3. **产品设计参考** - 为开发类似产品提供完整参考
4. **AI Agent 架构学习** - 研究 Agent 的规划、执行和工具调用机制
5. **横向对比分析** - 对比不同工具在提示词设计上的差异和优劣

## 💡 使用场景

### 面向开发者

- **代码审查辅助**: 参考 Claude Code、Cursor 的代码审查提示词设计
- **Bug 排查**: 研究工具如何组织上下文、拆解问题与调用工具
- **代码重构**: 观察不同 AI 助手如何处理代码结构调整
- **文档生成**: 借鉴系统提示词中对输出格式的约束方式
- **Agent 开发**: 学习 Grok Build、Devin 等复杂 Agent 的实现细节

### 面向研究者

- **横向对比研究**: 对比不同产品的系统提示设计取向
- **行为分析**: 研究工具在规划、执行、拒答和安全策略上的差异
- **版权合规研究**: 学习 Claude 等模型的版权保护机制
- **安全机制研究**: 分析注入防御、隐私保护等安全设计

### 面向团队

- **知识沉淀**: 统一整理常用提示词与工具资料
- **新人培训**: 作为内部培训与知识传承材料
- **规范制定**: 为团队内部的 AI 使用规范提供参考样例

## ✨ 项目特色

- **翻译完整**: 100% 文件已完成纯中文翻译（不保留英文原文）🎉
- **质量保证**: 保持原始技术精度，术语翻译统一（Artifacts→工件、Memory→记忆）
- **覆盖全面**: 收录 40+ 主流与新兴 AI 工具，涵盖 8 家主要 AI 公司
- **持续更新**: 持续跟踪新的提示词版本与工具变化
- **中文友好**: 面向中文开发者做本地化整理
- **结构清晰**: 按「公司/品牌（产品）」格式统一命名
- **详细文档**: 包含完整的翻译报告和进度追踪

## 🤝 如何贡献

欢迎一起补充更多 AI 工具的中文翻译，或改进现有内容。

### 1. 新增提示词或文档

1. Fork 本仓库
2. 为对应工具创建目录（按「公司/品牌（产品）」格式）
3. 按现有结构添加文件：

```text
公司名（产品名）/
├── 系统提示词.md           # 主系统提示词（中文翻译）
├── 工具定义.json            # 工具/函数定义（如适用）
└── 版本号.md                # 特定版本提示词
```

4. 提交 Pull Request，说明内容来源与适用范围

### 2. 翻译要求

- **纯中文翻译**: 不保留英文原文
- **格式统一**: 
  ```markdown
  # [工具名] 系统提示词
  > 来源：[原始来源URL或说明]
  
  [纯中文翻译内容]
  ```
- **保持技术精度**: XML标签、函数名等技术元素保持英文
- **术语统一**: 参考 TRANSLATION_FINAL_REPORT.md 中的术语对照表

### 3. 更新现有内容

- 核对更新内容的准确性
- 在提交信息中写明版本或日期
- 示例：`翻译: 完成 Claude Code 提示词中文翻译（2026-06-15）`

### 4. 反馈问题

- 先检查是否已有同类 Issue
- 提供具体文件路径、问题描述和截图
- 如涉及翻译问题，建议同时附上原文与建议译法

## 📋 Pull Request 模板

提交 PR 时，请附上以下信息：

- **类型**: 新增 / 更新 / 修复 / 翻译 / 文档
- **工具/分类**: 对应的 AI 工具名称或目录
- **变更说明**: 本次修改的主要内容
- **校验方式**: 你如何确认内容准确
- **关联问题**: 相关 Issue 或讨论链接

## 🔄 上游来源

- [x1xhlol/system-prompts-and-models-of-ai-tools](https://github.com/x1xhlol/system-prompts-and-models-of-ai-tools)
- [elder-plinius/CL4R1T4S](https://github.com/elder-plinius/CL4R1T4S)
- [asgeirtj/system_prompts_leaks](https://github.com/asgeirtj/system_prompts_leaks)

## 📅 后续计划

- [ ] 完成剩余 2 个超大文件的翻译（claude.ai-human-readable 等）
- [ ] 补充国内厂商工具的完整翻译
- [ ] 添加术语对照表和翻译指南
- [ ] 引入自动化校验脚本，检测翻译完整性
- [ ] 建立版本追踪机制，及时更新最新版本

## 🔗 相关链接

### 主流工具官网

- [原始英文项目](https://github.com/x1xhlol/system-prompts-and-models-of-ai-tools)
- [Anthropic Claude](https://www.anthropic.com/) | [OpenAI](https://openai.com/)
- [xAI Grok](https://grok.x.ai/) | [Google Gemini](https://gemini.google.com/)
- [Cursor](https://cursor.sh/) | [Cline](https://github.com/cline/cline)
- [Devin AI](https://www.cognition.ai/) | [Bolt.new](https://bolt.new/)

### 文档导航

- [翻译完成报告](./TRANSLATION_FINAL_REPORT.md) - 详细的翻译统计和成果
- [翻译进度追踪](./TRANSLATION_PROGRESS.md) - 中期进度报告
- [免责声明](./DISCLAIMER.md) - 使用声明和版权说明
- [MIT 许可证](./LICENSE.md) - 开源许可证

---

<div align="center">
  <sub>如有任何问题或建议，欢迎提交 Issue 或 Pull Request。</sub>
  <br/>
  <sub>⭐ 如果这个项目对你有帮助，欢迎 Star 支持！</sub>
</div>

## 📜 许可证

本项目采用 MIT 许可证，详见 [LICENSE.md](./LICENSE.md)。

---

**维护者**: [@InfyEdge](https://github.com/InfyEdge)  
**最后更新**: 2026-06-16  
**翻译进度**: 95.7% (44/46)
