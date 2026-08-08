---
title: "Chapter 14: From Association to Causation: Deriving Inferences from Epidemiologic Studies"
titleTC: "從關聯到因果：流行病學研究的推論"
description: "Gordis Epidemiology Chapter 14 - From Association to Causation: Deriving Inferences from Epidemiologic Studies"
draft: false
---

# Chapter 14: From Association to Causation: Deriving Inferences from Epidemiologic Studies
## 從關聯到因果：流行病學研究的推論

## Learning Objectives | 學習目標

By the end of this chapter, you should be able to:

- Explain the difference between **real** and **spurious** associations
- Define **necessary** and **sufficient** causes
- Apply the **Surgeon General's guidelines** for judging causal relationships
- Evaluate whether an observed association is likely to be causal

---

## Introduction | 導論

在前面的章節中，我們學會了如何測量暴露與疾病之間的**關聯性**。但關聯存在並不代表因果關係存在。

> 流行病學的核心問題：「我們觀察到的關聯是因果關係嗎？」

**Figure 14-1: The Two Key Questions**

```
Question 1: Is there an association? → Chapters 11-13
Question 2: Is the association causal? → This Chapter
```

> **臨床重點**
> 區分因果關聯與非因果關聯至關重要。如果膽固醇與冠心病的關聯是因果的，那降低膽固醇就能預防冠心病；但如果只是混雜（confounding）造成的虛假關聯，降低膽固醇就不會有任何效果。

---

## Types of Associations | 關聯的類型

### Real vs. Spurious Associations | 真實關聯與虛假關聯

When we observe an association, the first question is: **Is it real or spurious?**

**Spurious associations** can arise from:
- **Selection bias (選擇偏差)**: Errors in selecting study subjects
- **Information bias (資訊偏差)**: Errors in measuring exposure or disease
- **Confounding (混雜)**: Third factor associated with both exposure and disease

### The Coffee and Pancreatic Cancer Example | 咖啡與胰臟癌的例子

早期研究發現咖啡攝取與胰臟癌之間存在關聯。但後續分析揭示：

> 吸菸是**混雜因子 (Confounder)**：
> - 吸菸是胰臟癌的已知風險因子
> - 喝咖啡的人也更可能吸菸
> - 因此，咖啡與胰臟癌的關聯可能是混雜造成的虛假關聯

**Figure 14-2: Confounding Diagram**

```
Panel A: True Causal Association
Exposure → Disease

Panel B: Due to Confounding
Exposure ← Confounder (X) → Disease
```

---

## Types of Causal Relationships | 因果關係的類型

### Necessary and Sufficient Causes | 必要原因與充分原因

疾病發生的原因可以分為四種模型：

| Model | Definition | Example |
|---|---|---|
| **Necessary & Sufficient** | Must be present AND always causes disease | Prion disease (very rare) |
| **Necessary, not Sufficient** | Must be present BUT not always cause disease alone | *M. tuberculosis* for TB |
| **Sufficient, not Necessary** | Can cause disease BUT other factors can too | Radiation for leukemia |
| **Neither** | May or may not cause; not required | Most chronic diseases |

### Multistage Process | 多階段過程

癌變 (Carcinogenesis) 被認為是多階段過程：

```
Initiation (起始) → Promotion (促進) → Progression (進展)
```

兩個階段都需要才能發生癌症，說明了**必要但不充分**的因果關係。

---

## Approaches to Studying Disease Etiology | 研究疾病病因的方法

### Hierarchy of Evidence | 證據層級

| Level | Study Type | Evidence Strength |
|---|---|---|
| **Highest** | Randomized Controlled Trial | Best for causality |
| ↓ | Cohort Study | Good temporal relationship |
| ↓ | Case-Control Study | Retrospective |
| ↓ | Ecologic Study | Weakest individual-level evidence |

### Sequence of Studies | 研究順序

研究疾病病因時，通常遵循以下順序：

```
Clinical Observations
       ↓
Available Data Analysis
       ↓
Case-Control Study ← First new study often
       ↓
Cohort Study ← If case-control is positive
       ↓
Randomized Trial ← Only for interventions
```

---

## Guidelines for Judging Causality | 因果判斷指南

美國衛生局局長 (Surgeon General) 制定了判斷因果關係的準則，現已被廣泛採用：

### Table 14-1: Guidelines for Causal Inference

| # | Guideline | Description |
|---|---|---|
| 1 | **Temporal Relationship** | Exposure must precede disease |
| 2 | **Strength of Association** | Stronger associations more likely causal |
| 3 | **Dose-Response** | More exposure → More disease |
| 4 | **Replication** | Findings confirmed in other studies |
| 5 | **Biologic Plausibility** | Consistent with biological knowledge |
| 6 | **Alternate Explanations** | Considered and ruled out |
| 7 | **Cessation Exposure** | Risk drops when exposure stops |
| 8 | **Consistency with Knowledge** | Consistent with other evidence |
| 9 | **Specificity** | One exposure → specific disease |

---

## Applying the Guidelines | 應用這些指南

### 1. Temporal Relationship | 時間關係

> **This is the most critical criterion.** Exposure must occur BEFORE disease.

**Example:** Figure 14-3 shows London's 1952 air pollution episode:
- Particle concentration rose
- Mortality rose (respiratory & cardiovascular deaths)
- Concentration dropped → Mortality dropped

This temporal pattern strongly supported air pollution as a causal factor.

### 2. Strength of Association | 關聯強度

Measured by **relative risk (RR)** or **odds ratio (OR)**:
- Stronger association (higher RR) → More likely causal
- BUT weak association can still be causal

**Example:** 吸菸與肺癌的 RR ≈ 14
→ 這麼強的關聯很難用混雜解釋

### 3. Dose-Response Relationship | 劑量-反應關係

**Figure 14-4: Dose-Response Example (Smoking & Lung Cancer)**

| Cigarettes/Day | Death Rate (per 100,000) |
|---|---|
| Nonsmokers | ~10 |
| 1-9/day | ~50 |
| 10-19/day | ~90 |
| 20-39/day | ~140 |
| 40+/day | ~300 |

> Dose-response relationship is **strong evidence** for causality.

### 4. Replication of Findings | 研究結果的可重複性

- Results should be replicated in different populations
- By different investigators
- Using different methods

### 5. Biologic Plausibility | 生物學合理性

- Is the association consistent with current scientific knowledge?
- Is there a known mechanism?

### 6. Consideration of Alternate Explanations | 考慮替代解釋

- Could the association be due to **confounding**?
- Could **selection bias** explain the findings?
- Could **information bias** produce the result?

### 7. Cessation of Exposure | 暴露終止

- If exposure is eliminated, disease risk should decrease
- **Example:** Smoking cessation → Lung cancer rates decline over time

### 8. Consistency with Other Knowledge | 與其他知識的一致性

- Consistent with animal studies
- Consistent with clinical observations
- Consistent with other epidemiologic studies

### 9. Specificity of the Association | 關聯的特異性

- One exposure leads to one specific disease
- Less weighted in modern epidemiology
- Many exposures cause multiple diseases

---

## The Susceptible Individual | 易感個體

Not everyone exposed to a causal factor will develop disease:

> 疾病不等同於命運。基因與環境的交互作用決定了誰會發病。

**Example:** 
- 並非所有吸菸者都會得肺癌
- 並非所有肺癌患者都吸菸
- 差異反映了基因易感性與其他環境 cofactors

---

## Case Study: Smoking and Low Birth Weight | 案例：吸菸與低出生體重

### The Controversy | 爭議

多年來，學者對「吸菸導致低出生體重」存在爭議：

- **Jacob Yerushalmy** 認為可能是混雜：吸菸者與非吸菸者在許多特徵上不同
- 其他人則主張因果關係

### Resolution | 解決

最終證據支持因果關係：
- 劑量-反應關係明確
- 隨機試驗顯示戒菸計畫可降低低出生體重發生率

> 這個案例說明了即使面對爭議，仔細應用因果推論指南可以幫助得出正確結論。

---

## Summary | 摘要

判斷因果關係需要系統性評估：

1. **真實關聯 vs. 虛假關聯** — 首先確認關聯不是偏差造成
2. **時間關係** — 最關鍵：暴露必須在疾病之前
3. **九項指南** — 強度、劑量-反應、可重複性、合理性等
4. **混雜考慮** — 必須排除替代解釋
5. **必要vs充分** — 多數慢性病是 neither necessary nor sufficient

這些原則為第15章的偏差與混雜詳細討論奠定基礎。

---

## Review Questions | 複習問題

1. What is the difference between a spurious association and a real causal association?

2. List the three criteria for a factor to be a confounder.

3. Why is temporal relationship considered the most important criterion for causality?

4. What does a dose-response relationship tell us about a potential causal association?

5. In the smoking and lung cancer example, which of the Surgeon General's guidelines are satisfied?
