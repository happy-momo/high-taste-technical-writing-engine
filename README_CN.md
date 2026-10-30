<p align="center">
  <a href="README.md">English</a> | <a href="README_CN.md">中文</a>
</p>

<h1 align="center">High-Taste Technical Writing Engine</h1>

<p align="center">
  <strong>一套面向技术内容创作的高标准写作 Skill 规范，强调品味、作者感、工程判断与克制表达。</strong>
  <br/>
  适用于项目介绍、技术博客、开源发布、架构说明、产品级技术叙事等场景。
</p>

<p align="center">
  <img src="https://img.shields.io/badge/style-high--taste-black?style=flat-square" alt="style"/>
  <img src="https://img.shields.io/badge/focus-authorial%20voice-blue?style=flat-square" alt="voice"/>
  <img src="https://img.shields.io/badge/priority-taste%20first-purple?style=flat-square" alt="priority"/>
  <img src="https://img.shields.io/badge/license-MIT-green?style=flat-square" alt="license"/>
</p>

---

## 项目简介

**High-Taste Technical Writing Engine** 是一套平台无关的技术写作 Skill 规范，用于帮助 AI 系统生成具备明确作者感、工程判断、表达节制与结构完整性的技术内容。

它的目标不是产出常见的“AI 宣传文”或“模板式说明文”，而是让 AI 更接近一个真正做过项目、想清楚问题、对表达有标准的技术作者。

这个仓库将该 Skill 以标准开源项目的形式整理出来，便于在主流 AI 平台、Prompt 框架、自动化工作流和团队内部写作系统中复用。

---

## 为什么要做这个项目

大量 AI 生成的技术内容都存在相似的问题：

- 看起来正确，但不像有人真正写过
- 语言流畅，但信息空心
- 罗列功能，却讲不清价值
- 想增强说服力，反而损失可信度
- 像模板拼出来的，而不是作者写出来的

这个项目就是为了解决这些问题。

它不是为了让写作更热闹，而是为了让写作更好：

- 更准确
- 更可信
- 更有辨识度
- 更适合真实技术场景
- 更接近高质量作者表达

---

## 核心理念

这个 Skill 的最高优先级是：**品味**。

这里所说的品味，不是装饰性的“文风”，而是：

- 有判断
- 有分寸
- 不廉价用力
- 对语气敏感
- 尊重工程现实
- 让内容像“被写出来”，而不是“被拼出来”

这高于增长技巧，高于 SEO 小聪明，也高于空洞的热情表达。

这并不意味着检索、转化、结构和清晰度不重要。它们都重要。但它们必须服务于写作，而不是破坏写作。

---

## 这个 Skill 适合什么场景

当你希望 AI 生成以下内容时，可以使用这个 Skill：

- 技术博客
- 开源项目介绍
- GitHub 项目说明
- 发布公告
- 架构设计文章
- 工程复盘
- 产品或平台技术说明
- 实现细节解析
- 面向技术读者的长文内容

它尤其适合那些需要同时平衡以下目标的场景：

- 专业性与可读性
- 技术深度与传播效率
- 检索友好与表达质感
- 转化目标与克制感

---

## 这个 Skill 的不同之处

### 1. 把品味放在第一位
这个 Skill 把品味和作者感视为核心约束，而不是可有可无的附加项。

### 2. 明确压制通用 AI 腔
它会主动压制模板化表达、夸张赞美、空泛总结和合成式热情。

### 3. 强调工程判断，而不是功能堆砌
它不满足于列 feature，而会解释设计为什么重要、解决了什么问题、取舍在哪里。

### 4. 平台无关，可迁移
它可以用于 ChatGPT、Claude、Gemini、DeepSeek、Prompt 编排工具、内部 Copilot 或自定义 LLM 工作流。

### 5. 兼顾检索与尊严
它允许做 SEO、搜索优化和转化设计，但前提是自然、克制、不把内容写成广告。

---

## 设计目标

这个 Skill 想要产出的内容应该具备以下特征：

- 像作者写的，不像系统拼的
- 有说服力，但不油腻
- 清晰，但不寡淡
- 有结构，但不机械
- 有观点，但不表演化
- 易被检索，但不堆词
- 真正有用，而不是装饰性文本

---

## 仓库结构

```text
high-taste-technical-writing-engine/
├── README.md
├── README_CN.md
├── SKILL.md              ← 单文件 Skill，可直接导入
├── LICENSE
├── skill/
│   ├── skill.md
│   ├── skill.cn.md
│   ├── quickstart.md
│   └── quickstart.cn.md
├── docs/
│   ├── writing-principles.md
│   ├── platform-adaptation.md
│   ├── anti-patterns.md
│   └── examples.md
└── examples/
    ├── input-template.md
    ├── output-outline.md
    └── prompt-template.md
```

---

## 快速开始

### 方式零：直接导入单文件 SKILL.md（Claude Code / 命令式 Skill 导入）

仓库根目录的 `SKILL.md` 是完整 Skill 的自包含、可直接导入版本。在支持从目录加载 Skill 的 agent（如 Claude Code）中使用：

```bash
mkdir -p ~/.claude/skills/high-taste-technical-writing
cp SKILL.md ~/.claude/skills/high-taste-technical-writing/SKILL.md
```

重启会话后，该 Skill 会被自动发现，并在你编写技术内容时自动应用。它自带 frontmatter（`name` 和基于触发条件的 `description`），agent 知道何时加载它。

### 方式一：将完整 Skill 作为系统提示或开发者提示使用

将 `skill/skill.md` 中的内容作为高优先级指令块加载到你的 AI 平台中。

然后再提供：

1. 原始资料
2. 目标平台
3. 目标读者
4. 目标动作或结果
5. 期望输出格式

### 方式二：使用简化 Prompt 模板

如果你需要轻量化、可重复调用的版本，可以直接使用 `examples/prompt-template.md`。

### 方式三：按平台适配

查看 `docs/platform-adaptation.md`，将该 Skill 映射到：

- system prompt
- developer prompt
- 可复用 prompt library
- 自定义 assistant instructions
- 编排工具中的工作流节点

---

## 推荐使用流程

1. 先定义写作任务
2. 明确目标读者和目标结果
3. 提供真实资料，而不是空泛摘要
4. 加载 Skill 指令
5. 请求完整初稿
6. 按质量清单检查结果
7. 如有需要，再微调语气、重点和转化点

这个 Skill 在“资料真实且具体”的前提下效果最好。它不是用来伪造深度的。

---

## 质量标准

一个符合本 Skill 要求的输出，应该满足：

- 像真实技术作者写的
- 没有明显 AI 腔
- 先讲问题，再讲方案
- 会解释设计判断，而不是只讲结果
- 用词准确，不靠空泛形容词撑场面
- 即使在宣传场景下也保持可信度
- 能自然引导读者进入下一步动作

如果结果读起来像宣传册，那基本说明 Skill 没有被正确执行。

---

## 写作原则

本项目最重要的写作原则包括：

### 从真实问题切入
不要先夸，先讲现实。

### 解释价值，而不是只列功能
功能清单不是论证。

### 多写机制，少写形容词
说明它做了什么、为什么重要、适合什么场景。

### 带着判断写
可以有观点，但观点必须来自经验和分析。

### 保持克制
即使是宣传型内容，也要让人信服。

### 保留作者存在感
读者应该感觉到“这是有人认真写的”。

---

## 这个 Skill 主要防止哪些问题

- “在当今时代……”式空泛开头
- 没有依据的夸张赞美
- 反复出现“强大 / 完善 / 全面 / 灵活”之类空词
- 只有清单、没有判断的描述
- 强行兴奋的语气
- 生硬堆 SEO 关键词
- 硬广式行动引导
- 为了“客观”而抹掉作者判断

---

## 文档说明

### Skill 文件
- `SKILL.md`：单文件、可直接导入的 Skill（Claude Code / 命令式 Skill 导入）
- `skill/skill.md`：英文完整版 Skill 规范
- `skill/skill.cn.md`：中文完整版 Skill 规范
- `skill/quickstart.md`：英文快速使用说明
- `skill/quickstart.cn.md`：中文快速使用说明

### 支撑文档
- `docs/writing-principles.md`：写作原则与标准
- `docs/platform-adaptation.md`：多平台适配说明
- `docs/anti-patterns.md`：常见失败模式与禁忌
- `docs/examples.md`：示例用法

### 模板文件
- `examples/input-template.md`：输入资料模板
- `examples/output-outline.md`：默认输出结构
- `examples/prompt-template.md`：可复用短 Prompt 模板

---

## 典型使用场景

- 把 GitHub README 改写成没有 AI 痕迹的 CSDN 技术文章
- 把技术项目整理成更易检索、但仍然可信的发布帖
- 把架构笔记整理成可读性更强的工程文章
- 把内部技术总结改写成面向外部的公开博客，同时保留严谨性
- 把产品说明改写成真正有判断、有结构的技术解读

---

## 适合哪些人使用

这个项目适合：

- 持续输出技术内容的工程师
- 开源项目维护者
- 不喜欢营销腔的开发者布道者
- 技术型创业者
- 架构师、资深工程师
- 构建 AI 写作工作流的人
- 搭建内部写作 Copilot 的团队

---

## 使用提醒

这个 Skill 是故意“严格”的。

它生成的内容，通常会比常见 AI 营销文更克制、更稳、更像真实作者写的。这不是缺点，而是设计目标。

如果某个平台倾向于过度赞美、过度总结、过度圆滑，那么应尽可能把本 Skill 放在更高优先级的位置。

---

## 贡献说明

欢迎贡献，尤其是以下方向：

- 更多平台适配指南
- 更多写作场景示例
- 失败模式样例库
- 不同 AI 平台效果对比
- 在不降低标准前提下，进一步打磨 Skill 语言

请保持高标准。这个仓库不是用来堆砌通用 Prompt 的。

---

## License

本项目基于 MIT License 开源。

---

## 语言切换

- English: `README.md`
- 中文：`README_CN.md`

---

