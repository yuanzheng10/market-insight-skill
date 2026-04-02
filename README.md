# market-insight-skill

> 一套咨询级市场分析框架，让 AI 帮你系统地洞察市场  
> A consulting-grade market intelligence skill. Give AI your topic — it searches the web, applies structured frameworks, and delivers a complete strategic report.

---

## 什么是五看方法论？ What Is This?

"五看"是顶级咨询公司广泛使用的市场洞察框架，覆盖：

| # | 模块 | 核心问题 |
|---|------|---------|
| 1 | **看宏观** | 外部大环境有哪些确定与不确定的力量？ |
| 2 | **看行业** | 行业在哪个阶段？价值在哪里？机会在哪里？ |
| 3 | **看客户** | 谁是我的用户？他们真正要什么？ |
| 4 | **看竞争** | 竞争对手怎么打？我在哪里能赢？ |
| 5 | **看自己** | 我现在表现如何？差距在哪里？ |

This skill turns that framework into an **AI-powered, web-researched, recommendation-driven** market report. Give the AI your topic and a few context details — it does the rest.

---

## 快速上手 Quick Start

### Option A — Claude Code

```bash
# Install Claude Code if not already installed
npm install -g @anthropic-ai/claude-code

# Clone this skill
git clone https://github.com/YOUR_USERNAME/market-insight-five-views.git

# Run analysis
cd market-insight-five-views
claude "请用五看方法论分析中国新能源汽车市场，我是一家想进入这个行业的投资机构"
```

### Option B — Gemini CLI

```bash
# Install Gemini CLI
pip install gemini-cli  # or follow official install

# Run with skill as context
gemini --system-file SKILL.md "Analyze the China EV market using the five views framework. I'm an investor doing due diligence."
```

### Option C — OpenAI / GPT (API or Custom GPT)

```python
import openai

with open("SKILL.md", "r") as f:
    skill_content = f.read()

response = openai.chat.completions.create(
    model="gpt-4o",
    messages=[
        {"role": "system", "content": skill_content},
        {"role": "user", "content": "请用五看方法论分析中国咖啡连锁市场，我们是准备进入的新品牌"}
    ]
)
print(response.choices[0].message.content)
```

### Option D — Claude.ai / ChatGPT Web UI

1. Open a new conversation
2. Copy the contents of `SKILL.md`
3. Paste as your first message, then add your analysis request
4. The AI will guide you through providing inputs and deliver the full report

---

## 你只需要告诉 AI 这几件事 What You Need to Provide

```
1. 分析对象：公司名 / 产品 / 行业 / 市场
2. 你的角色：投资人 / 产品负责人 / 咨询顾问 / 创业者 / 战略分析师
3. 地域范围：中国 / 全球 / 特定地区
4. （可选）已知背景：主要竞品、大概市场规模、特别关注的问题
```

AI 会自动：
- 🔍 联网搜索行业数据、竞品信息、市场报告
- 📊 套用五看框架进行结构化分析
- 💡 给出有依据的战略结论和具体建议
- ⚠️ 标注不确定信息和需要验证的数据

---

## 输出示例 Sample Output Structure

```markdown
# 中国咖啡连锁市场 — 五看市场洞察报告

## 执行摘要
[核心结论 + 五维度关键发现表格]

## 一、看宏观
[确定性/不确定性矩阵 + 政策/经济/社会/技术分析]

## 二、看行业
[生命周期判断 + 产业链图谱 + 细分市场规模 + 行业集中度]

## 三、看客户
[用户细分 + 画像 + KANO模型需求分类]

## 四、看竞争
[瑞幸/星巴克/Manner等宏观战略 + 4P竞品对比 + 定位图]

## 五、看自己
[KPI复盘框架 + 差距根因分析 + 关键成功因素对标]

## 战略结论与建议
[即刻行动 / 中期布局 / 长期投入 + 优先级矩阵 + 风险预警]
```

---

## 文件结构 File Structure

```
market-insight-five-views/
├── SKILL.md                          # 核心技能文件 (AI reads this)
├── README.md                         # 本文件
├── references/
│   ├── report_structure.md           # 报告各章节详细写法指引
│   └── analytical_tools.md           # 10个分析工具详解
├── templates/
│   └── report_template.md            # 空白报告模板（可直接填写）
└── examples/
    └── coffee_chain_china.md         # 示例报告：中国咖啡连锁市场
```

---

## 支持的分析场景 Use Cases

| 场景 | 示例 prompt |
|------|------------|
| 新市场进入分析 | "我们是一家中国台湾饮料品牌，评估进入中国大陆市场的机会" |
| 投资尽调 | "请帮我做一个中国宠物食品赛道的市场洞察，用于投资决策" |
| 竞品分析 | "分析我们在教育SaaS领域的竞争格局，主要竞品是猿辅导和作业帮" |
| 产品战略规划 | "我是一个智能音箱产品负责人，帮我用五看框架梳理产品方向" |
| 战略规划输入 | "我们公司做健康食品，帮我准备年度战略会的市场分析材料" |
| 行业研究报告 | "写一份新能源两轮车行业的五看分析报告" |

---

## 内嵌分析工具 Embedded Analytical Tools

| 工具 | 应用场景 |
|------|---------|
| 确定性/不确定性矩阵 | 宏观力量分类与战略应对 |
| 行业生命周期模型 | 判断行业阶段，制定竞争姿态 |
| 产业链价值转移分析 | 找到高价值环节，规划布局方向 |
| MECE法则 | 客户细分设计，确保不重叠不遗漏 |
| KANO需求模型 | 产品功能优先级排序 |
| 4P竞品对比框架 | 系统化竞争对手分析 |
| 有效细分验证六标准 | 评估细分市场可行性 |
| 根因分析六维度 | 诊断业绩差距的真正原因 |
| 优先级矩阵 | 战略建议排序 |
| 风险评估矩阵 | 识别和管理战略风险 |

---

## 数据说明 Data & Accuracy Note

- AI 会联网搜索实时数据，但**关键数字请在战略决策前自行核实**
- 搜索能力取决于你使用的 AI 平台（Claude / Gemini / GPT）的联网设置
- 若无法联网，AI 会基于训练数据分析，并注明知识截止日期
- 建议将 AI 报告作为**分析框架和假设起点**，结合一手数据使用

---

## 贡献 Contributing

欢迎提交 PR 改进框架、补充行业示例、或适配更多 AI 平台。

---

## License

MIT License — 可自由使用、修改、商用，请保留出处。
