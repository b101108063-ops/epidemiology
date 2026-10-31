---
title: "Chapter 20: Inflammation and Immunology (發炎與免疫學): 先天與適應性免疫、生物製劑與疫苗"
date: 2026-10-31
draft: false
tags: ["Orthopaedics", "OKU14", "Immunology", "Inflammation", "Biologics"]
categories: ["General Topics"]
weight: 20
summary: "本章以骨科視角串連發炎與免疫學：先鋸 Toll-like receptor（TLR）訊息傳遞如何啟動促發炎細胞激素，再延伸到適應性免疫（MHC I／II 呈現、Th1／Th2、兩訊號假說與免疫檢查點），並以生物製劑（anti-TNF、IL-1／IL-6 抑制劑、JAK 抑制劑）、CAR-T 細胞療法與主動／被動免疫策略之臨床決策作結。"
---

# Chapter 20: Inflammation and Immunology — 發炎與免疫學

**章節導讀**：發炎是所有骨科疾病與手術的核心，範圍與持續時間決定組織癒合潛能與病理變化。本章由 TLR 訊息傳遞出發，依序闡述適應性免疫與免疫耐受、免疫檢查點與腫瘤免疫治療、疫苗平台與 COVID-19 的教訓，最後落到骨科常用的生物製劑與手術前停藥決策，是骨科醫師面對發炎性關節病、假體周圍骨溶解與感染時的免疫學基礎。

---

## 1. 核心概念：先天免疫與 TLR 訊息傳遞 (Innate Immunity & TLR Signaling)

### 1.1 發炎如何被啟動：PAMP 與 DAMP

<span style="color:#e2e8f0">Pathogen-associated molecular patterns（PAMP）</span> 指微生物產生、真核細胞無法自行合成的分子；<span style="color:#e2e8f0">Damage-associated molecular patterns（DAMP）</span> 則是壞死宿主細胞釋出的細胞內生化物質。兩者都是 <span style="color:#22d3ee">Toll-like receptor（TLR）</span> 的配體。

| 配體類別 | 代表分子 | 來源 |
|----------|----------|------|
| <span style="color:#c084fc">PAMP</span> | Peptidoglycan | 革蘭氏陽性菌 |
| | Lipoteichoic acid | 革蘭氏陽性菌（原文此處誤植為 gram-negative） |
| | Lipoproteins、Lipoarabinomannan | 分枝桿菌（Mycobacteria） |
| | LPS（lipopolysaccharide） | 革蘭氏陰性菌 |
| | Zymosan | 酵母菌（yeast） |
| | Profilin-like protein | 弓形蟲（Toxoplasma gondii） |
| <span style="color:#f87171">DAMP／內源性配體</span> | Uric acid crystals（尿酸鹽晶體） | 可活化 TLR，導致發炎性關節病（gout） |

> **Pearl**：尿酸鹽晶體屬於「內源性配體」也能活化 TLR，這正是痛風不單純是代謝疾病、而是免疫發炎疾病的免疫學基礎。

### 1.2 TLR 訊息傳遞路徑

- **啟動位置**：TLR 訊息傳遞可在細胞膜上，也可在細胞內區室（intracellular compartments）進行。
- **共同刺激分子（accessory molecules）**：<span style="color:#22d3ee">CD14、MD2、CD36</span> 可直接或與配體協同促進 TLR 二聚化。
- **接合蛋白（adaptors）**：<span style="color:#e2e8f0">MYD88</span>（myeloid differentiation factor 88）、<span style="color:#e2e8f0">TRIF</span>（Toll/IL-1R domain-containing adaptor-inducing interferon beta）、<span style="color:#e2e8f0">TIRAP</span>（Toll/interleukin-1 receptor domain-containing adaptor protein）、<span style="color:#e2e8f0">TRAM</span>（TRIF-related adaptor molecule）。
- **核內轉錄因子**：<span style="color:#60a5fa">NF-κB（nuclear factor kappa B）、IRF（interferon regulatory factors）、MAPK</span> 活化，導致促發炎細胞激素（proinflammatory cytokines）與趨化因子（chemokines）合成，啟動組織發炎。

<!-- FIG: 圖 1　Toll-like receptor（TLR）訊息傳遞示意（PAMP／DAMP → TLR → MYD88／TRIF → NF-κB、IRF、MAPK） -->
![圖 1　Toll-like receptor（TLR）訊息傳遞示意（PAMP／DAMP → TLR → MYD88／TRIF → NF-κB、IRF、MAPK）](/images/oku14/ch20_p0253_fig1.jpg)
*圖 1　Toll-like receptor（TLR）訊息傳遞示意（PAMP／DAMP → TLR → MYD88／TRIF → NF-κB、IRF、MAPK）*
> **Pearl**：TLR 訊息傳遞是「發炎」的總開關——不論病原體入侵或細胞壞死，最後都收斂到 NF-κB／IRF 這條共同下游路徑。

### 1.3 促發炎細胞激素的訊息傳遞與生物製劑介入點

<!-- FIG: 圖 2 — Illustration of proinflammatory cytokine signaling and biologic therap -->
![圖 2 — Illustration of proinflammatory cytokine signaling and biologic therap](/images/oku14/ch20_p0254_fig2.jpg)
*圖 2 — Illustration of proinflammatory cytokine signaling and biologic therap*
TNF 位於促發炎級聯的頂端（apex），經由 TNF 受體相關因子（TRAF）活化 NF-κB，並透過 TNF 受體相關死亡區域蛋白（TRADD）啟動細胞凋亡程式。Interferon 與 interleukin 則經由 <span style="color:#fbbf24">JAK（Janus kinase）／STAT（signal transducer and activator of transcription）</span> 蛋白傳遞訊息；此等路徑在類風濕性關節炎（RA）、乾癬性關節炎與強直性脊椎炎中同樣過度活化。

| 治療類別 | 代表藥物 | 標的 |
|----------|----------|------|
| <span style="color:#60a5fa">Anti-TNF 生物製劑</span> | Infliximab、Adalimumab、Golimumab、Certolizumab pegol、Etanercept | TNF |
| <span style="color:#60a5fa">抗發炎小分子</span> | <span style="color:#fb923c">Tofacitinib</span> 等 JAK 抑制劑 | JAK／STAT 訊息傳遞 |
| <span style="color:#60a5fa">細胞激素／受體標的</span> | Ustekinumab（抗 IL-12／IL-23）、Tocilizumab（抗 IL-6 受體）、Anakinra（抗 IL-1 受體） | 下游細胞激素 |
| <span style="color:#60a5fa">骨代謝標的</span> | Denosumab（RANKL）、Teriparatide、BMP-2 | RANKL／骨代謝軸 |
| <span style="color:#60a5fa">上游 B 細胞路徑</span> | 針對 APRIL、BAFF、BAFF-R 的製劑 | B 細胞活化 |


> **Pearl**：生物製劑可用於「gain-of-function」與「loss-of-function」研究；今日許多人類免疫學知識，正是來自這些生物製劑的臨床試驗。

### 1.4 生物製劑在類風濕性關節炎的三項重大限制

1. **FDA 核准門檻極低**：RA 藥物核准的效應標準僅為美國風濕病學會準則的 <span style="color:#f87171">ACR20（即改善 20%）</span>。
2. **本質上具免疫抑制性**：所有這些生物製劑皆為免疫抑制劑，因此<span style="color:#f87171">不可併用</span>，已知會增加伺機性感染（opportunistic infection）風險。
3. **術前停藥建議**：選擇性手術前建議「生物製劑假期（biologic therapy holiday）」，例如 <span style="color:#fbbf24">全關節置換術前 2～4 週停止 anti-TNF 治療</span>。

> **Danger zone**：RA 是最常見的免疫介導發炎疾病——成人盛行率 0.5%～1%，55 歲以上族群達 4.5%，每年每 10 萬人新增 5～50 例；且目前<b>沒有治癒方法</b>，這也是多數 FDA 核准生物製劑的第一適應症來源。

<!-- FIG: 圖 3　類風濕性關節炎之生物製劑治療標的示意（細胞激素、受體、特定細胞類型） -->
![圖 3　類風濕性關節炎之生物製劑治療標的示意（細胞激素、受體、特定細胞類型）](/images/oku14/ch20_p0257_fig3.jpg)
*圖 3　類風濕性關節炎之生物製劑治療標的示意（細胞激素、受體、特定細胞類型）*
---

## 2. 骨科疾病中的發炎性與免疫性疾病 (Inflammatory & Immunologic Disorders)

### 2.1 主要疾病之人口學、解剖位置與致病機轉

下表整理骨科常見的發炎性與免疫性疾病；所有數值與描述均依原文 Table 1。

| 疾病 | 人口學 | 常见解剖位置 | 已知致病機轉 |
|------|--------|----------------|--------------|
| <span style="color:#60a5fa">類風濕性關節炎</span> | 女性 > 男性；30～50 歲最常見，任何年齡皆可能 | 小關節（手、足）最常見；大關節與頸椎亦受累 | 具滑膜發炎的自體免疫疾病；B 細胞、T 細胞、巨噬細胞皆參與。全身表現含血管炎、心包炎、Felty 症候群（脾大與白血球減少）、Still 疾病、類風濕結節 |
| <span style="color:#60a5fa">強直性脊椎炎</span> | 男性 > 女性；20～40 歲，任何年齡皆可能；HLA-B27 帶因者較常見 | 骶髂關節與脊柱 | 具 enthesitis 的自體免疫疾病。全身表現含葡萄膜炎與虹膜炎、胃腸道發炎、肺纖維化、腎澱粉樣變性、主動脈炎 |
| <span style="color:#60a5fa">全身性紅斑性狼瘡</span> | 女性 >> 男性；15～44 歲最常見 | 全身性，多器官受累 | 診斷為排除式；準則與致病機轉均含自體抗體（ANA、anti-dsDNA、anti-Smith、antiphospholipid）。表現含皮膚、黏膜、漿膜炎、腎臟、神經與血液疾病 |
| <span style="color:#60a5fa">幼年型特發性關節炎</span> | 16 歲以下，症狀至少 6 週，病因不明 | 滑膜炎，但侵蝕性破壞較 RA 少 | 自體免疫疾病：遺傳易感性、體液免疫與自體抗體產生，合併環境因子。骨壞死是關節疼痛常見原因。分全身型、多關節型（≥5 關節）、寡關節型（<5 關節） |
| <span style="color:#60a5fa">乾癬性關節炎</span> | 20%～30% 乾癱患者可能合併；男性 = 女性；30～40 歲最常見 | Enthesitis 與遠端指間關節受累常見；大關節與脊柱亦可受累（多為寡關節型）。皮膚病通常先於關節病但非一定 | 自體免疫疾病：遺傳易感性與環境因子交互作用。皮節型（arthritis mutilans）為手足最常見的嚴重破壞性畸形 |
| <span style="color:#60a5fa">肌炎</span> | 男性 = 女性；30～40 歲最常見；差異取決於診斷（皮肌炎、多發性肌炎、包涵體肌炎） | 部分侵犯近端肌群（多發性肌炎），部分以遠端為主（包涵體肌炎） | CD8+ T 細胞扮演重要角色；遺傳易感性、先天與適應性免疫、環境因子交互作用。常見疲勞、肌無力或疼痛；可為急性與慢性表現 |
| <span style="color:#60a5fa">痛風與偽痛風</span> | 痛風：男性 > 女性；30～60 歲最常見，女性多為停經後。偽痛風多為年長者 | 痛風：下肢 > 上肢；第一蹠趾關節最常見，亦可見蹠骨、踝、膝、腕、掌指關節。偽痛風：關節置換部位周圍最常見 | 痛風＝高尿酸血症＋單尿酸鈉結晶；偽痛風＝軟骨表面焦磷酸鈣二水合物結晶。結晶誘發局部發炎細胞激素釋放，造成軟骨損傷與骨侵蝕 |
| <span style="color:#60a5fa">生物材料異物反應</span> | 無年齡或性別易感性 | 假體置換部位之關節周圍最常見 | 任何常用生物材料皆可引發（最常見聚乙烯、金屬腐蝕產物、骨水泥微粒）。磨損微粒刺激吞噬細胞釋放發炎細胞激素造成骨溶解 |

> **Pearl**：<span style="color:#fbbf24">Enthesitis（肌腱與骨交界處的發炎）</span> 是強直性脊椎炎與乾癱性關節炎共同的特徵性所在；反覆的 enthesitis 可導致骨化與脊椎「竹節樣」改變。

> **Danger zone**：骨溶解（osteolysis）常被歸因於「機械性磨損」，但其機轉其實是免疫發炎——磨損微粒活化吞噬細胞釋放發炎細胞激素而造成骨吸收，這也是 periprosthetic osteolysis 需以抗發炎策略介入的理由。

---

## 3. 適應性免疫與免疫檢查點：治療決策的免疫學基礎 (Adaptive Immunity, Tolerance & Checkpoints)

### 3.1 兩大平行分支：細胞性與體液性免疫

<span style="color:#e2e8f0">Adaptive immunity（適應性免疫）</span> 是长寿生物體對特定外來分子（抗原，antigens）演化出的複雜反應，涉及大量可溶性因子與細胞在數週至數月的長時間交互作用。

| 分支 | 目標 | 關鍵細胞／分子 |
|------|------|----------------|
| <span style="color:#60a5fa">細胞性免疫</span> | 產生抗原專一性細胞毒性 T 淋巴球（CTL），殺死表現該抗原的宿主細胞 | Th1、CTL、TCR、MHC I |
| <span style="color:#60a5fa">體液性免疫</span> | 產生抗原專一性中和性抗體，使危險分子（如可溶性毒素、棘蛋白）失活，並經 opsonophagocytosis 促進清除 | Th2、B 細胞、BCR、血漿細胞、IgG |

### 3.2 抗原呈現與 T 細胞活化

1. **樹突細胞（dendritic cells）** 產生胜肽抗原。
2. **MHC I 路徑（內源性）**：APC 自身新合成的蛋白由 <span style="color:#22d3ee">proteasome</span> 切成胜肽 → 運至內質網由胺肽酶再修飾 → 載 onto MHC I。MHC I 幾乎表現於所有人類細胞上，刺激 <span style="color:#22d3ee">CD8+ T 細胞</span>。
3. **MHC II 路徑（外源性）**：專業 APC 攝取外源性蛋白 → 溶酶體內蛋白水解 → 載入新合成的 MHC II → 運送至細胞膜，刺激 <span style="color:#22d3ee">CD4+ 輔助 T 細胞（Th）</span>。
4. **Th 分化**：TCR 辨識 MHC II 上的胜肽後，Th 依細胞激素環境分化為支持細胞性免疫的 <span style="color:#fb923c">Th1</span>（interferon gamma、TNF、IL-2）或支持體液性免疫的 <span style="color:#fb923c">Th2</span>（IL-4、IL-5、IL-13）。
5. **下游效應**：Th1 促進 CTL 增殖與活化（CTL 亦需 APC 上 MHC I 的胜肽刺激）；Th2 促進 B 細胞增殖與活化（B 細胞亦需 BCR 辨識游離或細胞結合的抗原）。B 細胞分化為血漿細胞時，免疫球蛋白重鏈基因重組將膜上抗原專一性 BCR（IgM）轉為可溶性 IgG 分泌入血。

> **Pearl**：保護性免疫反應中，辨識同一抗原的 Th1、Th2、CTL 與 B 細胞在感染部位協同清除病原體，之後在缺乏抗原刺激時經凋亡（apoptosis）死亡；未參與感染的前驅細胞則遷居骨髓，成為終身記憶細胞，可在再感染時釋出。

> **Danger zone**：免疫記憶的「歸巢（homing）」特性是疫苗與 CAR-T 療效持久的關鍵——CAR-T 的記憶細胞可自行回到骨髓並在復發時自行反應。

<!-- FIG: 圖 4　內源性（MHC I → CD8+ T 細胞）與外源性（MHC II → 輔助 T 細胞）抗原呈現路徑對照 -->
![圖 4　內源性（MHC I → CD8+ T 細胞）與外源性（MHC II → 輔助 T 細胞）抗原呈現路徑對照](/images/oku14/ch20_p0259_fig4.jpg)
*圖 4　內源性（MHC I → CD8+ T 細胞）與外源性（MHC II → 輔助 T 細胞）抗原呈現路徑對照*
### 3.3 免疫耐受與自體免疫：兩訊號假說

- <span style="color:#e2e8f0">Central tolerance（中央耐受）</span>：骨髓的 B 細胞 clonal deletion 與胸腺的 T 細胞 negative selection，在造血發育中清除自體反應性淋巴球。
- **逃逸比例**：約 <span style="color:#f87171">10% 的 B 細胞與 T 細胞逃逸</span>，須靠周邊耐受約束。
- **兩訊號假說（two-signal hypothesis）**：B 細胞與 T 細胞只有在抗原專一性 BCR／TCR 訊號之外**還有第二訊號**時才能反應；缺乏時會凋亡或進入長期無反應狀態（<span style="color:#e2e8f0">anergy</span>）。
- **最常用的第二訊號**：<span style="color:#22d3ee">CD40L 刺激 B 細胞上的 CD40</span>；<span style="color:#22d3ee">B7（CD80／CD86）刺激 T 細胞上的 CD28</span>。
- **抑制機制**：<span style="color:#60a5fa">CTLA-4</span> 與 APC 上的 B7 配體結合，可阻斷 T 細胞 CD28 的共同刺激訊號。
- **人類突變的證據**：<span style="color:#f87171">X-linked agammaglobulinemia／hyper-IgM syndrome</span> 患者遺傳性缺乏 CD40L；<span style="color:#f87171">CTLA-4 基因的多型性</span> 與實體器官移植排斥風險相關。
- **Horror autotoxicus**：1892 年證明母體抗體可被動轉移給胎兒後，隨即有實驗顯示異種與同種異體血注入動物可產生溶血性抗體，因而提出自體免疫假說。

> **Pearl**：<span style="color:#fbbf24">腫瘤免疫學與自體免疫是同一套機制的兩面</span>——檢查點（CTLA-4、PD-1／PD-L1）被抑制以提升抗腫瘤 T 細胞活性時，自體反應性 T 細胞也會被活化，可能誘發 1 型糖尿病等 immune-related adverse events。

### 3.4 骨科醫師需關心的腫瘤免疫治療

| 治療 | 機轉 | 代表藥物 |
|------|------|----------|
| <span style="color:#60a5fa">CTLA-4 抑制劑</span> | 結合 CTLA-4，允許 CD28／B7 持續共同刺激與 T 細胞活化 | <span style="color:#fb923c">Ipilimumab</span> |
| <span style="color:#60a5fa">PD-1 抑制劑</span> | 結合 PD-1，使負向訊號失效 | <span style="color:#fb923c">Pembrolizumab</span>、<span style="color:#fb923c">Nivolumab</span> |
| <span style="color:#60a5fa">PD-L1 抑制劑</span> | 阻斷 PD-L1 | <span style="color:#fb923c">Atezolizumab</span> |
| <span style="color:#60a5fa">CAR-T 細胞療法</span> | 重新編程患者 T 細胞以辨識並殺死表現特定表面受體的細胞 | <span style="color:#fb923c">Tisagenlecleucel</span>（CD19） |

- **CAR 結構**：胞外功能域 FMC63（單株抗體衍生的 single-chain variable fragment，辨識 CD19）＋ CD8 跨膜區（signal 1 由 CD3 zeta 傳遞）＋ 4-1BB（CD137）共同刺激區（signal 2）。
- **CAR-T 治療流程**：採集白血球 → 製造中心活化並轉染 CAR 基因 → 擴增 → 回輸 → **淋巴清除化學治療（lymphodepleting chemotherapy）** → 輸注 CAR-T 細胞。
- **Coley toxin 的歷史意義**：骨科腫瘤科曾報告慢性骨髓炎合併終末期轉移性癌症患者在抑制性抗生素治療下存活遠超預後；其機轉現今被理解為 PAMP–TLR 訊息使 CTLA-4、PD-1／PD-L1 下調。

> **Danger zone**：<span style="color:#f87171">免疫檢查點抑制劑只應用於無其他治療可選的轉移性癌症患者</span>，因可造成嚴重免疫相關不良事件。

> **Pearl**：CAR-T 相較放射、化學治療與生物製劑的優勢，在於**單次給藥即設計為終身有效**（記憶型 CAR-T 可歸巢並存留於骨髓，在復發時自行反應）；但 lymphodepletion 與自體免疫相關的嚴重不良事件不可輕忽。

<!-- FIG: 圖 5　免疫檢查點抑制劑（CTLA-4、PD-1／PD-L1）與抗體拮抗劑 -->
![圖 5　免疫檢查點抑制劑（CTLA-4、PD-1／PD-L1）與抗體拮抗劑](/images/oku14/ch20_p0260_fig5.jpg)
*圖 5　免疫檢查點抑制劑（CTLA-4、PD-1／PD-L1）與抗體拮抗劑*
<!-- FIG: 圖 6　CAR-T 細胞療法之結構與治療流程 -->
![圖 6　CAR-T 細胞療法之結構與治療流程](/images/oku14/ch20_p0261_fig6.jpg)
*圖 6　CAR-T 細胞療法之結構與治療流程*
---

## 4. 疫苗、感染防治與骨科決策的陷阱與爭議 (Vaccination, Infection & Pitfalls)

### 4.1 三種免疫形式

| 形式 | 定義 | 臨床意義 |
|------|------|----------|
| <span style="color:#60a5fa">自然免疫（Natural immunity）</span> | 宿主自病源性挑戰後恢復而獲得 | 了解最薄弱，因個體間適應性免疫反應差異極大。主因是 MHC 基因高度多型性，使同種族群成員在自然感染時呈現不同抗原，提高部分個體獲得保護性免疫的機率。**Herd immunity（群體免疫）**的免疫型別與閾值（族群 60%～90%）則不明確 |
| <span style="color:#60a5fa">主動免疫（Active immunization）</span> | 以病原體或毒素的抗原接種宿主 | 兩大成分：**佐劑**（如刺激 TLR 的 PAMP 與 DAMP，可上調 APC 的抗原呈現與第二訊號，同時下調檢查點抑制劑）＋ **抗原**。效力取決於宿主免疫反應，可從終身保護到完全測不出，且不能用於治療 |
| <span style="color:#60a5fa">被動免疫（Passive immunization）</span> | 由乳汁或藥物輸注將中和性抗體轉移給宿主 | 抗體立即生效但半衰期有限（約 3～4 個月），主要作為治療使用 |

### 4.2 主動免疫的六種疫苗平台

<!-- FIG: 圖 8 — Illustration of different types of vectors for active immunization. Si -->
![圖 8 — Illustration of different types of vectors for active immunization. Si](/images/oku14/ch20_p0263_fig8.jpg)
*圖 8 — Illustration of different types of vectors for active immunization. Si*
| 平台 | 原理 | 目前核准的人用疫苗 | 現況 |
|------|------|----------------------|------|
| <span style="color:#60a5fa">RNA</span> | 編碼棘蛋白的 RNA 被宿主細胞攝入並轉譯，誘發免疫反應 | — | 尚無核准人用疫苗；但 mRNA 疫苗（BNT162b2、mRNA-1273）效力最優 |
| <span style="color:#60a5fa">DNA</span> | 編碼棘蛋白的 DNA 被攝入、轉錄，再轉譯 mRNA | — | 尚無核准人用疫苗 |
| <span style="color:#60a5fa">Protein（蛋白質）</span> | 以酵母菌或 baculovirus 表現系統製造蛋白抗原，注射（通常佐以佐劑） | HPV、Hepatitis B virus、Influenza | 尚未使用此平台 |
| <span style="color:#60a5fa">Viral vectors（病毒載體）</span> | 病毒（如腺病毒）進入宿主細胞轉錄抗原，病毒本身亦具佐劑作用 | Ebolavirus vaccine（VSV vector） | 尚未使用此平台 |
| <span style="color:#60a5fa">Inactivated（不活化）</span> | 殺死的病毒作為免疫原注射，可搭配佐劑 | Influenza、Polio、Hepatitis A | — |
| <span style="color:#60a5fa">Live attenuated（活性減毒）</span> | 減毒病毒誘發強烈抗病毒免疫反應 | MMR、Chickenpox、Yellow fever | — |

- **歷史第一個科學化主動疫苗嘗試**：<span style="color:#fbbf24">1796 年</span> 首次報導以刻意主動接種控制感染性疾病。
- **COVID-19 疫苗效力差異**：複製缺陷型重組腺病毒載體疫苗（Ad26.COV2.S，Janssen／Johnson & Johnson／AstraZeneca-Oxford AZD1222）效力較 mRNA 疫苗有限，部分原因可能與宿主對載體的免疫反應有關，而此反應已知會限制追加劑（boosters）。
- **成本效益**：COVID-19 疫苗每劑約 <span style="color:#34d399">US$20</span>；主動免疫優勢為可將細胞性與體液性適應性反應聚焦於特定抗原。

### 4.3 抗體依賴性感染增強（ADE）與細胞激素風暴

<!-- FIG: 圖 7　中和性抗體與非中和性抗體、抗原漂移與 ADE、細胞激素風暴 -->
![圖 7　中和性抗體與非中和性抗體、抗原漂移與 ADE、細胞激素風暴](/images/oku14/ch20_p0262_fig7.jpg)
*圖 7　中和性抗體與非中和性抗體、抗原漂移與 ADE、細胞激素風暴*
- **保護性免疫**：特定中和性抗體透過 (1) 抑制病毒附著宿主細胞（COVID-19 中棘蛋白無法結合 ACE2）與 (2) opsonophagocytosis（抗體結合病毒，經 CD32 即 FcγRII 受體介導內吞，於溶酶體內立即破壞）兩種機制清除病毒。
- <span style="color:#f87171">ADE</span>：病毒抗原突變後，既往暴露或接種所產生的抗體與病毒形成不完美複合體；此不穩定複合體與免疫細胞的 FcγRII 受體結合後，病毒可在與溶酶體融合前逃出內體，開始毒性複製週期。
- **細胞激素風暴**：大量病毒複製產生大量 PAMP，加上感染壞死細胞釋出 DAMP，可同時大規模活化先天與適應性免疫，造成表現為 SARS、敗血性休克或猝死的細胞激素風暴。

> **Pearl（看似反直覺的處置）**：嚴重病毒感染病人會被給予<b>免疫抑制治療</b>（如 corticosteroids）以<b>預防</b>細胞激素風暴——與「感染要加強免疫」的直覺相反。

### 4.4 被動免疫的現代角色：REGEN-COV 與骨科感染

- **REGEN-COV**：COVID-19 被動免疫製劑，由兩種重組人源單株抗體 <span style="color:#fb923c">casirivimab</span> 與 <span style="color:#fb923c">imdevimab</span> 組成之雞尾酒，標的為 SARS-CoV-2 棘蛋白。
- **適應症**：主要用於嚴重感染者；亦獲 FDA 核准用於未接種疫苗者，或因暴露於 COVID-19 而有重症高風險的免疫功能低下者。
- **骨科抗微生物治療的困境**：手術部位感染（SSI）仍是骨科手術的重大併發症；人工關節感染性骨髓炎（implant-associated osteomyelitis）的現有治療**50 年來成果幾乎未變**；抗藥性且高毒力的菌株持續威脅現行治療典範。

> **Danger zone**：免疫功能低下者無法有效接受主動疫苗接種，因此被動免疫（恢復期血清或單株抗體）是其重要防線；臨床醫師在骨科術前評估時應主動確認病人的疫苗與免疫狀態。

> **Pearl**：COVID-19 疫情提供了當代證據，說明人類對微生物致病性的易感性，以及「保護性 vs. 非保護性抗體介導免疫」與「如何達成保護性免疫」之間仍存在巨大的知識落差（knowledge gap）。

---

## 5. 實證更新與 OKU 14 重點 (Recent Evidence & Take-Home Points)

### 5.1 OKU 14 強調之核心概念

| 主題 | 來源 | 要點 |
|------|------|------|
| <span style="color:#60a5fa">TLR 訊息傳遞</span> | Rakoff-Nahoum S, Medzhitov R: Nat Rev Cancer 2009;9(1):57-63；Liu-Bryan R, et al: Arthritis Rheum 2005;52(9):2936-2946 | TLR2 與 TLR4 及 MYD88 對單尿酸鈉結晶誘發的發炎具關鍵性 |
| <span style="color:#60a5fa">NF-κB 家族</span> | Verma IM, et al: Genes Dev 1995;9(22):2723-2735 | Rel／NF-κB／I kappa B 家族之關聯與解離 |
| <span style="color:#60a5fa">發炎與其消退</span> | Gallo J, Raska M, Kriegova E, Goodman SB: J Orthop Translat 2017;10:52-67 | 對肌肉骨骼系統的影響 |
| <span style="color:#60a5fa">敗血症與無菌性骨溶解</span> | Pajarinen J, et al: J Long Term Eff Med Implants 2014;24(4):283-296 | 髖關節假體周圍的先天免疫反應 |
| <span style="color:#60a5fa">慢性反覆多灶性骨髓炎</span> | Ferguson PJ, Sandu M: Curr Rheumatol Rep 2012;14(2):130-141 | 致病機轉與處理的最新理解 |
| <span style="color:#60a5fa">IMIDs 與生物製劑</span> | Kuek A, Hazleman BL, Ostor AJ: Postgrad Med J 2007;83(978):251-260 | 稱為「醫學革命」 |
| <span style="color:#60a5fa">M1／M2 巨噬細胞活化</span> | Martinez FO, Gordon S: F1000Prime Rep 2014;6:13 | 重新評估之必要性 |
| <span style="color:#60a5fa">死亡受體訊息傳遞</span> | Fas SC, et al: Curr Dir Autoimmun 2006;9:1-17 | 死亡受體訊息傳遞及其免疫功能 |

### 5.2 生物製劑與手術的實務要點

| 臨床情境 | 原文建議／數據 |
|----------|----------------|
| 類風濕性關節炎患者之生物製劑 | 核准門檻僅為 ACR20；所有生物製劑皆具免疫抑制性，<span style="color:#f87171">不可併用</span> |
| 選擇性手術前 | 建議生物製劑假期：<span style="color:#fbbf24">全關節置換術前 2～4 週停止 anti-TNF</span> |
| 免疫相關疾病之生物製劑使用與術前處置 | 依現有指引，生物製劑之使用與術前管理之共識性建議（Level of evidence: V） |
| Etanercept + anakinra 併用於 RA | 與 MTX 治療失敗者之併用治療研究（Arthritis Rheum 2004;50(5):1412-1419） |

> **Pearl**：面對使用生物製劑的患者，應主動確認**感染風險、停藥時程、停藥期間疾病是否復發**，並與風濕科／內科共同決策。

### 5.3 骨科專科考試核心總結（Take-Home Points）

1. **發炎啟動**：PAMP 與 DAMP 活化 TLR，經訊息傳遞促進促發炎細胞激素與趨化因子合成；尿酸鹽晶體等內源性配體亦可活化 TLR 而導致痛風。
2. **TLR 下游**：TLR 二聚化後經 MYD88、TRIF、TIRAP、TRAM 啟動 NF-κB、IRF 與 MAPK；TNF 位於級聯頂端，經 TRAF／TRADD 作用於 NF-κB 與凋亡；interferon 與 interleukin 走 JAK／STAT。
3. **生物製劑現況**：針對促發炎訊息的小分子（JAK 抑制劑）與生物製劑（anti-TNF 等）已是發炎性骨科疾病的標準治療（standard-of-care）；因其免疫抑制性不可併用，會導致伺機性感染。
4. **發炎的臨床後果**：促發炎細胞激素（TNF、IL-1、IL-6）長期表現，源自先天疾病、自體免疫、感染與植入物磨損碎屑，造成發炎侵蝕性關節炎與骨溶解。
5. **終身免疫與檢查點**：對病原體與癌細胞的終身後天免疫，需要下調阻礙 T 細胞活化與增殖的免疫檢查點（PD-L1 與 PD-1）。其生物製劑拮抗劑已證實可有效治療無法治癒的癌症，但也可能造成免疫相關不良事件（如 1 型糖尿病）。
6. **主動 vs. 被動免疫**：主動疫苗效力取決於宿主能否產生抗原專一性 T 細胞與中和性抗體；被動免疫直接提供恢復期血清或單株抗體中的中和性抗體。
7. **關節炎與骨溶解**：痛風與偽痛風皆以結晶誘發局部發炎細胞激素釋放為致病機轉；生物材料異物反應以磨損微粒刺激吞噬細胞釋放發炎細胞激素造成骨溶解。

---

## 參考文獻


9. Gallo J, Raska M, Kriegova E, Goodman SB: Inflammation and its resolution and the musculoskeletal system. J Orthop Transl 2017;10:52-67.
10. Pajarinen J, Jamsen E, Konttinen YT, Goodman SB: Innate immune reactions in septic and aseptic osteolysis around hip implants. J Long Term Eff Med Implants 2014;24(4):283-296.
11. Ferguson PJ, Sandu M: Current understanding of the pathogenesis and management of chronic recurrent multifocal osteomyelitis. Curr Rheumatol Rep 2012;14(2):130-141.
12. Kuek A, Hazleman BL, Ostor AJ: Immune-mediated inflammatory diseases (IMIDs) and biologic therapy: A medical revolution. Postgrad Med J 2007;83(978):251-260.
13. Her M, Kavanaugh A: Alterations in immune function with biologic therapies for autoimmune disease. J Allergy Clin Immunol 2016;137(1):19-27.
14. Scott DL, Wolfe K, Huizinga TW: Rheumatoid arthritis. Lancet 2010;376(9746):1094-1108.
15. Felson DT, Anderson JJ, Boers M, et al: American College of Rheumatology. Preliminary definition of improvement in rheumatoid arthritis. Arthritis Rheum 1995;38(6):727-735.
16. Genovese MC, Cohen S, Moreland L, et al: Combination therapy with etanercept and anakinra in the treatment of patients with rheumatoid arthritis who have been treated unsuccessfully with methotrexate. Arthritis Rheum 2004;50(5):1412-1419.
17. Rezaieyazdi Z, Sahebari M, Khodashahi M: Preoperative evaluation and management of patients receiving biologic therapies. Arch Bone Jt Surg 2019;7(3):220-228.
18. Neerincx A, Castro W, Guarda G, Kufer TA: NLRCS, at the heart of antigen presentation. Front Immunol 2013;4:397.
19. Silverstein AM: Autoimmunity versus horror autotoxicus: The struggle for recognition. Nat Immunol 2001;2(4):279-281.
20. Wang Q, Shangguan J, Zhang Y, Pan Y, Yuan Y, Que W: The prevalence of thyroid autoantibodies in autoimmune connective tissue diseases: A systematic review and meta-analysis. Expert Rev Clin Immunol 2020;16(9):923-930.

1. Garcia MA, Meurs EK, Esteban M: The dsRNA protein kinase PKR: Virus and cell control. Biochimie 2007;89(6-7):799-811.
2. Medzhitov R, Janeway C Jr: Innate immunity. N Engl J Med 2000;343(5):338-344.
3. Rakoff-Nahoum S, Medzhitov R: Toll-like receptors and cancer. Nat Rev Cancer 2009;9(1):57-63.
4. Liu-Bryan R, Scott P, Sydlaske A, Rose DM, Terkeltaub R: Innate immunity conferred by Toll-like receptors 2 and 4 and myeloid differentiation factor 88 expression is pivotal to monosodium urate monohydrate crystal-induced inflammation. Arthritis Rheum 2005;52(9):2936-2946.
5. Verma IM, Stevenson JK, Schwarz EM, Van Antwerp D, Miyamoto S: Rel/NF-kappa B/I kappa B family: Intimate tales of association and dissociation. Genes Dev 1995;9(22):2723-2735.
6. Pedersen J, Coskun M, Soendergaard C, Salem M, Nielsen OH: Inflammatory pathways of importance for management of inflammatory bowel disease. World J Gastroenterol 2014;20(1):64-77.
7. Fas SC, Fritzsching B, Suri-Payer E, Krammer PH: Death receptor signaling and its function in the immune system. Curr Dir Autoimmun 2006;9:1-17.
8. Martinez FO, Gordon S: The M1 and M2 paradigm of macrophage activation: Time for reassessment. F1000Prime Rep 2014;6:13.

## Summary

- **發炎啟動與 TLR**：PAMP（peptidoglycan、LPS、lipoarabinomannan、zymosan）與 DAMP（如尿酸鹽晶體）活化 TLR，經 MYD88／TRIF／TIRAP／TRAM 傳遞，啟動 NF-κB、IRF、MAPK，促進促發炎細胞激素與趨化因子合成。
- **TNF 為級聯頂端**：TNF 經 TRAF 活化 NF-κB，經 TRADD 啟動凋亡；interferon／interleukin 走 JAK／STAT——此為 anti-TNF、IL-1／IL-6 抑制劑與 JAK 抑制劑的介入點。
- **生物製劑三大限制**：核准門檻低（<span style="color:#f87171">ACR20</span>）、免疫抑制不可併用（伺機性感染）、選擇性手術前停藥（全關節置換前 2～4 週停 anti-TNF）。
- **RA 流行病學**：成人盛行率 0.5%～1%，55 歲以上 4.5%，年新增 5～50 例／10 萬人，目前仍無治癒方法。
- **適應性免疫**：MHC I → CD8+ CTL；MHC II → Th；Th1（IFN-γ、TNF、IL-2）促細胞免疫，Th2（IL-4、IL-5、IL-13）促體液免疫；B 細胞由膜上 IgM 轉為分泌型 IgG；記憶細胞歸居骨髓存續終身。
- **耐受與自體免疫**：中央耐受約 10% 逃逸，靠兩訊號假說與周邊耐受約束；CD40L／CD40 與 B7／CD28 為關鍵第二訊號，CTLA-4 可阻斷之；CD40L 缺陷造成 hyper-IgM 症候群。
- **腫瘤免疫**：CTLA-4（ipilimumab）、PD-1（pembrolizumab、nivolumab）、PD-L1（atezolizumab）抑制劑與 CAR-T（tisagenlecleucel）為代表；檢查點抑制劑僅限無其他治療可選的轉移性癌症。
- **疫苗與感染**：主動免疫（6 種平台，mRNA 效力最優，每劑約 US$20）／自然免疫（群體免疫閾值 60%～90% 不明）／被動免疫（半衰期 3～4 個月，REGEN-COV：casirivimab + imdevimab）。
- **ADE 與細胞激素風暴**：非中和性抗體可致病毒自內體逃逸、毒性複製，造成細胞激素風暴；重症病毒感染反而給予 corticosteroids 以預防風暴。
- **骨科終極挑戰**：手術部位感染與人工關節感染性骨髓炎 50 年來治療成果幾乎未變，且面臨抗藥性高毒力菌株威脅。
