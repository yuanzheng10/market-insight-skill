# Analytical Tools Reference

Quick reference guide for all analytical tools embedded in the Five Views framework.
Apply these tools during the relevant sections of analysis.

---

## Tool 1: Certainty-Uncertainty Matrix (看宏观)

**Purpose**: Distinguish macro factors that are predictable from those that could disrupt the industry.

**How to apply**:
1. List 15–25 macro forces across three categories: 消费者行为, 宏观环境, 技术趋势
2. Score each factor on two axes (1–3 scale):
   - X-axis: Impact on industry structure (1=low, 3=high)
   - Y-axis: Uncertainty of outcome (1=low, 3=high)
3. Plot on matrix → quadrant determines strategy

**Quadrant Interpretation**:

| Quadrant | Label | Strategy |
|----------|-------|----------|
| High Impact + Low Uncertainty | 相对确定的趋势 | Build core strategy around this |
| High Impact + High Uncertainty | 关键的不确定情况 (颠覆性) | Scenario plan; monitor closely |
| Low Impact + High Uncertainty | 不确定的情况 | Watch but don't over-invest |
| Low Impact + Low Uncertainty | 背景噪音 | Ignore for now |

**Common macro forces to consider**:
- 政策: regulations, subsidies, trade policy, data laws
- 经济: GDP growth, inflation, consumer spending power, labor costs
- 社会: demographics, urbanization, values shifts, health awareness
- 技术: AI/IoT adoption, platform maturity, infrastructure
- 竞争生态: supply chain disruption, industry boundary blurring, new entrants

---

## Tool 2: Industry Lifecycle Analysis (看行业)

**Purpose**: Determine which stage an industry (or segment) is in to inform the right competitive posture.

**Stage Indicators**:

| Signal | 导入期 | 成长期 | 成熟期 | 衰退期 |
|--------|--------|--------|--------|--------|
| Market growth rate | Volatile / Unknown | >20% YoY | 5–15% YoY | <5% or negative |
| Number of competitors | Few, growing | Rapidly increasing | Consolidating | Declining |
| Product standardization | Low (fragmented) | Increasing | High | Very high |
| Profit margins | Low to negative | High (early movers) | Compressing | Low |
| Consumer awareness | Low | Building fast | High | Declining |
| Technology change | Very fast | Fast | Moderate | Slow |

**Decision rules by stage**:
- **导入期** → Educate market, build infrastructure, accept losses for share
- **成长期** → Scale fast, grab distribution, invest in brand, ride the wave
- **成熟期** → Operational excellence, segmentation, loyalty programs, M&A
- **衰退期** → Harvest or pivot; find adjacent growth curves

**Differentiated lifecycle**: Note that different segments of the same market can be at different stages (e.g., 4G phones = maturity, 5G phones = growth). Always analyze at the segment level.

---

## Tool 3: Value Chain Analysis (看行业)

**Purpose**: Map where value is created, captured, and shifting across the industry.

**Analysis steps**:
1. Draw the full chain from raw materials → end user
2. For each node, assess:
   - **Gross margin**: High margin = power node
   - **Concentration**: Concentrated = high power, fragmented = competitive
   - **Barriers to entry**: Patent, capital, relationships, regulation
   - **Value trend**: Is this node gaining or losing value over time?

**Common value shift patterns to look for**:
- Hardware → Software/Services (e.g., smartphones, cars)
- Offline → Online (e.g., retail, media)
- Manufacturing → Brand/Experience (e.g., consumer goods)
- Product → Ecosystem/Platform (e.g., tech, payments)
- Generalist → Specialist (e.g., B2B SaaS)

**Strategic implication**: 
- If your node is losing value → migrate upstream/downstream or out
- If an adjacent node is gaining value → consider entering it
- If concentration is rising in your node → consolidate or differentiate

---

## Tool 4: MECE Principle (看客户 — Segmentation)

**Definition**: Mutually Exclusive, Collectively Exhaustive  
(麦肯锡分析法 — 子集相互独立，并集完全穷尽)

**How to apply to customer segmentation**:
1. Choose a segmentation variable
2. Define categories so they do NOT overlap (mutually exclusive)
3. Make sure ALL customers can fit into one category (collectively exhaustive)
4. Add "Other" category only as last resort

**Good example**:
```
Education level: 无学历 | 小学 | 初中 | 高中/中专 | 大专 | 本科 | 硕士 | 博士及以上
→ Mutually exclusive ✅ | Exhaustive ✅
```

**Bad example**:
```
Age: 20–30 | 30–40 | 40–50
→ Where does a 30-year-old go? → NOT mutually exclusive ❌
→ What about under 20 or over 50? → NOT exhaustive ❌
```

**Fix**: `<20 | 20–29 | 30–39 | 40–49 | 50+`

**Apply MECE to**: market segments, customer needs, competitive factors, root cause trees, recommendation lists

---

## Tool 5: KANO Model (看客户 — Feature Prioritization)

**Purpose**: Classify product features by their relationship to customer satisfaction, to prioritize where to invest.

**The five categories**:

| Category | Chinese | Logic | Investment Strategy |
|----------|---------|-------|---------------------|
| Must-be | 必备属性 | Expected; absence = major dissatisfaction | Minimum viable; don't fail here |
| Performance | 期望属性 | Linear relationship; more = more satisfied | Outperform competitors |
| Attractive | 魅力属性 | Unexpected delight; creates strong preference | Differentiation opportunity |
| Indifferent | 无差异属性 | No impact either way | Reduce or eliminate investment |
| Reverse | 反向属性 | Presence decreases satisfaction | Do NOT build this |

**How to determine categories**:
- Run KANO survey: ask functional question ("If this feature exists, how do you feel?") AND dysfunctional question ("If this feature doesn't exist, how do you feel?")
- Map responses to categories using the KANO evaluation table

**Key insight**: Categories shift over time. Today's attractive feature becomes tomorrow's must-be (e.g., smartphone cameras, free shipping).

**Practical shortcut** (when survey not available):
- Study reviews of your product and competitors → Complaints → Must-be gaps
- Study "what delights users" in reviews → Attractive candidates
- Study what users never mention → Likely indifferent

---

## Tool 6: Effective Segmentation Validation (看客户)

After proposing customer segments, validate against all six criteria:

| Criterion | Chinese | Question to ask |
|-----------|---------|-----------------|
| Differentiable | 差异性 | Do different segments actually respond differently to our offerings? |
| Substantial | 规模性 | Is each segment large enough to be worth targeting profitably? |
| Measurable | 可衡量性 | Can we identify who belongs to this segment and track them? |
| Stable | 相对稳定性 | Will this segment still exist in 2–3 years? |
| Accessible | 可进入性 | Can we actually reach and serve this segment? |
| Actionable | 关联性 | Does targeting this segment align with our strategy and capabilities? |

If a segment fails 2+ criteria → redefine or merge it.

---

## Tool 7: 4P Competitive Analysis (看竞争)

**Framework**: Analyze competitors across Product, Price, Place, Promotion

**How to apply**:

**Product**: 
- Feature set comparison (functional table: ✅/❌/partial)
- Quality level and positioning
- Product line breadth and tiering strategy
- Innovation pipeline (public patents, job postings, press)

**Price**:
- Absolute price points by segment
- Pricing model (per unit / subscription / freemium / bundle)
- Discount and promotional behavior
- Price positioning (premium / value / mass)

**Place (Distribution)**:
- Channel mix: direct vs. indirect, online vs. offline
- Key retail/platform partners
- Geographic coverage
- Channel economics (exclusivity, margins)

**Promotion**:
- Brand positioning statement
- Key messages and campaigns
- Media mix (TV, digital, KOL, events)
- Tone and target audience for communications

**Output**: Completed 4P comparison table + identification of where competitors are strong/weak

---

## Tool 8: Root Cause Analysis — 6-Dimension Framework (看自己)

**Purpose**: When a KPI gap is identified, diagnose the root cause accurately before recommending solutions.

**The six dimensions**:

| Dimension | Chinese | Key questions |
|-----------|---------|---------------|
| Strategy & Approach | 战略与策略 | Is our direction right? Are we targeting the right markets/customers? |
| Organization & Governance | 组织与管控 | Is our structure aligned with our goals? Is decision-making too slow? |
| Systems & Processes | 体系和流程 | Do our workflows support execution? Where are the bottlenecks? |
| Performance & Incentives | 绩效和激励 | Are people measured and rewarded for the right things? |
| People & Capabilities | 人员能力 | Do we have the skills we need? Where are capability gaps? |
| Technology & IT | IT和技术 | Does our technology enable or hinder performance? |

**How to use**:
1. State the gap clearly (e.g., "Market share declined 3% despite product improvements")
2. Systematically test each dimension with evidence
3. Identify 1–3 root causes (rarely more than 3 genuine root causes exist)
4. Match recommendations to root causes (not symptoms)

---

## Tool 9: Priority Matrix for Recommendations (战略建议)

**Purpose**: Help stakeholders decide where to invest limited resources.

**2×2 Matrix — Strategic Value × Execution Difficulty**:

| | Low Difficulty | High Difficulty |
|--|---------------|-----------------|
| **High Strategic Value** | ⭐ Quick Wins — Do immediately | 📋 Major Initiatives — Plan carefully |
| **Low Strategic Value** | 🔧 Fill-ins — Do when bandwidth allows | ❌ Avoid — Don't invest here |

**How to score each recommendation**:

Strategic Value (1–5):
- 5: Core to long-term competitive advantage
- 3: Meaningful improvement but not differentiating
- 1: Minor, marginal impact

Execution Difficulty (1–5):
- 1: Easy (resources exist, low coordination needed, quick results)
- 3: Moderate (some investment, cross-functional, 3–6 months)
- 5: Hard (major investment, organizational change, 12+ months)

---

## Tool 10: Risk Assessment Matrix (风险预警)

**Purpose**: Surface and prioritize strategic risks before they materialize.

**Risk Categories to check**:
- Market risks: demand shifts, price wars, commoditization
- Regulatory risks: new laws, compliance costs, licensing
- Technology risks: disruption, obsolescence, cybersecurity
- Competitive risks: new entrants, competitor moves, loss of key talent
- Supply chain risks: concentration, geopolitics, cost inflation
- Customer risks: churn, expectation shifts, platform dependency

**Risk Scoring**:

| Score | Likelihood | Impact |
|-------|------------|--------|
| High | Likely in 12 months | Business-threatening |
| Medium | Possible in 1–3 years | Significant but manageable |
| Low | Unlikely but plausible | Minor or containable |

**Output**: Risk register table with likelihood, impact, early warning signals, and contingency response

---

*These tools are embedded within the Five Views framework. Apply them in the relevant sections rather than in isolation — their power comes from connecting macro trends to customer needs to competitive responses.*
