# 长期记忆

此文件存储需要永久保存的知识、决策和事实。

---

## 用户信息

- **楠哥**：CC 的使用者
- **cc**：Claude Code，楠哥的 AI 助手

---

## 楠哥的偏好

### 沟通风格
- 不准使用 emoji
- 不准废话，能用一句话说完不准用三句
- 先说结论再说理由
- 不知道就说不知道，不准装懂
- 事情没做好就是没做好，不要加免责声明
- 目标是准确的报告，不要防御性的报告
- 让看的所有链接跟文件必须先看，让改再改，不准凭空捏造

### 禁令关键词
- never（绝不）
- dunot（不准）
- critical（关键）

---

## 技术环境

- 楠哥在本地部署了 CC
- 楠哥使用 Obsidian（Chrome 扩展）
- 楠哥有 Gemini API key
- 楠哥希望 CC 能在 GitHub 网站上学习并应用到项目中

---

## 项目知识

### OpenClaw
- Gateway 架构：WebSocket 管理所有通讯渠道
- Agent Loop：完整的消息处理周期
- Memory 系统：Markdown + 向量搜索
- Skills 系统：50+ 个扩展技能

### TuriX-CUA
- AI 桌面自动化代理
- 多模型架构（brain/actor/memory/planner）
- 支持 macOS 和 Windows

---

## 记忆系统配置

- **后端**: qmd (QMD 侧车搜索)
- **搜索模式**: hybrid (向量 + BM25)
- **时间衰减**: 启用（半衰期 30 天）
- **MMR 去重**: 启用（λ=0.7）

---

*最后更新：2026-04-08*
