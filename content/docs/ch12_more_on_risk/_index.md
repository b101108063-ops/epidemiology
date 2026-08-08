---
title: "Chapter 12: More on Risk: Estimating the Potential for Prevention"
titleTC: "風險進一步探討：估計預防潛力"
description: "Gordis Epidemiology Chapter 12 - More on Risk: Estimating the Potential for Prevention"
draft: false
---

# Chapter 12: More on Risk: Estimating the Potential for Prevention
## 風險進一步探討：估計預防潛力

## Learning Objectives | 學習目標

By the end of this chapter, you should be able to:

- Calculate and interpret the **attributable risk (AR)** for the exposed group
- Calculate and interpret the **population attributable risk (PAR)**
- Explain how attributable risk relates to prevention potential
- Compare relative risk and attributable risk in clinical applications

---

## Introduction | 導論

上一章節我們討論了**相對風險 (RR)** 和**勝算比 (OR)**，這些測量告訴我們暴露與疾病之間關聯的強度。然而，臨床醫師和公共衛生人員常問的另一個問題是：

> **「如果我們能消除這個危險因子，能預防多少疾病？」**

這正是**歸因風險 (Attributable Risk)** 要回答的問題。

> **臨床重點**
> 當醫師建議患者戒菸時，背後的思考是：「戒菸能降低多少心臟病風險？」這個思考正是基於歸因風險的概念。

---

## Attributable Risk for the Exposed Group | 暴露組的歸因風險

### Concept | 概念

**Attributable risk (AR)** 是指在暴露組中，發病率中有多少是因為該暴露而額外增加的。

Figure 12-1 以圖示說明這個概念：

- 暴露組的總風險 = 背景風險 + 暴露造成的額外風險
- **歸因風險 = 暴露組風險 − 非暴露組風險（背景風險）**

### Formula | 公式

**Formula 12-1: Attributable Risk (絕對值)**

```
AR = Incidence in exposed group − Incidence in nonexposed group
```

**Formula 12-2: Attributable Risk Proportion (百分比)**

```
     Incidence in exposed − Incidence in nonexposed
AR% = ───────────────────────────────────────────── × 100%
              Incidence in exposed group
```

AR% 代表：「在暴露組的所有病例中，有多少比例是因為暴露而造成的」

### Interpretation | 解釋

| AR Value | Interpretation |
|---|---|
| **AR = 10/1,000** | 每1,000名暴露者中，有10例額外病例是因為暴露 |
| **AR% = 37.9%** | 暴露組37.9%的病例是因為暴露造成的 |

> **臨床重點**
> 如果吸菸者的肺癌歸因風險為 92.9%，這表示戒菸理論上可預防吸菸者中 92.9% 的肺癌病例。

---

## Population Attributable Risk (PAR) | 族群歸因風險

### Concept | 概念

公共衛生決策者關心的不只是暴露組，而是**整個族群**。Population Attributable Risk (PAR) 問的是：

> **「在整個族群中（包括暴露與非暴露者），有多少疾病是因為這個暴露造成的？」**

### Formula | 公式

**Formula 12-3: Population Attributable Risk (絕對值)**

```
PAR = Incidence in total population − Incidence in nonexposed group
```

**Formula 12-4: Population Attributable Risk Proportion (百分比)**

```
          Incidence in total population − Incidence in nonexposed
PAR% = ────────────────────────────────────────────────────────── × 100%
                   Incidence in total population
```

### Alternative Calculation (Levin's Formula) | 替代計算方法

```
PAR% = P(e) × (RR − 1) / [P(e) × (RR − 1) + 1]

其中：
P(e) = 族群中暴露者的比例
RR = 相對風險
```

---

## Worked Examples | 實例計算

### Example 1: CHD and Smoking | 吸菸與冠狀動脈心臟病

From a hypothetical cohort study:

|  | CHD Develops | CHD Does Not Develop | Total | Incidence per 1,000/year |
|---|---|---|---|---|
| **Smokers** | 84 | 2,916 | 3,000 | 28.0 |
| **Nonsmokers** | 87 | 4,913 | 5,000 | 17.4 |

**Step 1: Calculate Attributable Risk (exposed group)**

```
AR = 28.0 − 17.4 = 10.6 per 1,000 per year
```

Interpretation: 每1,000名吸菸者中，每年有10.6例額外CHD病例是因為吸菸。

**Step 2: Calculate Attributable Risk Proportion**

```
AR% = (28.0 − 17.4) / 28.0 × 100% = 37.9%
```

Interpretation: 吸菸者中37.9%的CHD病例可歸因於吸菸。

**Step 3: Calculate PAR (假設吸菸者佔族群44%)**

```
Incidence in total population = (0.44 × 28.0) + (0.56 × 17.4) = 22.1 per 1,000

PAR = 22.1 − 17.4 = 4.7 per 1,000 per year

PAR% = (22.1 − 17.4) / 22.1 × 100% = 21.3%
```

Interpretation: 整個族群中21.3%的CHD病例可歸因於吸菸。

---

### Example 2: Doll and Peto Study | Doll與Peto研究

吸菸與死亡的英國醫師研究數據：

| Cause of Death | Smokers (per 100,000) | Nonsmokers (per 100,000) | RR | AR (per 100,000) | AR% |
|---|---|---|---|---|---|
| **Lung Cancer** | 140 | 10 | 14.0 | 130 | 92.9% |
| **Coronary Heart Disease** | 669 | 413 | 1.6 | 256 | 38.3% |

**Key Insight:**

> 肺癌的**相對風險**（14.0）遠高於冠心病（1.6），但冠心病的**歸因風險**（256人/10萬）卻是肺癌（130人/10萬）的近兩倍！

這說明一個重要概念：
- **相對風險**告訴我們「這個暴露有多危險」
- **歸因風險**告訴我們「消除這個暴露能救多少人命」

---

## Comparison: Relative Risk vs. Attributable Risk | 比較：相對風險 vs. 歸因風險

| Feature | Relative Risk (RR) | Attributable Risk (AR) |
|---|---|---|
| **Purpose** | Measure strength of association | Measure potential for prevention |
| **Clinical Use** | Etiologic research, causal inference | Clinical counseling, public health planning |
| **Calculation** | Ratio of risks | Difference of risks |
| **Interpretation** | 「暴露者風險是非暴露者的X倍」 | 「消除暴露可預防X例疾病」 |

> **臨床重點**
> 相對風險高 ≠ 公共衛生 impact 大。必須同時考慮暴露的普遍性與歸因風險，才能制定有效的公共衛生政策。

---

## Applications in Public Health | 公共衛生應用

### Leading Causes of Death (US, 2000)

| Risk Factor | % of All Deaths |
|---|---|
| Tobacco | 18.1% (435,000) |
| Diet & Physical Inactivity | 15.2% (365,000) |
| Alcohol Consumption | 3.5% (85,000) |
| Microbial Agents | 3.1% (75,000) |
| Toxic Agents | 2.3% (55,000) |
| Motor Vehicle | 1.8% (43,000) |
| Firearms | 1.2% (29,000) |
| Sexual Behavior | 0.8% (20,000) |
| Illicit Drug Use | 0.7% (17,000) |

> 菸草與飲食/活動模式合計佔死亡原因的33%，代表最大的預防潛力。

### Legal Applications | 法律應用

在毒性侵權訴訟中，歸因風險 > 50% 可能作為「more likely than not」的法律標準。

---

## Summary | 摘要

本章節介紹了歸因風險的核心概念：

1. **歸因風險 (AR)**：衡量暴露組中多少疾病可歸因於該暴露
2. **族群歸因風險 (PAR)**：衡量整個族群中多少疾病可歸因於該暴露
3. **預防潛力**：歸因風險直接回答「消除暴露能預防多少疾病」
4. **RR vs. AR**：RR 告訴我們暴露的危險性，AR 告訴我們公共衛生的 impact

這些概念為第14章的因果推論奠定了基礎。

---

## References | 參考文獻

1. Gordis L. Epidemiology. 5th edition. Philadelphia: Elsevier Saunders; 2013.
2. Doll R, Peto R. Mortality in relation to smoking: Twenty years' observations on male British doctors. Br Med J 2:1525–1536, 1976.
3. Levin ML. The occurrence of lung cancer in man. Acta Unio Int Contra Cancrum 9:531, 1953.
4. Mokdad AH, et al. Actual causes of death in the United States, 2000. JAMA 291:1238–1245, 2004.
