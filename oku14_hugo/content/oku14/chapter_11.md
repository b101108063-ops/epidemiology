---
title: "Chapter 11: New Technology in Orthopaedic Surgery（骨科手術新技術：機器人、人工智慧與機器學習）"
date: 2026-10-31
draft: false
tags: ["Orthopaedics", "OKU14", "Robotics", "Artificial Intelligence"]
categories: ["General Topics"]
weight: 11
summary: "本章回顧電腦輔助骨科手術的核心建構元素、三維定位與註冊技術，並依主動機器人、半主動觸覺導引、切板定位機器人、加速度計導引與徒手導航電動工具比較臨床證據；同時涵蓋增強與虛擬實境、國際標準，以及人工智慧在骨折判讀、植入物辨識、自然語言處理與風險調整支付模型上的應用與陷阱。"
---

# Chapter 11: New Technology in Orthopaedic Surgery — 骨科手術新技術：機器人、人工智慧與機器學習

## 章節導讀

本章拆解電腦輔助骨科手術（CAS）的建構元素：骨模型、三維定位與追蹤、註冊；並依運作原理分類主動機器人、半主動觸覺導引機器人、切板定位機器人、加速度計導引系統與徒手導航電動工具。同時檢視各系統的臨床數據、AR／VR、國際標準，以及人工智慧與深度學習在骨科影像判讀、植入物辨識、自然語言處理與支付模型上的應用與陷阱，最後提出「更容易、更快、更便宜、更好」四項判準。

---

## 1. 核心概念與技術建構元素 (Core Concepts & Building Blocks)

本章並非解剖學章節；其「關鍵結構」係指 **CAS 系統的建構區塊（building blocks）**：所有導航與機器人系統都依賴同樣的核心使能技術與步驟，差別只在這些步驟由誰執行、如何執行、以及在哪一步執行。

### 1.1 影像導引與非影像導引 (Image-Guided vs. Non-Image-Guided)

差別在於**是否建立病人專屬的虛擬解剖骨模型**，並在其上進行關節置換的規劃與執行。

| 面向 | Image-guided（以影像為基礎） | Non-image-guided（以非影像為基礎） |
|------|---------------------------|-------------------------------|
| 骨模型來源 | 病人 CT 或 MRI 建立病人專屬 3D 模型 | 取材自系統資料庫骨骼圖集（atlas）的模型 |
| 建模流程 | **segmentation（分割）** → **3D reconstruction（三維重建）** | 以 atlas 版本進行 **parametrization（參數化）** 與 **morphing（形變調整）** |
| 精度來源 | 病人專屬解剖，誤差少 | 需靠 kinematics registration 逼近病人解剖 |

**分割**以演算法從影像資料中取出代表一或多個骨或組織的資料點子集；以骨為例，因密度高，可將 CT 中 <span style="color:#22d3ee">Hounsfield unit（HU）</span> 高於某一門檻的所有點納入，軟組織位於較低 HU 區間，金屬植入物則位於相反極端。**重建**於分割後資料上建立虛擬 3D 模型：**Volumetric model（體積模型）**由大量極小立方塊（voxels）構成；**Surface model（表面模型）**較常用且運算效率高，為中空模型僅含表面，由互連的平面三角形組成。CT、MRI 乃至一般 X 光資料，皆可透過 <span style="color:#e2e8f0">DICOM</span>（Digital Imaging and Communications in Medicine）格式存取或傳輸。

### 1.2 病人專屬 PSI 與 Kinematic Registration

在影像式骨模型之上，可用一般或客製化的 CAD 工具為病人準備手術計畫，產物可以是**一個或多個 PSI**（patient-specific instrumentation，病人專屬器械），形式如帶槽的切骨塊（例如 TKA 用），通常以**積層製造（3D 列印）**打造，使其在手術中以單一方向吻合病人的骨輪廓。

> **Pearl**：PSI 的最大優勢在於**手術室內不需要追蹤或機器人系統**——只需一套客製切骨塊即可取代傳統器械組中動輒數百件的器械；但**術前規劃與 PSI 製造必須 involve 商業製造商**。

在非影像式系統中，術中測量值協助 morphing，包括髖關節中心與膝關節線的**位置與距離**、每一髁（condyle）的**最遠端點**、上髁（epicondyles）之間的**距離**。此過程稱為 <span style="color:#e2e8f0">kinematic registration（運動學註冊）</span>**，本質是骨模型的近似縮放與形變；再藉由追蹤不同骨段之間相對位姿（relative pose，即位置與方向）的運動，估計髖、膝、踝關節中心，並據此在虛擬電腦空間中決定機械軸。

### 1.3 三維定位與追蹤 (Three-Dimensional Localization and Tracking)

核心功能是讓**末端執行器（end effector）、導航指示器（pointer）、導航器械或機器人固定的植入物試件**能在空間中被定位：包含元件原點在 x、y、z 三軸的**座標**、繞三軸的三個**角度**，以及病人骨骼與手術視野內其他元件在同一時間點取得的**絕對位姿**；以目前技術，全部元件每秒重複量測並動態追蹤 **30 至 100 次**。

- **機器人自身感測**：手臂利用關節處的 onboard 位置與角度感測器量測末端執行器位姿。
- **外部追蹤系統**：*光學／紅外線追蹤*典型使用**兩台以小角度間隔配置的相機**，模擬人類雙眼的立體視覺，處理瞬時成對的二維影像以達成三維定位（含深度）；多數相機僅濾紅外光以降低雜訊。*磁場追蹤*亦可使用，但因金屬手術器械造成固有磁場干擾（noise），使用率遠較低。
- **標記物（markers）**：相機偵測主動或被動標記，通常呈獨特構形（<span style="color:#e2e8f0">reference frame / base / array</span>），由三個以上標記剛性固定於各被追蹤元件。主動標記實為電池供電的小型紅外 LED，有時以特定脈衝序列發光；被動標記是簡單銀色球體以反射紅外光。兩者皆**要求相機到被追蹤元件之間有清晰視線**。

### 1.4 註冊 (Registration)

**註冊**是量測與運算過程，用以在 3D 空間中把虛擬骨模型與病人實體解剖相互對應；每個參考座標架也須先註冊到其所附著元件的幾何形狀。**Point-to-point（點對點）**將預選 fiducial points（基準點）逐一對應到實體解剖地標；**Surface-to-surface matching（表面對表面配對）**則將實體表面數位化，運算其與骨虛擬模型等價表面區塊的最高相關（最小誤差）匹配位置。

> **Danger zone（判讀陷阱）**：註冊誤差是整條「影像 → 規劃 → 執行」鏈路的共同上游來源；註冊品質不佳時，後續再精確的機器人機械精度也無法補償。因此**任何報告單一數值（如角度誤差）的機器人研究，都應檢視其註冊方式與追蹤視線條件是否可重現**。

> **Pearl**：三種技術的差異可用一句話區分——**導航**由 3D 追蹤軟體引導使用者放置切骨塊，本身不主動執行；**被動／半主動機器人**由電腦依術前計畫與預核准切割區域，允許或抵抗術者手部運動；**主動機器人**則自行執行程式設定的切割路徑。

---

## 2. 機器人與導航系統的分類與決策矩陣 (Classification & Decision Making)

### 2.1 主動機器人 (Active Robots)：ROBODOC 的復興

最早且備受矚目的骨科主動機器人手臂為 **ROBODOC**（Integrated Surgical Systems／CA）；1990 年代末至 2000 年代初，**CASPAR**（OrthoMaquet／Germany）是另一廣受報導的系統。兩者皆為關節式機器人手臂，是產業界組裝的大型無塵室版本，能準確移動快速旋轉的切削磨頭（burr），依先前程式設定的切割路徑去除骨組織，類似電腦數值控制（CNC）加工製程。

> **Pearl**：ROBODOC 時代的關鍵教訓——**早期機器人看似「準確」，卻可能因學習曲線而在術中時間與失血量上付出代價**。美國 ROBODOC 髖關節置換多中心研究（136 個髖關節，約一半機器人、一半傳統對照）顯示機器人組**手術時間較長、失血量較高**。相對地，德國 900 例系列中 Harris Hip Score 從 **43.7 上升至 91.5**，手術時間自第一例的 **240 分鐘**迅速降至 **90 分鐘**；該系統被描述為安全有效，可產生影像學上較佳的植入物貼合與位置，同時消除股骨骨折。

ROBODOC 後來停止生產，由現代更新版本 **TSolution® One Robot**（THINK Surgical®，Inc.，Fremont, CA）取代。**現代改良方向**為整合跨領域創新：例如為較年輕與活動量大的病人開發**非骨水泥 TKA 脛骨側元件固定**並使日後翻修更容易；此方案將**創新的 TKA 脛骨元件設計（配合積層製造）與機器人**結合——輕巧敏捷的機器人手臂配備快速旋轉磨頭，於規劃階段自動程式化以準確銑削周邊固定鰭（fin）溝槽；另以較小、較輕的機器人執行植入物置入。

<!-- FIG: TSolution One Robot 與 Monogram 創新非骨水泥 TKA 脛骨元件加主動機器人手臂圖示 -->

### 2.2 半主動／觸覺導引機器人 (Semiactive, Haptically Guided)

<!-- FIG: 圖 2 — Graphical model of the TSolution One Robot-an active Semiactive Surgic -->

<!-- FIG: 圖 3 — Graphical models of the Monogram innovative nonce- mented tibial compo -->

此類系統中**術者以手部操作末端執行器**（攜帶旋轉磨頭、近期為 TKA 骨鋸或 THA 擴髓器）。系統同樣預先載入手術計畫（通常為 CT 影像式骨模型加上磨頭／切除器械尖端模型，呈現於電腦螢幕）。術者手部與末端執行器之間設置**六自由度 load cell**，感測術者欲移動機器人末端方向上的力與力矩。

> **Pearl**：此類系統的哲學是**「術者主導方向，機器人守住邊界」**——電腦依術者動作是否遵循術前計畫與預核准切割區域，決定「允許」或「抵抗」該動作。此概念在美國由 **Mako** 大力商業化。

Mako 起家以旋轉磨頭執行**單髁膝置換（unicompartmental knee arthroplasty）**骨切除，近期進展至控制髖關節置換的**擴髓器（reamer）**、膝關節磨頭，最終並在膝關節置換中由機器人末端固定**擺動式動力鋸（oscillating power saw）**。Mako 使用者介面允許術者執行表面切除；現代系統的外周器械可協助引導術者進行韌帶張力調整與間隙平衡（gap balancing）。

### 2.3 定位切骨導引的機器人 (Robots That Position Cutting Guides)

此類機器人定位帶槽的切骨導引，由槽引導擺動鋸片。最早者為 **Praxim/Omni 骨固定版本**（OMNIBot，Corin）：以兩支 pin 自切口內固定於**遠端股骨側面**。其 **imageless configuration（無影像配置）**用於 TKA，並搭配 **BalanceBot**——具兩片可伸縮厚度的擋板分置左右膝髁之下；於**脛骨切除後**置入膝關節，致動至一定力量水平，量測內外側間隙。

> **Pearl**：BalanceBot 的價值在於**將「軟組織包絡」量化**——在股骨切除前，讓膝關節通過整段活動範圍並量測內外側間隙，藉此輔助間隙平衡。

| 項目 | OMNIBot + BalanceBot | ROSA® Knee（Zimmer Biomet） | VELYS™（DePuy Synthes） |
|------|----------------------|---------------------------|----------------------|
| 固定方式 | 骨固定，2 支 pin 固定於遠端股骨 | 非骨固定；機器人臂固定於大型輪式底座櫃 | 兩輪式櫃體（two-wheeled cabinets） |
| 追蹤方式 | 與 BalanceBot 協同 | 另有獨立輪式控制台，含外部紅外相機追蹤末端執行器／切骨塊 | 整體定位靠可調整／可鎖定鉸鏈手動完成；精準定位由靠近末端的小型馬達致動器完成 |
| 優缺點 | 體積小、可結合韌帶張力器 | 切骨塊定位**更穩固**，但占地面積大、價格高 | 體積較小、重量較輕，剛性僅小幅妥協 |
| 臨床數據 | 逾 **30,000 例 TKA**（其中 **10,000 例**用韌帶平衡器）的臨床資料於 2021 年研究回顧；機械軸線改善約 **0.5°**；一個 cohort 3 年存活率 **99.26%**，另一個 766 例 TKA 系列 6 年存活率 **99.4%** | 8 位骨科醫師以 ROSA 協助 TKA、涵蓋 3 種不同植入物設計，**角度誤差 < 1°**、precision（以標準差量測之散佈）與平均切除平面偏移及散佈 **< 1 mm**，且由**另一套**電腦輔助系統於同一手術驗證 | 相對新穎，合理長度的臨床結果**稀少** |


### 2.4 限制器械運動之機器人 (Constrain the Motion of a Power Instrument)

<!-- FIG: 圖 5 — Photograph shows the ROSA " ' Knee System with a cut- Figure 6 Graphic -->

<!-- FIG: 圖 4 — A, Graphical model of the OMNIBot bone-mounted small robot (Corin, UK) -->

由前述機器人系統自然演進而來的方向，是讓機器人手臂**約束動力器械（矢狀鋸）的運動**，使其只能在單一期望平面內自由活動。

### 2.5 加速度計導引系統 (Accelerometer-Based Systems)

<!-- FIG: 圖 1 — Cellular constituents of bone. Histologic images and brief description -->

**小型、智慧的被動裝置**，於術中提供資訊。相較傳統機械器械，多數**不需要額外的 pin**，也沒有導航伴隨的視線問題；部分為拋棄式單次使用、無菌手持器械，部分僅部分如此。其運作採如智慧型手機般的**微型加速度計（accelerometry）**，量測相對於地球重力場與磁場的傾斜角度；結合**電子羅盤**與**重力方向感測**在三個互相正交的軸上運作，可裝置於單一手術器械上，多個元件並可**無線互動**。同一電子裝置亦可含**微型 load-cell 力感測器**，協助 TKA 屈曲間隙平衡與韌帶調整。系統實例包括 Lantern（OrthAlign）、iAssist（Zimmer Biomet）、Dash（Brainlab AG, Munich）。

> **Danger zone（加速度計系統的固有限制）**：加速度計**固有的無力量測位置或距離**——它只導引角度，不導引位置；準確度與反應速率亦僅屬中等。不過這在關節置換中尚可接受，因其使用呈**準穩態（quasi-steady-state）**：骨與器械雖會動動，但被假設在每次瞬間讀值時為靜止。

> **Pearl**：加速度計系統最具吸引力之處在於**相對大型機器人與導航系統的實用性**：功能類似且只需附著於機械切骨塊，學習曲線較短，幾乎不增加手術室占地面積、無視線問題，且對骨髓腔侵入性較小。

### 2.6 徒手導航電動工具 (Freehand Navigated Power Tools)

<!-- FIG: 圖 7 — Graphical models of the accelerometer-based systems. A, Lantern (Copyr -->

另一條根本不同的途徑，是**直接為骨切除電動工具導航**，術者如常手持並徒手操作。最早商業化者為 **Navio**（Bluebelt，現 Smith & Nephew），原用於單髁膝置換，現亦用於 TKA。此為**非影像式**導航（依賴 kinematic registration），追蹤手持裝置，並在**位置偏離手術計畫時控制速度、快速阻擋磨頭尖端**。Navio 已累積充足臨床資料，例如單髁膝置換 **128 例、平均追蹤 2.3 年、存活率 99.2%**。用於 TKA 的 Navia 系統近期接受評估，報告在機械軸、股骨冠狀面、矢狀面、旋轉、脛骨後傾與脛骨冠狀面對位等準確度上；所有鋸切面偏離計畫之**均方根誤差（root mean squared error）不超過 0.56°**。病例對照研究（70 例 Navio TKA）顯示學習曲線為 **11 例**即與標準器械等效，肢體對位與元件位置無差異。

> **Pearl**：Navio 已改進為 **CORI**（Smith & Nephew），配備**快五倍**且更利於切除與牽开的磨頭，並具更快速的註冊流程；因推出極新，目前尚無已發表結果。

| 版本 | 運作方式 | 優點 |
|------|---------|------|
| **Externally tracked tool** | **不需**切骨塊或其他機械器械；外部紅外線相機直接追蹤電動器械本身，提供即時 3D 引導、圖形回饋與速度控制 | 回饋亦透過智慧型手機提供，可選擇外接電腦螢幕 |
| **On-tool tracking** | 相機追蹤元件與電子電路整合於**裝在電動器械頂端的無線模組**內；另含**微型投影儀**，將引導或影像投影至骨面，顯示術者應從何處開始切割及如何 orient 器械 | 追蹤相機、電子電路與圖形回饋**全部機上化**並投影於骨面，多方面降低侵入性 |

更常見的電動工具（矢狀鋸與 reciprocating 擺動鋸、鑽頭）也已內建導航與智慧功能，且不增加太多重量或耗電、不影響無線使用的自由度、不需任何繫留的電力或訊號纜線。該技術在多次體外（in vitro）TKA 實驗（包含 2 例 cadaver 程序）中完成特性描述，骨切除時間**短於**傳統器械；詳細骨切除評估顯示表面粗糙度與植入物貼合度與傳統器械相當，而**表面對位優於**傳統器械。此技術與標準骨科鋸與鑽具直覺相容，並有潛力改善 TKA 對位、**縮短手術時間、減少手術器械數量**；器械更少、滅菌需求更低可降低 TKA 相關成本。

<!-- FIG: 外接追蹤與器械上追蹤的徒手導航骨切除器械照片（Haider H, PhD） -->

### 2.7 決策矩陣：如何選擇系統類型

<!-- FIG: 圖 8 — Graphical models of the CORI latest freehand navigated burr system. Th -->

| 考量 | 加速度計／徒手導航 | 大型機器人／導航 | PSI |
|------|------------------|------------------|-----|
| 學習曲線 | 較短 | 較長 | 最短（僅需熟悉切骨塊） |
| 手術室占位 | 幾乎不增加 | 顯著增加（ROSA、VELYS 體積大） | 幾乎不增加 |
| 術前流程 | 徒手工具無 | 需 CT 與規劃流程 | 需 CT 與商業製造商製造流程 |
| 對位精度來源 | 角度導引／3D 即時追蹤 | 3D 追蹤 + 硬性約束 | 病人專屬切骨塊 |
| 流程負擔 | 低 | 中至高（學習曲線） | 低，但需等待製造 |

---

## 3. 臨床證據與成本效益 (Evidence & Cost-Effectiveness)

**Mako 與單髁膝置換**：2020 年一篇納入 **21 篇** Mako 系統單髁膝置換研究的**系統性回顧**顯示，相較傳統技術，在植入物對位準確度、軟組織平衡、病人功能分數與滿意度、併發症率與學習曲線的短期結果上均有短期優勢；但作者明確指出，**這些發現尚不能外推至中期與長期結果**。

**機器人 vs. 傳統 TKA**：2022 年一項回顧性研究以 **1:1 配對**，比較 6 位高 volume 術者的 **2,392 例**傳統 TKA 與另 6 位高 volume 術者使用 Mako 系統的機器人 TKA（指標含手術時間、住院天數、總直接費用、90 天併發症、急性後期照護使用與 30 天再入院）。

| 指標 | 結果 |
|------|------|
| 住院天數中位數 | 兩組相同 |
| 90 天併發症率 | 無顯著差異 |
| 手術時間 | 機器人較傳統**長超過 10%** |
| 總直接費用中位數 | 機器人 **$11,615** vs. 傳統 **$8,674**，**P < 0.0001** |

> **Danger zone（成本論陷阱）**：作者亦**將成本的合理化理由懸而未決**，前提是較低的翻修率與／或更好的功能結果能夠抵銷此差距。評估任何機器人投資時的核心爭議是：<span style="color:#fbbf24">成本效益必須與臨床結局綁在一起看，不能只比較單次手術費用</span>。

**輕量導航的準確度證據**
- **iASSIST 對照光學導航**：短期（6 個月）前瞻性配對研究（**每組 38 膝**，iASSIST vs. 使用 Ci（DePuy Synthes/BrainLab）導航系統的對照組），病人報告結果與對位量測均**無顯著差異**；但 iASSIST 組**手術時間較短**，且**每例增加約 $1,000 成本**。2019 年系統性文獻回顧與 meta-analysis 合併 **558 膝**，約一半 iASSIST、一半傳統器械；iASSIST 組的**對位離群值（alignment outliers）比傳統 TKA 少 45%**；然而**手術時間延長**，短期功能分數**未見明顯優勢**。
- **OrthAlign（加速度計）對照大型無影像 CAS 系統**：**超過 96%** 的脛骨切除在冠狀面與矢狀面對位上**誤差在 ±2° 以內**；**超過 93.8%** 的股骨遠端切除與整體機械軸**誤差在 3° 以內**。與大型控制台無影像 CAS 系統（**AchieveCAS**，Smith & Nephew）的配對 cohort 比較結果相近。**100 例**前瞻性隨機對照研究將 OrthAlign 與傳統（**extramedullary** 髓外）機械器械比較，上述對位數值**僅由機械器械達成不到約 72%**。

> **Pearl**：文獻一致支持——**可攜式加速度計器械在 TKA 達成目標對位的準確度與精確度，與大型導航系統相當，且優於傳統機械器械**；代價是額外手術時間。

---

## 4. 增強／虛擬實境、國際標準與陷阱 (AR/VR, Standards & Pitfalls)

### 4.1 增強與虛擬實境 (Augmented and Virtual Reality)

**AR／mixed reality**整合多種技術，透過顯示媒介（半透明螢幕或鏡片）呈現真實物理場景，並將電腦輸出疊加其上，將虛擬內容帶入使用者自然視野；這直接對應本章導航與機器人主題。**VR**則讓使用者完全沉浸於虛擬環境，所見皆為電腦 3D 輸出；藉 3D 追蹤使用者頭部（即視線方向），使用者隨視角改變即時感受到圖像變化，故主要用於骨科手術**訓練與模擬器**——住院醫師可戴上頭戴裝置立即進入人造手術室，先熟悉器械、植入物與特定術式步驟。

**AR 技術難點與解方**：早期挑戰是**如何在平面電腦螢幕上顯示 3D 資訊**，同時讓使用者（頭／眼）運動能自動改變電腦 3D 算繪輸出以因應視角變化。當 AR 與**可穿戴 3D 眼鏡**（如 Microsoft HoloLens，內建相機並以附加在手術場景元件上的標記做 3D 追蹤）結合後大幅簡化：眼鏡隨使用者頭部移動並以立體視覺顯示；當 3D 圖形透過左右兩個獨立鏡片算繪，且場景中物件被追蹤時，即可輕易決定透視並將虛擬輸出疊加於實體骨骼。

| 系統 | 廠商 | 說明 |
|------|------|------|
| **HipInsight** | Surgical Planning Associates, Boston | FDA 核准的 AR 為基礎 3D 導引系統；Microsoft HoloLens 2 頭戴眼鏡搭配客製軟體，透過影像標記追蹤固定於髖臼的機械架上的骨盆位置 |
| **ARVIS** | Insight Medical Systems, Austin | **Augmented Reality Visualization and Information System**；目鏡可相容於典型骨科手術頭盔；協助遠端脛骨與股骨 TKA 切除及髖臼杯植入的導引，方向引導方式為將實體 impactor 與虛擬對應物**對齊** |
| **NextAR** | Medacta, Switzerland | 以 AR 為基礎的 TKA 手術平台，讓術者即時獲得韌帶平衡回饋並顯示於虛擬螢幕；已延伸至**肩關節置換與脊椎** |

開發者宣稱 ARVIS 展現與導航及機器人系統相當的準確度，並據此取得 FDA 核准，但**這些結果尚未發表**。

> **Danger zone（AR 系統的現實限制）**：上述三個系統在撰寫本章時都相當新，**沒有可引用的已發表臨床結果**。其缺點在於**術者視野與病人佩戴頭戴裝置之間可能互相干擾**；實際表現將取決於準確度以及**被導引的是何種手術工具或器械**。

> **Pearl**：AR 相對於傳統導航與機器人系統形成鮮明對比——後者設備笨重、工作流程繁複，而 AR 試圖把運算能力帶進術者視野。

### 4.2 臨床前測試與國際標準 (Preclinical Testing & International Standards)

<!-- FIG: 圖 10 — Photographs show augmented reality platforms. A, mounted glasses with -->

骨科植入物與醫療器械皆須經臨床前測試，並在包含臨床前驗證（verification）與確認（validation）測試的文件完整描述後，才取得 FDA 核准（clearance）。多數植入物標準由專家制定並由 **ASTM International** 或 **ISO** 出版；ASTM F04 委員會（Medical and Surgical Materials and Devices）與 ISO/TC150 委員會（Implantable Devices）的植入物委員會相對精簡，但導航與機器人橫跨更廣的委員會範圍，包括處理所有電機機械安全的 **IEC**（例如 **IEC 80601-2-77**，機器人輔助手術設備之基本安全與必要性能的特殊要求）以及 **AAMI**（Association for the Advancement of Medical Instrumentation）。

**ASTM F04.38「Computer Assisted Orthopaedic Surgical Systems」小組**已制定兩項標準：**ASTM F2554**（Measurement of Positional Accuracy of Computer Assisted Surgical Systems）與 **ASTM F3107**（Measuring Accuracy after Mechanical Disturbances on Reference Frames of Computer Assisted Surgery Systems）。

> **Pearl**：這兩項標準都是**開創性**標準，處理所有手術導航與機器人賴以運作的最基本功能——但**對於驗證系統整體準確度仍遠不足以夠**：尚無法回答「切骨塊放置是否正確」「機器人引導或約束磨頭是否正確」「切除後骨面是否平滑、位置與對位是否正確」，更不用說其後固定上去的植入物對位。

**ISO 19233-1**：*Implants for surgery—Orthopaedic joint prosthesis—Part 1: Procedure for producing parametric 3D bone models from CT data of the knee*，為術前手術規劃、導航、機器人手術、病人配對器械與個人化全膝關節假體建立虛擬骨模型的**參數化與產生流程**標準，並協助界定骨掃描影像的條件，以及分割與 3D 骨模型重建的規範。

> **Danger zone（標準化不足的現實）**：在此領域**測試標準化仍然缺乏**——撰寫標準是產業界、監管機關（如 FDA）、一般科學家、工程師以及作為最終使用者的外科醫師之間的**國際共識活動**。

---

## 5. 人工智慧、機器學習與深度學習 (Artificial Intelligence & Machine Learning)

### 5.1 三者的定義與差異

**人工智慧（AI）**一般指從簡單或複雜、大量資料中做出決策的電腦演算法，具備某種程度的**模擬認知**；這類演算法使電腦能在**沒有完整且明確規則**的情況下，從特定資料集中**學習既有模式**，無須明文規定「哪個模式／特徵會對應哪個結果」。專家才能完全體會的三種演算法細微差異如下。

| 類別 | 描述 |
|------|------|
| **1. Intelligent algorithms** | 自電腦誕生以來即以軟體撰寫的智慧型演算法 |
| **2. Knowledge-based systems** | 早期出現的知識型系統；與表格化資料集或關聯式資料庫結合並寫入查表程序與決策規則後，表現得更為智慧 |
| **3. Neural network-based systems** | 規則極少、或至少較不明確的神經網路系統；當規則變得模糊、演算法被程式化為在結構化資料與結果中尋找模式，或最佳化程式設計師自己（嘗試看似無限多、甚至數量過於龐大而不可行的可能性之前）無法預測的決策時，**第三類在現代機器學習中潛力爆發** |

**機器學習（ML）**：利用歷史（訓練）資料，讓演算法預測前所未見的輸入資料組合與情境之解答／結果；任何新的組合都可加入演算法所使用的資料集，形成**持續自我學習**的過程。**深度學習（deep learning）**：當資料集結構更少（如 X 光等醫學影像，或 CT／MRI 的 DICOM 資料）、規則變得不連貫甚至稀缺、模式更為複雜時，便被認為需要深度學習能力；其涉及**多層神經網路**，結構類似人腦，原始資料輸入後逐層進入更高階的抽象層級。

### 5.2 人工智慧在醫療的整體定位

過去十年間，人工智慧已成為社會上幾乎所有部門（尤其醫療保健）投入與研究最多的概念之一。病人、疾病與治療路徑是極度複雜、變數無限且彼此互相依存的過程；變數數量龐大，意味著同一疾病過程的每次照護（episode of care）都可能有極大的結果變異，尤其當治療路徑由不同的控制單位（照護提供者）執行時。

> **Pearl**：人工智慧的理論優勢在於——它能**更系統性地消化這些變數**，以預測成功率最高的結果或治療路徑，並從真實病人結果中持續學習。

近年的重點在於收集與分析 **big data**（大數據），這不僅改善了當前效率，更**推動了骨科手術中人工智慧的發展**。大數據現存於大型資料庫中，部分為正式的**國家登錄（national registries）**；資料庫由個別醫師輸入手術類型、危險因子、併發症、植入物類型與住院天數等，目標是辨識特定之相關性。**AI 最自然的醫療應用**是**建模與最佳化照護路徑模型**，其中在**心理健康、心臟科、皮膚科、眼科與放射科**最為成功。

### 5.3 骨科的具體應用 (Specific Applications in Orthopaedics)

骨科中的人工智慧主要以**影像辨識**領先並多集中於此：

| 應用領域 | 說明 |
|---------|------|
| **骨折判讀與創傷** | 所有 AI 模型皆能辨識骨折，但各模型的演算法與訓練方法差異顯著 |
| **骨關節炎偵測與分級** | 深度學習與 AI 模型已成功於 X 光辨識骨關節炎嚴重程度，以及於 MRI 辨識軟骨病灶；並可預測人體膝關節的早期症狀性骨關節炎 |
| **髖與膝植入物元件辨識** | 見下節詳述 |
| **肌肉骨骼腫瘤** | AI 具偵測骨與軟組織腫瘤的潛力；亦可由 micro-CT 影像進行癌症骨分割 |
| **前十字韌帶損傷、脊椎病變** | 已有相關應用發表 |

> **Pearl**：**關節置換再次領先**——原因很可能是接受相同照護路徑的病人量體龐大，而該路徑基於影像與病人因子，非常適合機器學習演算法。連**骨關節炎偵測**本身除了用於量化骨關節炎程度與評估置換手術結果外，也能**協助將病人分流至適當的手術或非手術診間（clinic）**。

### 5.4 植入物辨識 (Implant Detection)

從 X 光影像進行植入物辨識的進展極為驚人，這對**翻修手術**至關重要——尤其在**缺乏先前手術資訊**的情況。製造商與設計日益增加、且沒有充足紀錄時，辨識病人體內使用了哪一種植入物是一大挑戰；若某次翻修僅需更換植入系統的單一元件（如 TKA 的 UHMWPE 承載墊片，或鬆動的髖臼杯），問題便變得嚴重。

| 研究 | 設計與結果 |
|------|-----------|
| **深層卷積網路（THA 設計辨識）** | 以 **252 張**已知三種 THA 植入物設計的術後 X 光**訓練**，自動在 **25 張**新 X 光上辨識其類型。同一團隊另以 **402 張** X 光將演算法結果與**三位具骨科專科認證的外科醫師**比較，發現深層學習系統**快得多且準確度相當** |
| **Karnuta 等（髖臼）** | 以 **1,766 張 AP X 光**訓練與驗證，涵蓋 **1,715 位病人的 18 種**不同股骨柄元件；經 **1,000 個訓練循環**後，於 **206 張**測試 AP X 光中辨識出來自 **4 家製造商**的 18 種元件，準確度 **> 99%**。文獻註記：準確度 **99.6%**、**sensitivity 94.3%**、**specificity 99.8%** |
| **膝關節植入物** | 在 **74 張**測試 X 光中辨識 **9 種**來自 **4 家製造商**的獨特膝關節置換植入物，準確度接近完美；該深度學習演算法以 **424 位病人的 682 張** X 光訓練 |
| **Borjali 等（2021，Med Phys）** | 以訓練好的卷積神經網路辨識失敗的 THA 植入物設計準確度極高，**僅需 0.06 秒**——顯著且更準確地快於受訓的骨科醫師 |
| **Borjali 等（2020，J Orthop Res）** | 卷積神經網路辨識三種常用 THA 植入物設計達 **100% 準確度**；可用於術前在數秒內自動辨識失敗 THA 植入物設計，節省時間並提升辨識準確度 |

> **Pearl**：當電腦能在數秒甚至數分之一秒內完成上述辨識，證據便令人信服：**人工智慧已能夠、或極快地將能夠，以比任何人類都更快、更可靠、更有效率的方式，辨識病人體內的骨科植入物——即使沒有紀錄可查**。

### 5.5 臨床與手術室流程效率及成本

成本控是多數骨科醫師討論議程中的重點。控制成本的主要途徑之一是**推行 bundled payment plans（打包支付方案）**，實質上是將控制成本的責任轉移給醫院與醫師。早期打包支付方案並不完善，因為每位病人的照護存在不可避免的變異性，卻缺乏辨識可能導致成本升高因素的能力；因此降本努力演變成**競逐最低化（race to the bottom）**，常影響病人照護品質與醫師士氣，許多醫院與醫師因選擇退出。這些支付模式仍會持續存在以控成本，但**當前的努力方向是更好地辨識與預測可能導致成本升高的風險**；因此機器學習演算法被用於以**術前病人專屬共病資料**計算風險校正、病人專屬的照護 episode 支付模型。

> **Pearl**：以複雜病人專屬變數為基礎的模型，不僅能協助**辨識節省成本的策略**，更能**預測結果期望值（outcome expectation）**。隨著醫師與醫院持續收集、記錄與整理病人資料，人工智慧將可進行複雜分析，不僅辨識「尚不知道其存在」的模式，更能以**符合成本效益與時間效益**的方式提供高度精確的病人專屬照護。

### 5.6 自然語言處理 (Natural Language Processing)

**自然語言處理（NLP）**指電腦辨識、詮釋並可能分析人類語言的能力，目標是建構**適應性的模擬思考過程**。語言處理最早的形式是**語音辨識**；照護提供者近來使用語音辨識技術將人類語言轉譯為醫療紀錄中的文字，雖然這藉由免除轉錄／打字而提升時間效率，但它**不會分析語境、不會將資料轉換為連貫（參數化）形式，也不會在個別病人互動的脈絡中提供任何回饋**（例如填入資料庫欄位）。

| 能力 | 說明 |
|------|------|
| **即時回饋** | 於病人就診過程中提供即時回饋，讓醫師得以與病人互動並提問，以改善病歷記錄 |
| **病歷撰寫** | 協助形成不僅準確且針對個別病人客製，同時**符合編碼標準**的病歷 |
| **指令辨識** | 辨識如「請為這位病人安排手術」等指令，可據此安排手術日期，並通知照護團隊從診間到手術室所需的**術前流程** |
| **工作流程自動化** | 此類「workflow」自動化能力可偵測心臟病史並**自動轉介**至病人的心臟科醫師進行術前許可——這是避免遺漏手術前必要條件的眾多例子之一 |

**Dragon Ambient eXperience**（Nuance of Burlington, MA，近期由 Microsoft 接手）是醫療自然語言處理的領導者；此新推出的人工智慧平台 aims to improve automatic real-time documentation and clinical intelligence。隨著技術持續改進，**可能只需數年**就能讓每個診間都配備人工智慧平台，從第一次診間到可能的術後結果都能簡化並改善病人照護。

> **Pearl**：作者對此技術的整體評價是——它確實會讓骨科醫師的工作**更容易、更快、更便宜、更好**。

### 5.7 人工智慧的挑戰與結論性評語 (Challenges & Concluding Comments)

儘管潛力巨大，人工智慧在骨科領域**仍處於非常早期的階段**，並且已受到某些批評。

> **Danger zone（資料品質造成的假陰性陷阱）**：主要疑慮是**資料的準確度**，引出核心問題：**演算法會不會學錯？** 這已發生於大型資料庫研究——它們完全依賴所收集與分析資料的品質與應用類型。若資料**從一開始就缺乏足夠的粒度（granularity）**，產生**假陰性與假陽性結果**的潛力便會增加。

原文舉例說明：假設某登錄系統回報的 TKA 植入物存活率為粗略資料，僅記錄整體成功或失敗（是否翻修）。假設某 TKA 有創新且最佳的骨固定特徵（鰭、龍骨等），但**矢狀面與冠狀面承載面吻合不佳**，犧牲了約束度（膝穩定性）並造成病人不適，因而**僅因後者**而頻繁翻修。若登錄系統（典型做法）**未回報失敗的詳細原因**，而僅歸因於某個特定細粒度設計特徵，則一個**假陰性結果可能會被歸咎於整個系統**，連帶譴責了那些其實良好的固定特徵。

**AI 應用於醫療的四個關鍵前提**：大型且準確的資料集、強大的運算能力、雲端運算，以及**開源的演算法開發**。這些都不遙不可及，但**持續改善文件記錄的準確度與更具細粒度的資料至關重要**，因為這會直接影響人工智慧的準確度。

> **Pearl**：人工智慧在骨科領域持續發展的潛力，是成為**新的照護標準（standard of care）**，前提是有足夠的檢核與平衡機制監督其準確度。目前文獻中**極少有研究**試圖比較人工智慧與現有已知方法的準確度；然而隨著技術成長，其能力將遠超其他資料分析領域所能比較的範圍，且**可以預期它將被信賴為黃金標準（gold standard）**。

> **Danger zone（監管誤讀）**：**法規（FDA）clearance 不等同於 approval**。採用導航與機器人手術技術的倫理極為複雜，而**責任在於外科醫師**——必須詳盡檢視所提供的文獻並自行判斷。

---

## 參考文獻

1. Bargar WL, Bauer A, Borner M: Primary and revision total hip replacement using the Robodoc system. Clin Orthop Relat Res 1998;354:82-91.

2. Cobb J, Henckel J, Gomes P, et al: Hands-on robotic unicompartmental knee replacement: A prospective, randomised controlled study of the Acrobot system. J Bone Joint Surg Br 2006;88:188-197.

3. Lin J, Yan S, Ye Z, Zhao X: A systematic review of MAKO-assisted unicompartmental knee arthroplasty. Int J Med Robot 2020;16:e2124.

4. Tompkins GS, Sypher K, Li H, Griffin M, Duwelius P: Robotic versus manual total knee arthroplasty in high volume surgeons: a comparison of cost and quality metrics. J Arthroplasty 2022;37(8S):S782-S789.

5. Shatrov J, Murphy GT, Duong J, Fritsch B: Robotic-assisted total knee arthroplasty with the OMNIBot platform. Arch Orthop Trauma Surg 2021;141:2087-2096.

6. Goh GS, Liow MHL, Lim WS, et al: Accelerometer-based navigation is as accurate as optical computer navigation in restoring the joint line and mechanical axis after total knee arthroplasty. J Arthroplasty 2016;31:92-97.

7. Kinney MC, Cidambi KR, Severns DL, Gonzales FB: Comparison of the iAssist handheld guidance system to conventional instruments for mechanical axis restoration in total knee arthroplasty. J Arthroplasty 2018;33:61-66.

8. Li J, Gao X, Li X: Comparison of iASSIST navigation system with conventional techniques in total knee arthroplasty: A systematic review and meta-analysis. Orthop Surg 2019;11:985-993.

9. Nam D, Cody EA, Nguyen JT, Figgie MP, Mayman DJ: Extramedullary guides versus portable, accelerometer-based navigation for tibial alignment in total knee arthroplasty. J Arthroplasty 2014;29:288-294.

10. Battenberg AK, Netravali NA, Lonner JH: A novel handheld robotic-assisted system for unicompartmental knee arthroplasty. J Robot Surg 2020;14:55-60.

11. Savov P, Tuecking LR, Windhagen H, Ehmig J, Ettinger M: Imageless robotic handpiece-assisted total knee arthroplasty: a learning curve analysis. Arch Orthop Trauma Surg 2021;141:2119-2128.

12. Haider H, Barrera OA, Garvin KL: Minimally invasive total knee arthroplasty surgery through navigated freehand bone cutting. J Arthroplasty 2007;22:535-542.

13. Beam AL, Kohane IS: Big data and machine learning in health care. JAMA 2018;319:1317-1318.

14. Bini SA: Artificial intelligence, machine learning, deep learning, and cognitive computing. Arthroplasty 2018;33:2358-2361.

15. Cabitza F, Locoro A, Banfi G: Machine learning in orthopedics: a literature review. Front Bioeng Biotechnol 2018;6:75.

16. Rainey C, McConnell J, Hughes C, Bond R, McFadden S: Artificial intelligence for diagnosis of fractures on plain radiographs. Intell Based Med 2021;5:100033.

17. Joseph GB, McCulloch CE, Sohn JH, et al: AI MSK clinical applications: cartilage and osteoarthritis. Skeletal Radiol 2022;51:331-343.

18. Karnuta JM, Luu BC, Roth AL, et al: Artificial intelligence to identify arthroplasty implants from radiographs of the knee. J Arthroplasty 2021;36:935-940.

19. Karnuta JM, Haeberle HS, Luu BC, et al: Artificial intelligence to identify arthroplasty implants from radiographs of the hip. J Arthroplasty 2021;36:S290-S294.e1.

20. Borjali A, Chen AF, Bedair HS, et al: Comparing the performance of a deep convolutional neural network with orthopedic surgeons on the identification of total hip prosthesis design. Med Phys 2021;48:2327-2336.

## Summary

### 6.1 技術世代的整合框架

| 技術類別 | 核心機轉 | 臨床現況 |
|---------|---------|---------|
| **導航** | 3D 追蹤軟體引導切骨塊或髖臼擴髓器的**定位** | 成熟；需相機視線 |
| **機器人** | 自動致動上述切骨塊或切除器械的**定位** | 主動（ROBODOC、TSolution One）、半主動（Mako）、切板定位（OMNIBot、ROSA、VELYS）、器械運動約束 |
| **PSI** | 依術前影像式骨建模與手術規劃的基本原理提供切骨塊，**不需導航或機器人** | 多數骨科植入物製造商均提供；**術前需獨立準備流程** |
| **加速度計** | 以微型加速度計導引**角度** | 輕量、學習曲線短、幾乎不占手術室空間；**不能量測位置** |
| **徒手導航工具** | 直接導航手持電動器械，術者徒手操作 | Navio／CORI；on-tool tracking 將追蹤與投影機機上化 |
| **AR／VR** | AR 將 3D 虛擬內容疊加於真實場景；VR 提供沉浸式訓練 | HipInsight、ARVIS、NextAR；**均無已發表臨床結果** |
| **AI／ML** | 影像辨識、流程最佳化、語言處理 | 骨科仍處早期；植入物辨識已達近完美準確度 |

### 6.2 骨科專科考試核心總結（Take-Home Points）

1. **CAS 三大建構區塊**：骨模型（影像式 vs. 非影像式 morphing／kinematic registration）→ **註冊**（point-to-point 或 surface-to-surface）→ **三維定位追蹤**（x/y/z 座標加三軸角度，每秒 30–100 次；光學追蹤佔主流，磁場追蹤受金屬器械干擾）。
2. **PSI 的取捨**：病人專屬切骨塊免去術中追蹤與機器人，但**術前須商業製造商參與規劃與製造**。
3. **系統分類**：導航只「引導定位」；被動／半主動機器人「允許或抵抗」術者動作；主動機器人「自行執行程式設定的切割路徑」。
4. **早期機器人的教訓**：ROBODOC 在美國多中心研究（136 髖）出現手術時間延長與失血增加（學習曲線），但在德國 900 例系列中 Harris Hip Score 43.7 → 91.5、時間 240 → 90 分鐘。
5. **成本是機器人最大的爭議**：Mako 機器人 TKA 總直接費用中位數 $11,615 vs. 傳統 $8,674（P<0.0001），手術時間長 10% 以上，住院天數與 90 天併發症率則無差異；成本合理化須以較低翻修率與更好功能結果為前提。
6. **輕量方案未必落後**：加速度計系統在 TKA 達成目標對位的準確度與大型導航系統相當（OrthAlign：96% 脛骨切除 ±2°、93.8% 股骨遠端／機械軸 3° 以內），而機械器械僅達不到約 72%；但代價是額外手術時間。
7. **AI 最成熟的應用是影像辨識**：骨折判讀、骨關節炎分級、植入物辨識（THA 18 種元件準確度 > 99%，0.06 秒完成；失敗 THA 設計辨識 100% 準確度）；關節置換之所以領先，是因照護路徑高度標準化。
8. **標準化尚不夠**：ASTM F2554、F3107 與 ISO 19233-1 處理的是基本功能，無法驗證整體系統準確度；撰寫標準本身是國際共識的困難過程。
9. **AI 的最大陷阱是資料粒度**：粗略資料會製造假陰性，並可能讓好的設計特徵被整體系統「連坐」譴責。
10. **四項判準**：任何新技術都應以「**更容易、更快、更便宜、更好**」檢驗；**FDA clearance 不等於 approval**，最終判斷責任在外科醫師。

---
