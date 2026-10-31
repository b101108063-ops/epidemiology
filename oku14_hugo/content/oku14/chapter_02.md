---
title: "Chapter 2: Biostatistics (生物統計學): 骨科研究的設計、統計分析與文獻判讀"
date: 2026-10-31
draft: false
tags: ["Orthopaedics", "OKU14", "Biostatistics", "Research Methodology", "Evidence-Based Medicine"]
categories: ["General Topics"]
weight: 2
summary: "本章介紹骨科研究的描述性與分析性設計、病人報告式結果與最小臨床重要差異、假設檢定與檢定力分析、參數與非參數檢定之選擇、多變數與混因因子的處理，最後整理常見統計陷阱與文獻判讀重點。"
---

# Chapter 2: Biostatistics — 生物統計學

## 章節導讀

本章是骨科研究的方法學工具箱。骨科醫師不一定要自己跑統計，但必須能判讀研究設計、樣本數、效果量與信賴區間是否合理，並分辨「統計顯著」與「臨床重要」的落差。本章從研究設計分類講到 outcome measure、MCID、檢定力分析與各類檢定，最後整理骨科文獻最常見的統計陷阱。

---

## 1. 核心概念與研究設計 (Foundational Concepts & Study Design)

本章非解剖學章節，其「關鍵結構」為**研究設計的證據架構**：不同設計能回答的問題不同，推論範圍也不同。

<!-- FIG: Figure 2 — 研究設計分類圖（Analytic：RCT／Retrospective case-control／Cohort；Descriptive：Cross-sectional／Correlational／Case series & case reports）。 -->

### 1.1 描述性研究 (Descriptive Studies)

描述性研究只描述狀況或事件，**不提供變數間關係的解釋**，但可提供假設供後續研究。骨科文獻中最常見的報告形式即 case series。

| 描述性研究 | 定義 | 骨科實例 |
|-----------|------|---------|
| <span style="color:#e2e8f0">Cross-sectional</span> | 單一時間點收集資料 | 病人特性與術前疼痛期待 |
| <span style="color:#e2e8f0">Correlational</span> | 兩變數間的潛在關係 | 術前用藥與住院天數 |
| <span style="color:#e2e8f0">Case series</span> | 病人群描述，>10 人 | 10 位年輕病人軟骨碎片修補 |
| <span style="color:#e2e8f0">Case report</span> | 罕見疾病併發症，<10 人 | 71 歲女性置換後皮膚病灶 |

- **Cross-sectional**：可提供某事件的盛行率；成本低，但**無法解釋因果**。
- **Case report 應呈現 novelty（新穎性）**：疾病的非典型表現、疾病與症狀間的意外關聯、不良事件、新興疾病或罕見副作用。原文舉例：全膝關節置換後 7 週切口周圍散在搔癢性水疱。
- **Correlational study**：以族群層級的平均暴露水準探討兩變數關係；相關不等於因果，群體層級關係未必適用於個體，也未考慮混因因子。原文舉例：術前處方藥物使用與全髖關節置換住院天數，並控制年齡、種族、BMI、吸菸與保險。

> **Danger zone**：correlational study 只能說「關聯」，**不能宣稱術前用藥「造成」住院天數延長**。

### 1.2 分析性研究 (Analytic Studies)

分析性研究回答科學假設，並以樣本推論整體目標族群。

| 設計 | 分組依據 | 骨科實例與要點 |
|------|---------|-------------|
| <span style="color:#60a5fa">RCT</span> | 隨機分派、前瞻追蹤 | 翻修全膝關節傷口併發症高風險者：標準照護 vs. 切口密閉式負壓治療（ciNPT）。EBM 的 gold standard；對照可為既有治療或安慰劑 |
| <span style="color:#60a5fa">Cohort</span> | 依**暴露**分組 | 比較基線相近但暴露不同的兩組，可近似疾病發生率，並推論預後 |
| <span style="color:#60a5fa">Case-control</span> | 依**疾病狀態**分組 | 病例與對照比較暴露程度，求 **odds ratio** |

- **RCT 的缺點**：成本高、耗時、外科領域不總是可行或合乎倫理；因 selection bias，結果未必可推廣至全部族群（前述研究即不知適用於所有翻修病人，或僅高風險者）。多中心 RCT 可改善推論性。2012–2017 年 <span style="color:#f87171;font-weight:600">RCT 僅占 Bone & Joint Journal 原創研究 8%</span>。
- **Case-control 的難處**：界定**基礎族群（base population）**與選擇對照病人；結果為 odds ratio（暴露者罹病之 odds ÷ 未暴露者之 odds），罕見疾病或事件時可近似相對風險；OR < 1 為降低，OR > 1 為增加。

> **Pearl**：同一個「危險因子」問題，cohort（依暴露分組、算風險）與 case-control（依疾病分組、算 odds）量尺不同；閱讀時先確認切入端。

---

## 2. 結果測量與臨床重要性 (Outcome Measures & Clinical Significance)

### 2.1 病人報告式結果 (PROs, PROMs, PRO-PMs)

<span style="color:#e2e8f0">PROs</span>：直接來自病人、未經詮釋的健康狀況、行為與經驗。**<span style="color:#e2e8f0">PROMs</span>**：以問卷量化病人症狀的工具，用以估計手術效益與照護品質。**PRO-PMs**：PROM 的數值化量化，常為病人間彙總值，針對特定術式驗證。

| 骨科常用 PROM | 說明 |
|--------------|------|
| Knee Society Score、Hip Society Score | 關節別評分 |
| <span style="color:#e2e8f0">WOMAC</span> | Western Ontario and McMaster Universities Index |
| Oxford Knee Score、Oxford Hip Score | 病人自填 Oxford 系列 |
| SF-36、SF-12 | 通用健康相關生活品質 |
| UCLA Score、VAS（visual analog scale） | 肩關節評分、疼痛強度 |
| <span style="color:#60a5fa">HOOS</span>、<span style="color:#60a5fa">KOOS</span> | Hip Disability and Osteoarthritis Outcome Score／Knee Injury and Osteoarthritis Outcome Score；驗證最完善的關節別 PROM，納入 CJR 模型 |

- 目前**不存在**單一可靠且已驗證、可供跨研究比較的 PROM index；合用取決於疾病、部位或結果。
- **Performance testing**：病人執行特定測試固定時間，由醫師或物理治療師評分。例：<span style="color:#e2e8f0">AM-PAC</span>，評估爬樓梯、翻身需多少協助。
- PRO-PMs 用於 value-based healthcare 的品質面，並納入支付方案與 American Joint Replacement Registry 等登錄，以比較不同醫療者與醫療中心。

### 2.2 臨床重要性的量化指標 (MCID 與相關指標)

病人感受的是治療效果，而非 P 值；統計顯著未必讓病人感受到有意義的改變。

| 術語 | 定義 |
|------|------|
| <span style="color:#e2e8f0">MIC</span> | 相對於基線、cohort 報告生活品質改善的變化 |
| <span style="color:#e2e8f0">MID</span> | 病人認為重要的最小差距 |
| <span style="color:#60a5fa">MCID</span> | 無改善者與僅些微改善者之**平均變化差**（亦稱 MCIC、MCII） |
| <span style="color:#e2e8f0">MDC</span> | 單一病人能感受到改善的最小值 |
| <span style="color:#e2e8f0">CID</span> | 具臨床重要性的結果測量差距 |
| <span style="color:#e2e8f0">PASS</span> | patient acceptable symptom state；以二分法 PROM 為錨點辨識切點 |

- **MCID 定義方式**：**分布法**（distribution based）以 0.5 個標準差視為可被臨床察覺的差異，採此法時效益可能**高估**；**錨定法**（anchor based）將分數變化與「整體改善」連結。
- **Fragility Index（脆弱指數）**：為 RCT 設計的指標，採迭代方式將一名病人的結果在 event 與 nonevent 間移動，顯示 P 值判定的顯著性多易被推翻。
  - **Fragility Quotient** = Fragility Index ÷ 總樣本數。
  - **robust 報告法**：當**失訪人數 > Fragility Index** 時，該試驗標示為較不穩健；其詮釋具主觀性，目前**未定義穩健界限**。
- **Clinical Relevance Ratio**：先確立臨床關聯門檻將結果二分，再報告某時間點達成臨床重要之病人數 **除以** 起始病人數（含失訪）。

> **Pearl**：骨科尚無計算「臨床顯著變化」的標準做法；建議沿用**相似族群中已建立的指標**。

---

## 3. 統計檢定與樣本數計算 (Statistical Testing & Power Analysis)

### 3.1 第一型與第二型錯誤、檢定力

| 誤差類型 | 真實情況 | 報告結果 |
|---------|---------|---------|
| <span style="color:#f87171">Type I error</span>（α） | 兩治療**有**差異 | 判為**無**差異（false positive） |
| <span style="color:#f87171">Type II error</span>（β） | 兩治療**無**差異 | 判為**有**差異（false negative） |

- **Alpha（α）**：第一型錯誤的機會，即顯著水準，通常設 <span style="color:#34d399">5%</span>。
- **Beta（β）**：第二型錯誤的機會；**Power = 1 − β**，通常設 <span style="color:#34d399">80%</span>。
- **Power analysis**：提供主要結果所需最小觀察數的估計。

> **Danger zone**：原文表格標題掃描誤植為「Type I and Type I Errors」，實為 **Type I 與 Type II**；另「type II error … referred to as p」之 p 為希臘字母 **β** 的 OCR 誤讀。

### 3.2 樣本數計算的要素

樣本數受下列因素影響：測量變數數目、臨床顯著差異的量值、避免第一型錯誤的確定程度，以及所採用的統計檢定。

1. **先決定結果測量與 MCID** — clinically important difference 是樣本數計算的關鍵；差距過小可能統計顯著卻無臨床相關性。
2. **再決定檢定方法** — 理想狀況是與最終分析使用的檢定相同（one-/two-sample 或 paired）。
3. **設定 alpha 與 power** — α 一般 5%、power 一般 80%；**效應量愈大、SD 愈小，樣本數愈少**（SD 取自文獻或先導資料）。
4. **保守分析** — 參數（如 SD）不準確時應偏保守。
5. **考慮失訪** — 計入可能的 loss to follow-up。

| 常見檢定 | 應用 |
|---------|------|
| <span style="color:#e2e8f0">Student t-test</span> | 參數性；常態分布下比較兩組平均數（例：比較兩組病人年齡） |
| <span style="color:#e2e8f0">ANOVA</span>（>2 組） | 參數性；兩組以上平均數比較（例：治療三組之結果） |
| <span style="color:#e2e8f0">Chi-square test</span> | 非參數性；比較類別變數頻率（例：兩組女性參與者百分比） |
| <span style="color:#e2e8f0">Fisher exact test</span> | 頻數過小時之替代（列聯表任一期望值 <5） |
| <span style="color:#e2e8f0">Mann-Whitney U test</span> | 非參數性；以中位數比較兩組分布（例：兩組 PROM） |
| <span style="color:#e2e8f0">Kruskal-Wallis test</span> | 非參數性；三組以上（例：多組 PROM） |
| <span style="color:#e2e8f0">Kaplan-Meier curve</span> | 非參數性；time-to-event 與存活分析（例：植入物存活率） |
| <span style="color:#e2e8f0">Competing risk analysis</span> | 納入競爭事件機率的存活分析（高齡族群植入物存活率） |
| <span style="color:#e2e8f0">Logistic regression</span> | 二元事件之 odds 模型（例：吸菸者之翻修手術 odds） |
| <span style="color:#e2e8f0">AUC</span> | ROC 曲線之分類模型 goodness-of-fit |

### 3.3 假設檢定的原則

- **Null hypothesis（H₀）**：預設敘述，代表**無效應**。**Alternative hypothesis（H₁）**：代表效應存在或差異不等於零，即**雙側**假設，最常用。
- **P 值的定義**：在 H₀ 為真時，觀察到的差異純屬隨機發生的機率；機率過小則拒絕 H₀，主張統計顯著差異。
- **接受 H₀ ≠ 證明等價**：P 值大於門檻只能說「無法拒絕 H₀」；主張等價採 **two one-sided tests**（雙單側檢定）。
- 檢定應反映資料的分布型態與類型；趨勢是從假設檢定走向更多**估計**（CI、effect size）。

> **Pearl**：文獻常只報「用了什麼檢定 + P 值」，檢定前提多為隱含假設；應追問「前提在他們資料成立？」

### 3.4 多元資料與資料型態

| 變數數目 | 分類 |
|---------|------|
| 1 | <span style="color:#e2e8f0">Univariate</span>（單一變數） |
| 2 | <span style="color:#e2e8f0">Bivariate</span>（兩個變數） |
| ≥3 | <span style="color:#e2e8f0">Multivariate</span>（含一個以上**依變數**） |

| 多變數方法 | 目的 | 常用技術 |
|-----------|------|---------|
| <span style="color:#60a5fa">Dependence</span> | 檢視因果：一變數能否解釋或預測另一變數 | 迴歸分析、機器學習預測模型 |
| <span style="color:#fbbf24">Interdependence</span> | 理解資料型態，不賦予因果 | 因子分析、路徑分析、多變數 ANOVA |

- **非獨立性 (nonindependence)** 須特別處理，因多數檢定假定觀察值互相獨立：
  - **Longitudinal**：同一病人不同時間點。
  - **Clustered data**：每位病人一筆觀察，但以某醫師或醫院為群組聚集。
  - **Repeated measures**：測量多次，但分隔測量的效應**不是時間**而是其他效應。
  - 非獨立性來源可為相近時間窗內對相似樣本的觀察。
- **Data types**：quantitative（數值）／categorical（類別）決定可用檢定；**選檢定前先描述統計與繪圖**，偏離用非參數。

---

## 4. 統計陷阱與文獻判讀 (Common Statistical Pitfalls)

> **陷阱 1：把顯著性當成臨床重要性**。P 值只說明「不太可能純屬偶然」，病人關心效果大小；須同時看 MCID 與信賴區間。

> **陷阱 2：多重比較未校正**。多組比較或多種檢定同時進行會增加第一型錯誤風險；**Bonferroni correction** 將個別假設的顯著水準設為 α ÷ 比較次數。

> **陷阱 3：ANOVA 只告訴你「有差異」**。ANOVA 不指出哪兩組不同，須以 post hoc 檢定（t-test、Tukey-Kramer）做配對比較，並考慮多重比較校正。

> **陷阱 4：忽略檢定前提**。t-test 與 ANOVA 皆要求**觀察獨立、常態分布、變異數同質（homoscedasticity）**；樣本較大時因 central limit theorem 更容易滿足，分布明顯異常時改用非參數檢定（Mann-Whitney U、Wilcoxon signed-rank）。原文指出：即使僅輕微偏離，**t-test 仍優於非參數**。

> **陷阱 5：類別資料選錯檢定**。列聯表任一期望值 <5 應改用 **Fisher exact test**；配對資料用 **McNemar test**；三個類別變數（如分層 cohort）產生多張 2×2 表，考慮 **Cochran-Mantel-Haenszel**。

> **陷阱 6：混因因子未受控制**。混因因子是同時影響兩主要變數關係的第三變數。例如年齡影響治療對結果的效應，若兩組年齡不同而年齡又影響結果，年齡即為混因因子。可藉由**適當隨機化、跨 cohort 配對**控制，或以**多變數迴歸**納入模型。

> **陷阱 7：文獻中的偏差來源**。包括利益衝突（conflict of interest）、產業相關偏差、樣本數錯誤與偏好發表正向結果。**CONSORT**（RCT 報告清單與流程圖）與 **PRISMA**（SR/meta-analysis 規範）為降低偏差的規範。

> **陷阱 8：把 P 值當成唯一資訊**。可另報 Fragility Index、Fragility Quotient、Clinical Relevance Ratio 評估穩健性。

---

## 5. 實證更新與 OKU 14 重點 (Recent Evidence & Take-Home Points)

### 5.1 本章工具與重點整理

- **研究設計**：Analytic 回答假設；Descriptive 描述現象並產生假設；correlational 相關不等於因果，case-control 依疾病分組算 OR。
- **RCT 現況**：2012–2017 年 Bone & Joint Journal 原創研究 RCT 僅占 <span style="color:#f87171">8%</span>。
- **PROM**：HOOS 與 KOOS 驗證最完善；無單一可比 index。
- **臨床重要性**：MCID、MIC、MID、MDC、CID、PASS 定義不同，切勿混用。
- **檢定力**：α = 5%、power = 80% 為慣例；須計入失訪。
- **Fragility Index**：反映統計脆弱性；失訪數 > FI 較不穩健。
- **報告規範**：CONSORT、PRISMA。

### 5.2 骨科專科考試核心總結（Take-Home Points）

1. **研究設計對應問題**：「治療有效嗎」→ RCT；「危險因子預後」→ cohort；「罕見結果關聯」→ case-control（OR）；「發生率」→ cross-sectional。
2. **統計顯著 ≠ 臨床重要**：MCID 是樣本數計算起點，也是判讀效益的尺度；fragility 的意義是 P 值 0.049 與 0.051 只差「一名病人」。
3. **多重比較必須校正**（Bonferroni）；ANOVA 顯著後仍需 post hoc 才知道差在哪兩組。
4. **檢定前提要自己驗**：常態、變異數同質、觀察獨立；不符時改用非參數檢定。混因因子由隨機化／配對 + 多變數迴歸控制。

---

## References

1. Sackett DL, Rosenberg WMC, Gray JAM, et al: Evidence based medicine: What it is and what it isn't. Br Med J 1996;312(7023):71-72.
2. Jolles BM, Martin E: Statistics in brief - Study designs in orthopaedic clinical research. Clin Orthop Relat Res 2011;469(3):909-913.
3. Robinson AHN, Johnson-Lynn SE, Humphrey JA, et al: Challenges of translating RCT results into clinical practice. Bone Joint J 2019;101-B(2):121-123.
4. Higuera-Rueda CA, Emara AK, Nieves-Mallory Y, et al: Closed-incision negative-pressure therapy versus silver-impregnated dressings in revision knee arthroplasty: The PROMISES RCT. J Arthroplasty 2021;36(7):S295-S302.e14.
5. Clement ND, Bardgett M, Weir D, et al: Minimum clinically important difference for the WOMAC index after TKA? Clin Orthop Relat Res 2018;476(10):2005-2014.
6. Ridgeon EE, Young PJ, Bellomo R, et al: The fragility index in multicenter randomized controlled critical care trials. Crit Care Med 2016;44(7):1278-1284.
7. Checketts JX, Scott JT, Meyer C, et al: The robustness of trials that guide evidence-based orthopaedic surgery. J Bone Joint Surg Am 2018;100(12):e85.

8. Siljander MP, McQuivey KS, Fahs A, et al: Current trends in patient-reported outcome measures in total joint arthroplasty: A study of 4 major journals. J Arthroplasty 2018;33(11):3416-3421.
9. Ramkumar PN, Harris JD, Noble PC: Patient-reported outcome measures after total knee arthroplasty: A systematic review. Bone Joint Res 2015;4(7):120-127.
10. Maltenfort M, Diaz-Ledezma C: Statistics in brief: Minimum clinically important difference. Clin Orthop Relat Res 2017;475(4):933-946.
11. Tignanelli CJ, Napolitano LM: The fragility index in randomized clinical trials for optimizing patient care. JAMA Surg 2019;154(1):74-79.
12. Williams PJ, Murphy P, Van Koughnett JAM, et al: Statistical techniques in general surgery literature. J Am Coll Surg 2018;227(4):450-454.

---

## Summary

- <span style="color:#60a5fa;font-weight:600">研究設計</span>：Analytic（RCT／cohort／case-control）回答假設；Descriptive 描述現象並產生假設；case-control 依疾病分組算 OR，cohort 依暴露推論預後。
- <span style="color:#f87171;font-weight:600">RCT 比例偏低</span>：2012–2017 年 Bone & Joint Journal 原創研究中 RCT 僅占 8%；selection bias 限制推論性。
- <span style="color:#60a5fa;font-weight:600">PROM</span>：常用 Knee/Hip Society Score、WOMAC、Oxford 系列、SF-36/12、UCLA Score、VAS；HOOS 與 KOOS 驗證最完善；無單一跨研究可比 index。
- <span style="color:#60a5fa;font-weight:600">臨床重要性</span>：MIC、MID、MCID、MDC、CID、PASS 定義不同；MCID 可採分布法（0.5 SD，易高估）或錨定法。
- <span style="color:#60a5fa;font-weight:600">檢定力</span>：α = 5%、power = 80% 為慣例；樣本數須以 MCID 為起點、計入失訪；power = 1 − β。
- <span style="color:#60a5fa;font-weight:600">Fragility Index</span>：Fragility Quotient = FI ÷ 總樣本數；失訪人數 > FI 較不穩健。
- <span style="color:#fbbf24;font-weight:600">檢定選擇</span>：兩組用 t-test、多組用 ANOVA、分類資料用 chi-square（期望值 <5 改 Fisher exact、配對用 McNemar、分層用 CMH）；多重比較須 Bonferroni 校正。
- <span style="color:#f87171;font-weight:600">前提與混因</span>：須滿足觀察獨立、常態分布、變異數同質；混因以隨機化／配對及多變數迴歸控制。
- <span style="color:#34d399;font-weight:600">報告規範</span>：CONSORT 與 PRISMA 為降低偏差的工具。
