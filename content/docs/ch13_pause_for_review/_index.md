---
title: "Chapter 13: A Pause for Review: Comparing Cohort and Case-Control Studies"
titleTC: "回顧與比較：隊列研究與病例對照研究"
description: "Gordis Epidemiology Chapter 13 - A Pause for Review: Comparing Cohort and Case-Control Studies"
draft: false
---

# Chapter 13: A Pause for Review: Comparing Cohort and Case-Control Studies
## 回顧與比較：隊列研究與病例對照研究

## Learning Objectives | 學習目標

By the end of this chapter, you should be able to:

- Describe the **sequence of study designs** used in studying disease etiology
- Differentiate **cohort studies** from **case-control studies**
- Explain when each study design is appropriate
- Identify key **advantages and limitations** of each design

---

## Introduction | 導論

經過前幾章的學習，我們已經接觸了多種流行病學研究設計。現在讓我們暫停一下，回顧並比較最重要的兩種觀察性研究設計：**隊列研究 (Cohort Studies)** 和 **病例對照研究 (Case-Control Studies)**。

> **臨床重點**
> 選擇正確的研究設計是回答特定研究問題的關鍵。隊列研究和病例對照研究各有其適用情境，臨床醫師理解這些差異有助於批判性評讀醫學文獻。

---

## Study Design Comparison | 研究設計比較

### Fundamental Difference | 根本差異

| Feature | **Cohort Study** | **Case-Control Study** |
|---|---|---|
| **Starting Point** | Exposure status | Disease status |
| **Groups Compared** | Exposed vs. Not Exposed | Cases (disease) vs. Controls (no disease) |
| **Direction** | Forward in time | Backward in time |
| **Measures** | Incidence, Relative Risk | Odds Ratio |
| **Can Calculate Incidence?** | Yes (directly) | No (requires additional assumptions) |

### Visual Comparison | 視覺化比較

**Figure 13-1: Cohort Study Design**

```
START: Identify EXPOSED and NOT EXPOSED groups
  ↓
FOLLOW OVER TIME
  ↓
COMPARE INCIDENCE of disease in each group
  ↓
Measure: RR, AR, OR (if rare disease)
```

**Figure 13-2: Case-Control Study Design**

```
START: Identify CASES (disease) and CONTROLS (no disease)
  ↓
LOOK BACK: Determine exposure history
  ↓
COMPARE odds of exposure in cases vs. controls
  ↓
Measure: Odds Ratio (OR)
```

---

## Cohort Studies | 隊列研究

### Characteristics | 特性

**Advantages of Cohort Studies:**

| Advantage | Explanation |
|---|---|
| Direct incidence calculation | Can measure actual disease occurrence |
| Multiple outcomes | Can study one exposure → many diseases |
| Temporal relationship clear | Exposure precedes disease |
| Relative risk calculable | Direct comparison of incidence rates |
| Minimizes recall bias | Exposure data collected before disease |

**Limitations of Cohort Studies:**

| Limitation | Explanation |
|---|---|
| Expensive | Requires large populations and long follow-up |
| Inefficient for rare diseases | Must follow many people to get enough cases |
| Loss to follow-up | Can introduce bias over time |
| Not suitable for rare exposures | Need large exposed group |

### Types of Cohort Studies | 隊列研究類型

| Type | Timing of Data | Characteristics |
|---|---|---|
| **Prospective** | Forward from start | Exposure data collected as study begins |
| **Retrospective (Historical)** | Backward | Uses past records; exposure already occurred |
| **Nested Case-Control** | Mixed | Cases identified within cohort; matched controls selected |

---

## Case-Control Studies | 病例對照研究

### Characteristics | 特性

**Advantages of Case-Control Studies:**

| Advantage | Explanation |
|---|---|
| Efficient for rare diseases | Start with existing cases |
| Faster and cheaper | Fewer subjects needed |
| Multiple exposures | Can study one disease → many exposures |
| Suitable for rare outcomes | Can recruit available cases |

**Limitations of Case-Control Studies:**

| Limitation | Explanation |
|---|---|
| Cannot calculate incidence directly | No true denominator |
| Recall bias risk | Exposure data collected after disease |
| Control selection difficult | Must represent source population |
| Cannot study multiple outcomes | Only one disease at a time |

### Key Challenge: Control Selection | 關鍵挑戰：對照組選擇

> **臨床重點**
> 病例對照研究中對照組的選擇是研究成敗的關鍵。理想的對照組應代表病例的來源族群，否則會產生 selection bias。

---

## Comparing Study Designs | 研究設計比較

### When to Use Each | 適用情境

| Scenario | Best Design |
|---|---|
| Exposure is rare | **Cohort study** |
| Disease is rare | **Case-control study** |
| Want to study multiple outcomes | **Cohort study** |
| Want to study multiple exposures | **Case-control study** |
| Need to establish temporal sequence | **Cohort study** |
| Limited resources and time | **Case-control study** |

### Decision Framework | 決策框架

```
Question: Is exposure → disease?
         ↓
Is exposure common? → YES → Cohort Study
         ↓ NO
Is disease rare? → YES → Case-Control Study
         ↓ NO
Consider feasibility, resources, time
```

---

## Sequential Study Approach | 研究順序

流行病學研究疾病病因時，常遵循以下順序：

**Figure 13-3: Typical Sequence**

```
1. Clinical Observations (床邊觀察)
   ↓
2. Analysis of Available Data (現有數據分析)
   ↓
3. Case-Control Study (病例對照研究) ← 通常作為第一步
   ↓
4. Cohort Study (隊列研究) ← 若病例對照有陽性發現
   ↓
5. Randomized Trial (隨機試驗) ← 僅針對治療干預
```

> **Historical Example:**
> 外科醫師 Alton Ochsner 观察到几乎所有他手术的肺癌患者都有吸烟史，由此提出吸烟可能与肺癌存在因果关系的假设。

---

## Hybrid Designs | 混合設計

### Nested Case-Control Study | 巢式病例對照研究

在大型隊列研究的框架內，於疾病發生後從同隊列中選取病例與對照：

| Advantage | Explanation |
|---|---|
| Eliminates recall bias | Exposure data collected before disease |
| Pre-illness state | Data from pre-diagnosis specimens |
| Cost-effective | Lab tests only on cases and matched controls |

### Cross-Sectional Studies | 橫斷面研究

測量特定時間點的暴露與疾病狀態，提供**患病率 (Prevalence)** 而非發生率。

---

## Summary | 摘要

本章回顧了兩種主要的觀察性研究設計：

1. **隊列研究 (Cohort Study)**
   - 從暴露分組，追蹤疾病發生
   - 可直接計算 RR 和 AR
   - 適合暴露常見、疾病相對常見

2. **病例對照研究 (Case-Control Study)**
   - 從疾病分組，回溯暴露歷史
   - 計算 OR（可近似 RR）
   - 適合疾病罕見、暴露相對常見

> 選擇何種設計取決於：暴露的稀有性、疾病的稀有性、所需資源與時間。

---

## Review Questions | 複習問題

1. What is the fundamental difference between a cohort study and a case-control study?

2. When would you choose a case-control study over a cohort study?

3. Why is control selection particularly challenging in case-control studies?

4. What is a nested case-control study and what are its advantages?
