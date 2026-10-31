---
title: "Chapter 1: Orthopaedic Research (骨科研究方法與實證層級): 研究設計與臨床實務指引之建立"
date: 2026-10-31
draft: false
tags: ["Orthopaedics", "OKU14", "Evidence-Based Medicine", "Research Methodology"]
categories: ["General Topics"]
weight: 1
summary: "本章界定骨科研究從 bench-to-bedside 的轉譯路徑，說明 RCT、cohort、case-control、case series 與 expert opinion 的證據層級差異，並以 PICO、PRISMA、GRADE 與 AMSTAR 2 建立臨床實務指引（clinical practice guideline）的標準流程。"
---

# Chapter 1: Orthopaedic Research — 骨科研究方法與實證層級

## 章節導讀

骨科研究的價值取決於設計與證據強度能否回答真正的臨床問題。本章先建立從基礎研究到臨床應用的轉譯層次，再依 RCT、cohort、case-control 等設計說明證據強度差異，最後以 PICO、PRISMA、GRADE 與 AMSTAR 2 示範如何將文獻轉為臨床實務指引。

## 1. 臨床評估與關鍵解剖 (Anatomy & Deforming Forces)

本章非解剖學章節，「關鍵結構」係指**研究證據金字塔（evidence hierarchy）**與**臨床決策所依賴的資料組成**；骨科醫師在面對一項臨床決策時，必須先辨識該決策所依賴的證據類型與其結構性弱點。

### 1.1 Bench-to-Bedside 轉譯層次（Translational Science Spectrum）

| 層次 | 研究內容 | 對臨床決策的意義 |
|------|----------|------------------|
| **Basic science**（benchtop） | 遺傳、分子、細胞訊息傳遞路徑；疾病病理機轉與治療設計 | 機轉假設來源，無法直接推論臨床效果 |
| **Preclinical research** | 體外細胞／組織培養、小動物模式、大動物模式 | 探討疾病與療法；新藥或新術式進入人體試驗前的必經階段 |
| **Early clinical research** | Phase I/II、可行性與安全性 | 確立劑量、可行性、初步療效訊號 |
| **Late clinical research** | Phase III/RCT、樞紐試驗 | 最高層級的療效與安全性證據 |
| **Clinical implementation** | Real-world evidence、big data、 registries | 真實世界適用性與外部效度 |

> **Pearl**：National Institutes of Health National Center for Advancing Translational Sciences 將 translational science 定義為「專注於理解轉譯過程每一步驟之科學與操作原則的研究領域」。臨床醫師若不理解轉譯層次，便無法判斷一項「漂亮」的 bench 發現是否真的能改變臨床處置。

### 1.2 骨科特有的結構性限制（Deforming Forces on the Evidence Base）

- **外科決策即時性**：手術中的 on-the-spot decisions 受 surgical community 內部 socialized knowledge 影響，臨床試驗難以複製此情境。
- **Complexity of intervention**：手術為複雜性介入（complex intervention），具有高度變異性。
- **Sham surgery 與 double blinding 倫理困難**：安慰劑手術（sham surgery）與治療端盲法在骨科領域可行性低。
- **結果**：骨科領域 RCT 的比例顯著低於其他醫療專科，描述性研究（descriptive studies）占多數。

> **Danger zone（研究判讀陷阱）**：當臨床研究僅比較 surgical technique 而非 surgical indication 時，其結果僅能回答「如何做」，不能回答「何時做」。跨研究外推時須先核對 inclusion criteria 是否反映真實臨床族群。

---

## 2. 分型系統與決策矩陣 (Classification & Decision Making)

### 2.1 研究設計與證據層級（Levels of Evidence）

| Level | 研究類型 | 臨床決策意義 |
|-------|----------|-------------|
| **I** | Randomised controlled trial；RCT 的 systematic review | 最高證據等級；RCT 依嚴謹度可為 Level I 或 II |
| **II** | Individual RCT（信賴區間寬時）；inception cohort study 且 follow-up >80%、CDR 已在單一族群驗證 | 可支持因果推論；品質次於 I |
| **III** | Prospective cohort study | 觀察性研究最高層級；可研究多變數或無法隨機化的治療 |
| **IV** | Case-control study、retrospective cohort study、case series | 適用罕見結果；受限於單一 outcome、抽樣與回憶偏差（sampling/recall bias） |
| **V** | Expert opinion | 不等同系統性研究結果；僅作方向性指引 |

**特殊分級補充**
- **Inception cohort**（起始世代 cohort）：若為前瞻、控制良好且 CDR 經單一族群驗證，可升級至 Level II。
- **「-」標記**：若單一結果之 confidence interval 過寬，或 systematic review 存在 troublesome heterogeneity，於等級數字後加「-」，表示該研究未能提供結論性答案。
- **Poor quality cohort study 定義**：未清楚界定比較組、未以相同（最好為盲法、客觀）方式測量暴露與結果、未識別或適當控制已知混因因子、或追蹤期不足且不完整。
- **Poor quality case-control study 定義**：同上，適用於 case 與 control 兩組。

### 2.2 研究設計之分類架構

| 類別 | 設計 | 起點 | 比較對象 |
|------|------|------|----------|
| **Descriptive**（描述性） | Case series、case report | 特定診斷或介入之病例群 | 無對照組 |
| **Analytic**（分析性） | RCT | Exposure（介入） | 隨機分派之另一組 |
| | Cohort | Exposure（暴露） | 有暴露 vs. 無暴露 cohort |
| | Case-control | Outcome（結果） | 有結果（case）vs. 無結果（control） |

### 2.3 判讀文獻的提問矩陣（Internal vs. External Validity）

| 內部效度（Internal）— 研究的說法可信嗎？ | 外部效度（External）— 結果有意義嗎？ |
|---|---|
| 研究是否測量了它宣稱測量的東西？ | 結果能否轉譯到我的臨床？ |
| 是否進行隨機化（randomization）？ | 研究的病人是否與我的病人不同？ |
| 是否進行盲法（blinding）？ | 如何將結果套用到我的病人？ |
| 隨機分組的組別 baseline 是否相似？ | |
| 追蹤期間為何？ | |
| 有多少病人退出研究？ | |
| 效益是否值得其風險與成本？ | |

### 2.4 假設與變數（Proper Study Design）

- **Null hypothesis（H₀）**：組間無統計差異；在出現顯著資料支持拒絕之前，皆視為成立。
- **Alternative hypothesis（H₁）**：存在效應。
- **Independent variable**：預期影響結果的變數（如 BMI）；**Dependent variable**：受其影響的結果變數（如 complication rate）。
- **重要提醒**：independent 與 dependent variable 之關係**並非必然線性**。以 THA 併發症率為例，BMI **過高或過低**（超出 normal-to-overweight 範圍）併發症率皆顯著較高。

---

## 3. 治療指引：手術 vs. 保守 (Treatment Algorithm)

本章不涉及手術與保守治療的取捨，其「治療指引」對應的是**證據轉譯成臨床處置的決策流程**。

### 3.1 PICO 問題建構（Table 2 之實際應用）

以臨床問題「acetaminophen 對治療骨關節炎有何效用？」為例：

| PICO 要素 | 定義 | 範例填答 |
|----------|------|----------|
| **P — Population / Patient / Diagnosis / Condition** | 所研究疾病最重要的特徵（年齡、診斷、疾病嚴重度、共病） | 成人 primary knee osteoarthritis，無重大共病 |
| **I — Intervention / Exposure** | 介入內容（藥物、劑量、頻率、給藥途徑） | 口服 acetaminophen 3,000 mg/day |
| **C — Comparison** | 對照方案（安慰劑、無治療、usual care、gold standard） | Placebo |
| **O — Outcome** | 關注結果（死亡、TJR、疼痛、功能） | 疼痛、功能分數變化 |

> **Pearl**：完整 PICO 敘述範例——「acetaminophen [I] 與 placebo [C] 相比，對成人 knee osteoarthritis [P] 的疼痛與功能分數變化 [O] 有何效益與危害？」

### 3.2 Systematic Review 與 Meta-analysis 的執行步驟（Figure 1）

1. **Formulate study question**（PICO）
2. **Establish protocol** — 依 PRISMA-P（Preferred Reporting Items for Systematic Review and Meta-Analysis Protocols）撰写研究計畫書
3. **Register** — 於 PROSPERO（International Prospective Register of Systematic Reviews）登錄
4. **Literature search and retrieval** — **至少兩個電子資料庫**（PubMed、Medline、Embase 或 Cochrane）＋ 手動搜尋參考文獻（hand searching article bibliographies）
5. **Study selection per protocol** — 由**至少兩位審查者**依 inclusion/exclusion criteria 篩選
6. **Data extraction**
7. **Critical appraisal / Quality assessment**
8. **Analysis and interpretation**

### 3.3 兩種 Meta-analysis 模型之決策矩陣（Table 3）

| 比較項目 | Fixed-Effect Model | Random-Effects Model |
|---------|--------------------|---------------------|
| 假設 | 所有研究的族群效應量相同 | 所選研究為更大族群的隨機樣本 |
| 納入誤差 | 僅考慮 within-study error | 同時考慮 within-study error 與 between-study variation |
| 權重分配 | 權重給予 precision 較高之研究 | 權重分配以最小化兩種變異來源 |
| 適用情境 | **僅能用於對納入研究本身做推論** | 嘗試將結論外推至納入研究之外 |

### 3.4 偏差控制與報告規範

- **Cochrane risk of bias tool**（RCT 品質評估）常評估參數：**allocation concealment（selection bias）、blinding of participants and personnel（performance bias）、blinding of outcome assessment（detection bias）、withdrawals（attrition bias）、reporting accuracy（reporting bias）**。
- **Proper randomization、standardized prospective data collection、patient and provider blinding、active follow-up measures** 可降低上述偏差。
- **Publication bias**：負面結果與小樣本研究較少被發表。
- RCT 之 systematic review 依 **PRISMA 2020** 報告；觀察性研究之 systematic review 優先依 **MOOSE**（Meta-analysis of Observational Studies in Epidemiology）規範。
- **AMSTAR / AMSTAR 2** 為評量 systematic review 品質、可重現評估的工具。

### 3.5 Clinical Practice Guideline 的建立（AAOS 流程）

**National Academy of Medicine 定義**：clinical practice guidelines 為「包含建議、旨在優化病人照護、且以系統性文獻回顧之證據與替代照護方案之效益／危害評估為基礎的陳述」。

**建立流程**：定義臨床問題與病人族群 → 組成 guideline development group → 評估最佳可得證據 → 創造並傳播 guideline。AAOS 實際流程為：選定題目 → 建立 PICO 問題 → 執行 systematic review 與 meta-analysis → 依最佳證據評估後做出帶強度分級的建議 → **peer review 與 community review** → 出版。

### 3.6 建議強度分級（Grades of Recommendations）

| 等級 | 來源 |
|------|------|
| **Strong**（強烈） | 綜合二項以上高證據層級（high level of evidence）研究 |
| **Moderate**（中等） | 證據品質次高 |
| **Limited**（有限） | 有限數量或較低品質之研究 |
| **Consensus**（共識） | 無研究可用，但專家意見可提供指引方向 |

> **Pearl**：GRADE（Grading of Recommendations, Assessment, Development and Evaluation）之流程為：PICO 問題 → systematic reviews → 對每一重要 outcome 產生效應估計 → 跨研究評定每一 outcome 的證據品質 → 評定整體證據品質（取關鍵 outcome 中最低者）→ 決定方向（支持／不支持）→ 評定建議強度（strong／weak）。

---

## 4. 手術入路與危險地雷 (Surgical Approach & Pearls)

本章無手術內容；以下為**文獻判讀與研究方法學的「操作陷阱」與防守技巧**。

> **陷阱 1：把觀察性關聯當成因果**。Cohort study 與 case-control study 僅能證明 association。BMI 與 THA 併發症的關係為非線性（U 型），單純以「越高越差」推論會誤導風險溝通。

> **陷阱 2：忽略 case-control 的單一 outcome 限制與 recall bias**。若研究設計只對一個結果追問暴露，任何暴露—結果交互作用都將被掩蓋。

> **陷阱 3：錯用 fixed-effect 模型做外推**。Fixed-effect 僅可對納入研究本身推論；若要外推至更廣族群，應採 random-effects，並做 multiway sensitivity analyses。

> **陷阱 4：將 systematic review 等同高质量**。必須以 AMSTAR 2 區分高低品質系統性回顧；未依 PRISMA/MOOSE 報告者，其 pooled estimate 需降級解讀。

> **陷阱 5：open access 中的 predatory publishing**。2021 年 DOAJ 已收錄超過 16,000 本 open access 期刊；因成本由作者端支付（large article processing charges），易生掠奪性期刊。讀者須留意 publisher 與作者的 conflict 與 motivation。傳統訂閱期刊亦常設 open access partner journal：稿件遭退稿後可改投 partner 期刊並獲得自動評估。

---

## 5. 實證更新與 OKU 14 重點 (Recent Evidence & Take-Home Points)

### 5.1 OKU 14 強調之實證與工具

| 主題 | 來源／工具 | 要點 |
|------|------------|------|
| **Levels of Evidence（OCEBM 2011）** | Howick J, Chalmers I, Glasziou P, et al.；JBJS 2003 引入 levels of evidence | 依研究設計分 Level I–V；臨床問題型態（therapy/prevention、etiology/harm、prognosis、diagnosis、differential diagnosis、prevalence、economic analysis）各有對應分級表 |
| **Bias 與 Level of Evidence 的關聯** | Pannucci CJ, Wilkins EG | 方法學薄弱的研究（case report、expert opinion）較易引入偏差；研究設計與嚴謹度提升則偏差風險下降；偏差可發生於設計至資料分析各階段 |
| **RoB 2** | Sterne JAC, et al. BMJ 2019;366:j4008 | 隨機對照試驗之新版偏差風險評估工具 |
| **AMSTAR / AMSTAR 2** | Shea BJ, et al. BMJ 2017;358:j4008 | 系統性回顧之關鍵方法學品質評估工具 |
| **PRISMA-P / PRISMA 2020** | Shamseer L, et al. BMJ 2015;349:g7647；Page MJ, et al. BMJ 2021;372:n1607 | 系統性回顧計畫書與報告規範 |
| **MOOSE** | Brooke BS, et al. JAMA Surg 2021;156(8):787-788 | 觀察性研究之 meta-analysis 報告規範 |
| **GRADE** | Guyatt G, Oxman AD, Aki EA, et al. J Clin Epidemiol 2011;64(4):383-394 | 建議強度與證據品質之透明評估流程 |
| **AAOS Guideline Language** | AAOS Understanding Guideline Language | strong／moderate／limited／consensus 四級建議 |
| **Clinical trial 數量負荷** | Bell RJ, Climacteric 2017;20(1):22-24 | 每年約 250 萬篇新論文問世，無法以閱讀期刊跟上進度 |

### 5.2 骨科專科考試核心總結（Take-Home Points）

1. **證據層級速記**：RCT／RCT 的 SR = Level I → RCT（CI 窄）= I–II → prospective cohort = III → case-control／retrospective cohort／case series = IV → expert opinion = V。Inception cohort 若控制良好且 CDR 驗證可升 Level II。
2. **外科的侷限性要記得**：sham surgery 與 double blinding 難行 → 骨科 RCT 比例低 → 描述性研究常見 → 大型 prospective cohort database 可提供更佳且族群更多元的證據。
3. **PICO → PRISMA-P → PROSPERO → 至少兩個資料庫 → 至少兩位審查者篩選 → 品質評估 → PRISMA/MOOSE → AMSTAR 2**，是系統性回顧的標準骨架。
4. **Fixed-effect 只用於對納入研究本身推論；需外推時用 random-effects**。
5. **建議分四級**：strong、moderate、limited、consensus；strong 需二項以上高層級研究支持，consensus 則在無研究時由專家意見產生。

---

## 參考文獻 (Annotated References)

1. Summary of Report of the Graylyn Development Consensus Conference, November 1998, From Report 13 of the Council on Scientific Affairs (I-99), Update on Clinical Research. http://www.ama-assn.org/ama/pub/article/2036-2392.html. Accessed June 5, 2021.
2. Warth LC, Callaghan JJ, Liu 55, Klaassen AL, Goetz DD, Johnston RC: Thirty-five-year results after Charnley total hip arthroplasty in patients less than fifty years old. A concise follow-up of previous reports. J Bone Joint Surg Am 2014;96(21):1814-1819.
3. Watson Levings RS, Broome TA, Smith AD, et al: Gene therapy for osteoarthritis: Pharmacokinetics of intra-articular self-complementary adeno-associated virus interleukin-1 receptor antagonist delivery in an equine model. Hum Gene Ther Clin Dev 2018;29(2):90-100.
5. Durbin CG Jr: How to read a scientific research paper. Respir Care 2009;54(10):1366-1371.
6. Subramanyam R: Art of reading a journal article: Methodically and effectively. J Oral Maxillofac Pathol 2013;17(1):65-70.
7. Wright JG, Swiontkowski MF, Heckman JD: Introducing levels of evidence to the journal. J Bone Joint Surg 2003;85(1):1-3.
8. Pannucci CJ, Wilkins EG: Identifying and avoiding bias in research. Plast Reconstr Surg 2010;126(2):619-625.
9. Howick J, Chalmers I, Glasziou P, et al: Explanation of the 2011 Oxford Centre for Evidence-Based Medicine (OCEBM) Levels of Evidence (Background Document). Oxford Centre for Evidence-Based Medicine. Accessed June 5, 2021.
10. Bell RJ: What is wrong with the medical literature? Climacteric 2017;20(1):22-24.
11. Shamseer L, Moher D, Clarke M, et al: Preferred reporting items for systematic review and meta-analysis protocols (PRISMA-P) 2015: Elaboration and explanation. BMJ 2015;349:g7647.
12. National Institute for Health Research: PROSPERO: International prospective register of systematic reviews. Available at: https://www.crd.york.ac.uk/PROSPERO/. Accessed June 2, 2022.
13. Sterne JAC, Savovic J, Page MJ, et al: RoB 2: A revised tool for assessing risk of bias in randomised trials. BMJ 2019;366:l4898.
14. Page MJ, Moher D, Bossuyt PM, et al: PRISMA 2020 explanation and elaboration: Updated guidance and exemplars for reporting systematic reviews. BMJ 2021;372:n160.
15. Brooke BS, Schwartz TA, Pawlik TM: MOOSE reporting guidelines for meta-analyses of observational studies. JAMA Surg 2021;156(8):787-788.
16. Shea BJ, Grimshaw JM, Wells GA, et al: Development of AMSTAR: A measurement tool to assess the methodological quality of systematic reviews. BMC Med Res Methodol 2007;7:10.
17. Shea BJ, Reeves BC, Wells G, et al: AMSTAR 2: A critical appraisal tool for systematic reviews that include randomised or non-randomised studies of healthcare interventions, or both. BMJ 2017;358:j4008.
18. Institute of Medicine: Clinical Practice Guidelines We Can Trust. The National Academies Press, 2011.
19. The American Academy of Orthopaedic Surgeons: Understanding Guideline Language. Available at: https://www.orthoguidelines.org/definitions. Accessed March 15, 2022.
20. GRADE series in the Journal of Clinical Epidemiology. Available at: https://www.jclinepi.com/content/jce-GRADE-Series. Accessed June 5, 2021.
21. Moher D, Moher E: Stop predatory publishers now: Act collaboratively. Ann Intern Med 2016;164(9):616-617.

## Summary

- **證據層級速記**：RCT／RCT 的 SR = Level I → RCT（CI 窄）= I–II → prospective cohort = III → case-control／retrospective cohort／case series = IV → expert opinion = V。Inception cohort 若控制良好且 CDR 驗證可升 Level II。
- **外科的侷限性**：sham surgery 與 double blinding 難行 → 骨科 RCT 比例低 → 描述性研究常見 → 大型 prospective cohort database 可提供更佳且族群更多元的證據。
- **系統性回顧標準骨架**：PICO → PRISMA-P → PROSPERO → 至少兩個資料庫 → 至少兩位審查者篩選 → 品質評估 → PRISMA/MOOSE → AMSTAR 2。
- **統計模型選擇**：<span style="color:#60a5fa">Fixed-effect</span> 只用於對納入研究本身推論；需外推至更廣族群時用 <span style="color:#60a5fa">random-effects</span>，並做 multiway sensitivity analyses。
- **建議分四級**：strong、moderate、limited、consensus；strong 需二項以上高層級研究支持，consensus 則在無研究可用時由專家意見產生。
- **常見誤讀**：把觀察性關聯當成因果、忽略 case-control 的單一 outcome 限制與 recall bias、錯用 fixed-effect 做外推、將 systematic review 一律視為高品質、未察覺 predatory publishing。
