---
title: "Chapter 11: Estimating Risk: Is There an Association?"
titleTC: "風險估計：是否存在關聯？"
description: "Gordis Epidemiology Chapter 11 - Estimating Risk: Is There an Association?"
draft: false
---

# Chapter 11: Estimating Risk: Is There an Association?
## 風險估計：是否存在關聯？

## Learning Objectives | 學習目標

By the end of this chapter, you should be able to:

- Differentiate between **relative risk (RR)** and **attributable risk (AR)**
- Calculate and interpret the **odds ratio (OR)**
- Explain when the odds ratio approximates relative risk
- Understand the relationship between incidence and risk

---

## Introduction | 導論

When we conduct an epidemiologic study, we often begin by asking a fundamental question: **Is there an association between an exposure and a disease?**

This chapter focuses on how we measure and quantify that association. We will examine different measures of risk and learn how to interpret them in the context of disease etiology.

> **臨床重點**
> 理解風險測量不僅是研究方法的核心，也是臨床決策的基礎。醫師在建議患者時，必須了解暴露與疾病之間關聯的強度。

---

## Measures of Association | 關聯測量

### Relative Risk (RR) | 相對風險

The **relative risk (RR)**, also called **risk ratio**, compares the incidence of disease in the exposed group to the incidence in the nonexposed group.

**Formula 11-1: Relative Risk**

```
        Incidence in exposed group
RR = ─────────────────────────────────
      Incidence in nonexposed group
```

| Interpretation of RR | Meaning |
|---|---|
| RR = 1.0 | No association (same risk in both groups) |
| RR > 1.0 | Increased risk in exposed group (positive association) |
| RR < 1.0 | Decreased risk in exposed group (protective association) |

### Odds Ratio (OR) | 勝算比

The **odds ratio (OR)** is calculated from case-control studies where we cannot directly calculate incidence. It compares the odds of exposure among cases to the odds of exposure among controls.

**Formula 11-2: Odds Ratio**

```
        Odds of exposure in cases
OR = ─────────────────────────────
      Odds of exposure in controls
```

Using a 2×2 table:

|  | Disease (Cases) | No Disease (Controls) |
|---|---|---|
| **Exposed** | a | b |
| **Not Exposed** | c | d |

```
        a × d
OR = ─────────
        b × c
```

### Relationship Between OR and RR | 勝算比與相對風險的關係

When disease is **rare** (which is often the case in case-control studies), the **odds ratio approximates the relative risk**. This is because:

> When prevalence is low, the odds of disease ≈ the risk of disease

This approximation becomes more accurate as the disease becomes rarer.

---

## The 2×2 Table | 2×2 表格

The fundamental tool for calculating measures of association is the **2×2 contingency table**.

### Standard Layout

|  | Disease (+) | Disease (−) | Total |
|---|---|---|---|
| **Exposed (+)** | a | b | a + b |
| **Not Exposed (−)** | c | d | c + d |
| **Total** | a + c | b + d | a + b + c + d |

### Calculations from the 2×2 Table

| Measure | Formula | Interpretation |
|---|---|---|
| **Incidence in exposed** | a / (a + b) | Risk among those with exposure |
| **Incidence in nonexposed** | c / (c + d) | Risk among those without exposure |
| **Relative Risk (RR)** | [a/(a+b)] / [c/(c+d)] | How many times greater risk in exposed |
| **Odds Ratio (OR)** | (a×d) / (b×c) | Ratio of exposure odds |
| **Attributable Risk (AR)** | [a/(a+b)] − [c/(c+d)] | Excess risk due to exposure |

---

## Understanding Risk | 風險的理解

### What Is Risk? | 什麼是風險

**Risk** is the probability that a disease will occur in a specific time period. It is calculated as:

```
Risk = Number of new cases / Population at risk
```

### Cumulative Incidence | 累積發生率

Cumulative incidence represents the proportion of a disease-free population that develops the disease during a specified time period:

```
Cumulative Incidence = New cases during time period / Disease-free population at start
```

### Incidence Rate | 發生率

When population size changes during the study period, we use incidence density:

```
Incidence Rate = New cases during time period / Person-time at risk
```

---

## Appendix: Mathematical Relationship Between OR and RR | 附錄：勝算比與相對風險的數學關係

### Derivation | 推導

Given the 2×2 table above, the **relative risk** is:

```
       a / (a + b)
RR = ─────────────────
       c / (c + d)
```

The **odds ratio** is:

```
       a × d
OR = ─────────
       b × c
```

The ratio of RR to OR can be expressed as:

```
      RR   (a / (a + b)) / (c / (c + d))
────── = ──────────────────────────────────
      OR          ad / bc
```

This simplifies to:

```
      RR   b / (a + b) × d / (c + d)
────── = ───────────────────────────────
      OR          1
```

### Rare Disease Approximation | 罕見疾病近似

When the disease is rare:
- a / (a + b) → very small
- c / (c + d) → very small

The terms in the formula approach 1, so:

> **RR ≈ OR when disease is rare**

This is why we can use odds ratios from case-control studies as a valid estimate of relative risk in most practical situations.

---

## Summary | 摘要

本章介紹了流行病學中測量關聯性的核心概念：

1. **相對風險 (RR)**：比較暴露組與非暴露組的發病率，是隊列研究中的首選測量
2. **勝算比 (OR)**：從病例對照研究計算，當疾病罕見時可近似 RR
3. **2×2 表格**：計算所有測量值的基礎工具
4. **稀有疾病近似**：當疾病發生率低時，OR 是 RR 的良好近似值

這些測量構成後續章節討論因果推論與預防潛力的基礎。

---

## References | 參考文獻

1. Gordis L. Epidemiology. 5th edition. Philadelphia: Elsevier Saunders; 2013.
2. Rothman KJ, Greenland S, Lash TL. Modern Epidemiology. 3rd edition. Philadelphia: Lippincott Williams & Wilkins; 2008.
