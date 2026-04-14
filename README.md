# 🚀 Prompt Optimizer - 提示词优化器

<p align="center">
  <img src="https://img.shields.io/badge/OpenClaw-技能包-blue?style=for-the-badge&logo=rocket" alt="OpenClaw">
  <img src="https://img.shields.io/badge/版本-3.2-green?style=for-the-badge" alt="Version">
  <img src="https://img.shields.io/badge/Python-3.12+-yellow?style=for-the-badge" alt="Python">
  <img src="https://img.shields.io/badge/测试-57个通过-green?style=for-the-badge" alt="Tests">
</p>

> [!TIP]
> AI 任务处理器 - 先优化 Prompt，再精准执行

---

## ✨ 一句话介绍

**一个能把您的模糊需求自动翻译成 AI 能精准执行的指令的工具！**

---

## 🎯 能做什么？

### 原始需求 → 精准指令

| 您说 | 优化后 |
|------|--------|
| "帮我写个排序" | "你是一个专业工程师。帮我写个排序。请用 Markdown 格式输出..." |
| "查下天气" | "请提供准确、全面的信息，标注信息来源。查下天气。用 Markdown..." |
| "帮我debug报错" | "你是一个资深调试专家。请分析问题原因，提供完整的错误分析..." |
| "帮我写个测试用例" | "你是一个资深测试工程师。请编写完整的测试用例，覆盖主要场景..." |

---

## 📋 支持的任务类型 (20种)

| 类型 | 示例 |
|------|------|
| 写代码 | "帮我写个排序" |
| 代码审查 | "审查这段代码" |
| 改写代码 | "重构这段代码" |
| 写文档 | "帮我写个文档" |
| 写文案 | "写一段推广文案" |
| 总结摘要 | "帮我总结一下" |
| 翻译 | "翻译成英文" |
| 查资料 | "查一下深圳天气" |
| 数据分析 | "分析一下这份数据" |
| 头脑风暴 | "给我几个创业想法" |
| 生成内容 | "生成一张图片" |
| 数学计算 | "计算 123+456" |
| 对话聊天 | "聊聊AI的发展" |
| **写测试用例** | "帮我写单元测试" |
| **代码调试** | "帮我debug这个报错" |
| **性能优化** | "优化这段代码性能" |
| **安全检查** | "检查代码安全隐患" |
| **API设计** | "设计一个RESTful API" |
| **数据结构设计** | "设计一个高效的数据结构" |
| **处理文件** | "处理这个文件" |

---

## 🚀 快速开始

### 安装

```bash
# 克隆仓库
git clone https://github.com/ntaffffff/prompt-optimizer-skill.git
cd prompt-optimizer-skill
```

### 使用

```bash
# 基本用法
python prompt_optimizer.py "帮我写个排序"

# JSON 输出
python prompt_optimizer.py "帮我写个排序" --json

# 从文件批量处理
python prompt_optimizer.py --file input.txt

# 查看版本
python prompt_optimizer.py --version
```

---

## 📖 CLI 用法

```
用法: python prompt_optimizer.py [options] [prompt]

选项:
  -f, --file FILE        从文件读取 prompt（每行一个）
  -o, --output FILE      输出文件路径
  -j, --json             输出 JSON 格式
  -v, --verbose          显示详细信息
  -q, --quiet            静默模式
  --stats                显示统计信息
  -t, --types            显示支持的任务类型
  --cache / --no-cache   启用/禁用缓存
  --clear-cache          清空缓存
  -c, --config FILE      配置文件路径
  --version              显示版本号
  -h, --help             显示帮助信息
```

---

## 🆕 新功能 (v3.2)

### 新增任务类型 (7种)
- 写测试用例
- 代码调试
- 性能优化
- 安全检查
- API设计
- 数据结构设计
- 处理文件

### 新增输出格式 (11种)
- Markdown (默认)
- JSON
- YAML
- XML
- 纯文本
- 表格
- PlantUML
- 代码块
- HTML
- CSV
- Markdown表格

### 新增目标受众 (7种)
- 技术人员
- 产品经理
- 管理者
- 运维工程师
- 设计师
- 初学者
- 普通用户

---

## 🧪 测试

```bash
python test_prompt_optimizer.py

# 结果
📊 测试结果: 57 通过, 0 失败
```

---

## 📁 项目结构

```
prompt-optimizer/
├── SKILL.md                   # 技能文档
├── prompt_optimizer.py        # 主程序 (v3.2)
├── config_data.py             # 配置数据
├── test_prompt_optimizer.py   # 测试用例
├── _meta.json                 # 元数据
├── config.yaml.example        # 配置示例
└── .gitignore                 # Git忽略文件
```

---

## 🤖 在 OpenClaw 中使用

### 安装 Skill

```bash
# 方式1: 从 ClawHub 安装
npx clawhub@latest install prompt-optimizer-v3

# 方式2: 复制到 skills 目录
cp -r prompt-optimizer ~/.openclaw/workspace/skills/
```

### 自动优化

在 OpenClaw 中，每次执行任务前会自动用 prompt-optimizer 优化你的需求，生成更精准的指令。

---

## 📝 更新日志

### v3.2 (2026-04-14)
- ✅ 新增 7 种任务类型（共20种）
- ✅ 新增 7 种输出格式（共11种）
- ✅ 新增 7 种目标受众
- ✅ 新增约束条件（字数限制、条数限制）
- ✅ 57 个测试全部通过

### v3.1 (2026-04-07)
- ✅ 配置分离 - 独立 config_data.py
- ✅ LRU 缓存
- ✅ 31 个测试通过

---

## 👤 作者

- **作者**: dxx (AI 助手)
- **仓库**: [ntaffffff/prompt-optimizer-skill](https://github.com/ntaffffff/prompt-optimizer-skill)
- **OpenClaw**: https://openclaw.ai

---

<p align="center">
  <sub>Made with ❤️ by dxx</sub>
</p>