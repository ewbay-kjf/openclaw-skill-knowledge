# OpenClaw Skill Knowledge Base

## 概述

这是一个包含 OpenClaw 所有可用技能的知识库和技能查询技能。

## 内容

### 1. 技能知识库 (技能知识库.md)
包含 OpenClaw 所有可用技能的详细信息：
- 20个核心技能（基于 AGENTS.md）
- 系统技能目录中的所有技能
- 基础工具能力（read、write、exec等）
- 技能使用规则和触发原则

### 2. 技能查询技能 (skill-lookup.skill)
一个完整的技能查询技能，包括：
- SKILL.md - 技能描述和使用方法
- scripts/skill-search.sh - 技能搜索脚本
- scripts/update-skills.sh - 技能库更新脚本
- references/skill-categories.md - 技能分类指南
- references/usage-examples.md - 技能使用示例

### 3. 压缩包 (skill-knowledge.tar.gz)
包含完整的技能目录和知识库文件

## 如何使用

### 导入技能
1. 下载 `skill-lookup.skill` 文件
2. 在 OpenClaw 环境中导入技能：
   ```bash
   # 将 .skill 文件放入技能目录
   cp skill-lookup.skill /path/to/openclaw/skills/
   ```

### 使用技能查询技能
当用户询问以下问题时触发：
- "你有什么技能"
- "列出所有技能"
- "查看技能列表"
- "技能库"
- "技能查询"
- "OpenClaw 有哪些功能"
- "如何使用某个技能"

### 查看知识库
查看 `技能知识库.md` 文件了解所有技能的详细信息

## 技能目录结构

```
skill-lookup/
├── SKILL.md (技能主文件)
├── scripts/
│   ├── skill-search.sh (技能搜索脚本)
│   └── update-skills.sh (技能库更新脚本)
├── references/
│   ├── skill-categories.md (技能分类指南)
│   └── usage-examples.md (使用示例)
```

## 贡献

如果你想更新技能知识库：
1. 编辑 `技能知识库.md` 文件
2. 运行 `./scripts/update-skills.sh` 脚本
3. 重新打包技能

## 创建信息

创建于：2025年4月21日
作者：小宝 (OpenClaw AI Assistant)