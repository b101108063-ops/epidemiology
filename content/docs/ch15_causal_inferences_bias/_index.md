---
title: "Chapter 15: More on Causal Inferences: Bias, Confounding, and Interaction"
titleTC: "因果推論深入探討：偏差、混雜與交互作用"
description: "Gordis Epidemiology Chapter 15 - More on Causal Inferences: Bias, Confounding, and Interaction"
draft: false
---

# Chapter 15: More on Causal Inferences: Bias, Confounding, and Interaction
## 因果推論深入探討：偏差、混雜與交互作用

## Learning Objectives | 學習目標

By the end of this chapter, you should be able to:

- Define and identify **selection bias** and **information bias**
- Understand **confounding** and methods to address it
- Recognize **interaction (effect modification)** and its implications
- Apply strategies to minimize bias in study design and analysis

---

## Introduction | 導論

上一章節我們討論了判斷因果關係的九項指南。然而，要正確應用這些指南，我們必須首先確保研究本身沒有**系統性錯誤**。

> **偏差 (Bias)** 會系統性地扭曲研究結果，導致錯誤的因果推論。

本章深入探討三個關鍵主題：
1. **偏差 (Bias)** — 研究設計與執行中的系統性錯誤
2. **混雜 (Confounding)** — 第三因子造成的虛假關聯
3. **交互作用 (Interaction)** — 兩因子如何共同影響疾病風險

---

## Bias | 偏差

**Bias 定義：** 研究設計、執行或分析中的任何系統性錯誤，導致對暴露與疾病風險關係的錯誤估計。

### Table 15-1: Major Types of Bias

| Type | Definition | Impact |
|---|---|---|
| **Selection Bias** | Systematic error in selecting study subjects | Distorts exposure-disease relationship |
| **Information Bias** | Systematic error in measuring exposure/disease | Misclassification of subjects |
| **Confounding** (a form of bias) | Third factor distorts the true relationship | Can falsely suggest or mask causality |

---

## Selection Bias | 選擇偏差

### Definition | 定義

Selection bias 發生在研究對象的選擇方式導致即使現實中暴露與疾病無關，卻觀察到明顯關聯時。

### Non-Response Bias | 無回應偏差

**Example:** Swedish asthma study (Ronmark et al., 1999)
- 9,132人受邀參與問卷調查
- 回應率85%
- **無回應者中：吸菸者比例更高、呼吸症狀更多**

> 這說明不回應者與回應者有系統性差異，可能引入偏差。

### How to Minimize | 如何減少

| Strategy | Description |
|---|---|
| Maximize response rate | Keep participation attractive |
| Characterize non-responders | Use available data to compare |
| Document differences | Report potential impact |

### Exclusion Bias | 排除偏差

**The Reserpine and Breast Cancer Example (1974)**

Table 15-2: Reserpine-BC Matched-Pairs Analysis

| | Controls (+) | Controls (−) |
|---|---|---|
| **Cases (+)** | 8 | 45 |
| **Cases (−)** | 23 | 362 |

**Matched OR = 45/23 = 1.96**

**Problem Identified:**
- Controls excluded patients with certain conditions (cholecystectomy, cardiac surgery)
- These exclusions NOT applied to cases
- Result: Artificially low reserpine use in controls

**When Horwitz & Feinstein replicated with proper controls:**
- OR including all women = 1.1
- OR excluding cardiovascular disease = 2.5

> This demonstrated the original OR of 1.96 was due to **exclusion bias**.

---

## Information Bias | 資訊偏差

### Definition | 定義

Information bias 發生在獲取研究資訊的方法不完善時，導致暴露和/或疾病狀態的錯誤分類。

### Misclassification | 錯誤分類

**Types of Misclassification:**

| Type | Definition | Effect |
|---|---|---|
| **Differential** | Misclassification rate differs between groups | Can create OR bias in either direction |
| **Non-differential** | Same misclassification rate in all groups | Usually dilutes OR toward 1.0 |

### Table 15-3: Sources of Information Bias

| Source | Description |
|---|---|
| Record abstraction bias | Errors in reading medical records |
| Interviewer bias | Systematic differences in how questions are asked |
| Surrogate bias | Using family members as proxy respondents |
| Surveillance bias | More intense monitoring in exposed group |
| Recall bias | Cases remember exposures differently |
| Reporting bias | Reluctance to report sensitive information |
| Wish bias | Patients seek reasons for their illness |

### Recall Bias | 回憶偏差

**Case-Control Study Example:**
- Mothers of infants with malformations recalled prenatal infections more accurately
- Cases (affected) → Enhanced recall of exposure
- Controls (unaffected) → Less accurate recall

> **Differential misclassification** occurred → False association appeared.

### Surveillance Bias | 監測偏差

**Example: Oral Contraceptives and Thrombophlebitis**

Physicians monitored OC users more closely → Identified more thrombophlebitis cases

> This created a **spurious association** through better case ascertainment.

### Wish Bias | 心願偏差

Patients who develop disease may:
- Deny lifestyle exposures ("It wasn't my fault")
- Emphasize occupational exposures (if litigation pending)

---

## Confounding | 混雜

### Definition | 定義

**Confounding 發生在：**

因子 X 是疾病 B 的已知風險因子，且因子 X 與暴露 A 相關（但不是暴露 A 的結果），卻造成暴露 A 與疾病 B 的虛假關聯。

### Table 15-4: Criteria for a Confounder

| Criterion | Requirement |
|---|---|
| 1 | Must be associated with the exposure |
| 2 | Must be an independent risk factor for the disease |
| 3 | Must NOT be on the causal pathway between exposure and disease |

### The Classic Example: Coffee and Pancreatic Cancer

**Confounder: Smoking**

| Criterion | Smoking (X) vs. Coffee (A) | Pancreatic Cancer (B) |
|---|---|---|
| Associated with exposure? | ✓ Smokers drink more coffee | — |
| Risk factor for disease? | ✓ Known cause of pancreatic cancer | — |
| On causal pathway? | ✗ Coffee doesn't cause smoking | — |

**Result:** Coffee-BC association may be due to confounding by smoking.

### Figure 15-1: Confounding Diagram

```
Panel A: True Causal
Coffee → Pancreatic Cancer

Panel B: Due to Confounding
Coffee ← Smoking → Pancreatic Cancer
         ↑
    Confounder
```

### Addressing Confounding | 處理混雜

**In Study Design:**

| Method | Description |
|---|---|
| **Randomization** | Randomly assign exposure (eliminates confounding) |
| **Restriction** | Limit to specific subgroup |
| **Matching** | Match cases/controls on confounder |

**In Data Analysis:**

| Method | Description |
|---|---|
| **Stratification** | Analyze within strata of confounder |
| **Statistical adjustment** | Regression models (adjust for confounders) |

### Stratification Example | 分層分析範例

**Unadjusted OR = 1.95** (confounded by age)

After stratification by age:

| Stratum | OR |
|---|---|
| Age < 40 | 1.0 |
| Age ≥ 40 | 1.0 |

**Conclusion:** Age was the confounder. True OR = 1.0 (no association)

---

## Interaction (Effect Modification) | 交互作用

### Definition | 定義

**Interaction** occurs when the effect of one exposure on disease risk is modified by the presence of another factor.

> 也稱為 **Effect Modifier (效應修飾因子)** 或 **Synergism (协同作用)**。

### Additive vs. Multiplicative Models | 加法與乘法模型

**Table 15-5: Interaction Models**

| Model | Assessment |
|---|---|
| **Additive** | Is the combined effect greater than sum of individual effects? |
| **Multiplicative** | Is the combined effect greater than product of individual effects? |

### Example: Smoking and Asbestos

| Exposure | Lung Cancer Risk |
|---|---|
| Neither | 1.0 (baseline) |
| Smoking only | RR = 5 |
| Asbestos only | RR = 10 |
| Both | RR = 50 |

**Additive check:** 50 vs. 5 + 10 = 15 → **Synergistic (greater than additive)**
**Multiplicative check:** 50 vs. 5 × 10 = 50 → **Exactly multiplicative**

> 吸菸與石棉的組合效應遠大於兩者單獨效應之和。

### Identifying Interaction | 識別交互作用

| Method | Description |
|---|---|
| Stratified analysis | Compare stratum-specific ORs/RRs |
| Statistical test | Test for homogeneity across strata |
| Regression models | Include interaction term |

---

## Summary | 摘要

### Bias

| Type | Solution |
|---|---|
| Selection bias | Careful study design, representativeness |
| Information bias | Valid measurement tools, blinding |
| Recall bias | Use records, reduce differential |

### Confounding

| Prevention | Control |
|---|---|
| Randomization | Stratification |
| Matching | Statistical adjustment |
| Restriction | Multivariable analysis |

### Interaction

- Effect modification rather than bias
- Stratify to identify homogeneous subgroups
- Report stratum-specific estimates

---

## Review Questions | 複習問題

1. What is the difference between selection bias and information bias?

2. Give an example of differential misclassification versus non-differential misclassification.

3. What are the three criteria for a confounder?

4. In the reserpine-breast cancer study, what type of bias was demonstrated?

5. What is the difference between confounding and interaction?

6. If you suspected age was a confounder, how would you address it in analysis?
