---
name: market-insight-skill
description: >
  A structured market intelligence skill based on the "Five Views" consulting methodology.
  Use this skill whenever a user wants to analyze a market, industry, product, or company —
  including requests like "help me understand this market", "do a competitive analysis",
  "analyze this industry", "I need a market report", "help me research [company/product/industry]",
  "do a five-forces analysis", or "I need insights before launching a product".
  Also triggers for: due diligence research, go-to-market planning, investor decks, 
  strategic planning sessions, and any request that involves understanding customers, 
  competitors, or market trends. When in doubt, use this skill — it dramatically improves 
  output quality for any market-related question.
---

# 市场洞察五看方法论 · Market Insight Five Views

A consulting-grade market analysis framework. Given minimal input from the user, 
you will use web search to gather data, apply structured analytical tools, and 
produce a complete market insight report with actionable conclusions.

---

## HOW TO USE THIS SKILL

### Step 1 — Collect User Input

Ask the user for the following (all in one message, keep it simple):

```
To get started, I need a few basics:

1. **What are you analyzing?** (company name / product / industry / market)
2. **Your role / purpose** (e.g., launching a product, doing due diligence, strategy planning)
3. **Geography** (China / Global / specific region)
4. **Any known context?** (optional: key competitors, rough market size, special concerns)
```

If the user has already provided enough context, skip directly to Step 2.

### Step 2 — Web Research Phase

Before writing any analysis, conduct web searches to gather real data. Use the following search strategy:

**For each of the Five Views, search for:**

| View | Search Queries to Run |
|------|----------------------|
| 看宏观 | `[industry] macro trends [year]`, `[industry] policy regulation`, `[industry] technology trends`, `[industry] consumer behavior trends` |
| 看行业 | `[industry] market size [year]`, `[industry] growth rate forecast`, `[industry] supply chain`, `[industry] market share`, `[industry] industry lifecycle` |
| 看客户 | `[industry] target customer profile`, `[industry] consumer insight report`, `[industry] user needs pain points`, `[product] customer segment` |
| 看竞争 | `[industry] top competitors`, `[competitor] product strategy`, `[competitor] market share`, `[industry] competitive landscape [year]` |
| 看自己 | `[company] revenue performance`, `[company] SWOT`, `[company] vs competitors`, `[company] product positioning` |

Run **at least 8–12 searches** before writing the report. Synthesize findings across sources.

### Step 3 — Generate the Report

Follow the full report structure in `references/report_structure.md`.
Apply analytical tools from `references/analytical_tools.md` where relevant.
Output in Markdown format.

### Step 4 — Conclusions & Recommendations

**This is mandatory.** Every report must end with:
- A "So What" summary (3–5 bullet strategic takeaways)
- Specific, prioritized action recommendations
- Key risks and uncertainties to monitor

---

## REPORT STRUCTURE OVERVIEW

```
# [Company/Industry] 市场洞察报告

## 执行摘要 Executive Summary

## 一、看宏观 Macro Environment
  - Certainty/Uncertainty Matrix
  - Key macro forces: policy, economy, social, technology

## 二、看行业 Industry Analysis  
  - Industry lifecycle stage
  - Value chain analysis
  - Segment size & growth
  - Industry concentration

## 三、看客户 Customer Insights
  - Customer segmentation
  - User personas
  - Key value factors (KANO model)
  - Unmet needs

## 四、看竞争 Competitive Landscape
  - Competitor strategy (macro)
  - Product benchmarking (micro)
  - Competitive positioning map

## 五、看自己 Self Assessment
  - KPI review vs. targets
  - Gap analysis & root causes
  - Key success factors benchmark

## 战略结论与建议 Strategic Conclusions & Recommendations
  - Core findings
  - Prioritized recommendations
  - Risk watch list
```

For detailed instructions on each section → read `references/report_structure.md`
For analytical tools and how to apply them → read `references/analytical_tools.md`

---

## OUTPUT RULES

1. **Always search before writing** — never fabricate data, always cite sources
2. **Always conclude** — every section ends with "对本企业的启示" (implications)
3. **Use tables and matrices** — structured data is clearer than prose
4. **Be specific** — name actual companies, give actual numbers with sources
5. **Flag uncertainty** — clearly mark estimates vs. confirmed data
6. **Language** — match the user's language (Chinese or English); section headers can be bilingual
7. **Length** — aim for comprehensive but scannable; use headers, bullets, and tables

---

## COMPATIBILITY

Works with:
- **Claude Code**: `claude -p "analyze [X] using the five views framework"`
- **Gemini CLI**: Load SKILL.md as system context, then provide user query
- **GPT (via API)**: Use SKILL.md as system prompt, follow the same workflow
- **Claude.ai / ChatGPT UI**: Paste SKILL.md content as initial context

Web search capability required for best results. If web search is unavailable, 
note this clearly and proceed with model knowledge, flagging the knowledge cutoff.
