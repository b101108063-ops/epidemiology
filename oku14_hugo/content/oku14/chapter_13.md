---
title: "Chapter 13: Biomaterials and Implants (生物材料與植入物): 骨科再生工程策略"
date: 2026-10-31
draft: false
tags: ["Orthopaedics", "OKU14", "Biomaterials", "Regenerative Engineering", "Tissue Engineering"]
categories: ["General Topics"]
weight: 13
summary: "本章回顧骨科再生工程的兩大研究取向（自上而下與自下而上）、原生細胞外基質的階層結構與機械轉導訊號，並以支架設計原則（生物相容性、機械完整性、可生物降解）為核心，比較凍乾、溶劑鑄造顆粒浸出、氣泡發泡、溶液與熔體電紡絲、三維列印到四維與五維列印等製造技術的臨床轉譯現況與限制。"
---

# Chapter 13: Biomaterials and Implants — 生物材料與植入物：骨科再生工程策略

**章節導讀**：本章聚焦骨科再生工程（regenerative engineering）的材料學基礎與支架製造技術。內容自研究典式（自上而下 vs. 自下而上）談起，經由原生細胞外基質（extracellular matrix, ECM）的階層結構與機械轉導（mechanotransduction）機制，深入支架設計三原則、電紡絲（electrospinning）與三維列印（3D printing）等製造技術，最後以臨床檢體研究（retrieval study）與動物模型證據收束，並指出各技術的限制。

---

## 1. 核心概念與再生工程策略 (Core Concepts & Regenerative Strategies)

### 1.1 研究典式：自上而下與自下而上

| 典式 | 核心思維 | 主要挑戰 |
|------|----------|----------|
| <span style="color:#60a5fa">自上而下（Top-down）</span> | 從臨床問題的病理生理出發，找出可攔截並改變疾病進程的介入點 | 需先診斷清楚且介入點明確 |
| <span style="color:#60a5fa">自下而上（Bottom-up）</span> | 從幹細胞與細胞訊息傳遞出發，藉生物材料與生長因子在空間與時間上的調控重建原生組織 | 重建原生組織極困難 |

此領域的終極目標並非單純的「修復」（repair），而是**再生**（regeneration）複雜組織與器官系統。要達成 bench-to-bedside 的轉譯，必須從一開始就清楚理解材料整合與臨床應用的挑戰。

> **Pearl**：兩種典式並非互斥。現代骨科再生工程（如 BMP-2 載體支架）本質上是兩者結合——由疾病機轉決定介入標的，再由材料學決定如何安全有效地局部釋放。

### 1.2 原生組織的階層結構與細胞－基質關係

原生組織維持複雜的**階層式結構（hierarchical structure）**：奈米尺度的細胞－組織交互作用影響微米尺度的組織微結構，微結構再決定巨觀的材料性質。這種尺度間的層層傳遞，是支架設計必須仿真的對象。

- **細胞活力維持**：經由擴散（diffusion）與整合的血管系統（vascularity）進行養分與氧氣輸送、廢物清除。
- **機械完整性**：組織須維持生物力學完整性，才能提供功能性支撐。
- **細胞－細胞與細胞－基質交互作用**：透過細胞特異性的訊息傳遞級聯（signaling cascades），並受生長因子、基質表面特性與整體結構影響，維持細胞外基質。

細胞外基質中的**膠原蛋白與蛋白聚醣（proteoglycans）**提供孔隙度與表面拓撲（topography），並運送生長因子以影響細胞行為。高孔隙率有利於細胞遷移、養分輸送、生長因子釋放與廢物移除。對間質幹細胞分化而言，**細胞－基質關係**可參與細胞命運決定。

> **Pearl**：高孔隙率是支架的第一號設計參數，但不能單獨最佳化，須與基質可降解性、力學支撐需求同步設計。

### 1.3 機械轉導與基質黏稠度

由於基質成分與水的互動，機械完整性內在於基質之中；**mechanotransduction（機械轉導）** 亦被證實會影響細胞功能。近年的研究更顯示**基質黏稠度（matrix viscosity）**在機械轉導中扮演關鍵角色：2020 年一項研究證實基質黏稠度可透過活化 **YAP/TAZ** 機械敏感轉錄因子來影響細胞命運。

> **Pearl**：設計支架時，「軟硬」之外還有「黏稠度」這個軸；同一材料經不同交聯程度而改變黏稠度，可能就足以改變幹細胞分化命運。

---

## 2. 支架設計原則與分類矩陣 (Scaffold Design Principles & Classification)

### 2.1 骨再生支架的三大功能屬性

| 屬性 | 英文定義 | 意義 |
|------|----------|------|
| <span style="color:#60a5fa">骨傳導性</span> | <span style="color:#e2e8f0">Osteoconductive</span> | 促進成骨細胞遷移與增殖 |
| <span style="color:#60a5fa">骨誘導性</span> | <span style="color:#e2e8f0">Osteoinductive</span> | 促進前驅細胞分化 |
| <span style="color:#60a5fa">骨整合性</span> | <span style="color:#e2e8f0">Osteointegrative</span> | 與宿主局部組織環境良好整合 |

### 2.2 再生工程的額外設計準則

| 準則 | 內容 |
|------|------|
| **生物相容性**（biocompatibility） | 不引起局部不良組織反應 |
| **機械完整性**（mechanical integrity） | 依目標組織的原生功能而定 |
| **可生物降解產物**（biodegradable products） | 產物不造成局部不良組織反應，且可被容易代謝 |

> **Danger zone**：原生骨是由膠原蛋白、脂質與其他蛋白質等多種成分構成的複雜材料。因此「理想的骨支架」很可能是**複合材料（composite material）**而非單一純材料——單一材料往往難以同時兼顧高生物活性與結構穩定性。

### 2.3 工程化組織的三種建構策略

| 策略 | 描述 |
|------|------|
| **僅細胞基質**（cell-only substrates） | 不使用支架，直接以細胞構建組織 |
| **僅支架基質**（scaffold-only scaffolds） | 支架本身具備體內再生能力 |
| **細胞＋支架複合** | 依賴細胞與基質在體外（in vitro）的交互作用 |

以韌帶與肌腱的修復與再生為例，研究已探索使用可降解聚合物（可加入或不加入多能幹細胞），並已有部分臨床轉譯成功。

> **Pearl**：支架製程會顯著影響材料最終可達成的物理與力學性質——同一種聚合物，製程不同就是不同的「材料」。發表時必須同時描述材料配方與製程。

### 2.4 傳統支架製造技術

| 技術 | 原理 | 優點 | 限制 |
|------|------|------|------|
| **凍乾**（freeze-drying） | 凍結後昇華去除溶劑，溶劑結晶留下孔隙 | 孔隙可控 | 快速原型與放大製造困難 |
| **溶劑鑄造－顆粒浸出**（solvent casting with particle leaching, SCPL） | 加入顆粒佔位劑後溶出形成孔隙 | 可模擬骨髓 niches | 同上 |
| **氣泡發泡**（gas foaming） | 以氣體發泡形成孔隙 | 製程簡單 | 孔隙結構較難精細調控 |


> **Pearl**：凍乾、SCPL 與氣泡發泡是最早的三種多孔支架製程，為多數臨床前研究的「黃金標準」。缺點在快速原型（rapid prototyping）與规模化製造（scalability）能力有限——正是後續轉向電紡絲與 3D 列印的驅動力。

### 2.5 支架表面改質與生長因子載入

<!-- FIG: 圖 1 — Schematic illustration depicts common scaffold fabrication techniques. -->

| 實例 | 結果 |
|------|------|
| 殼聚糖微球載入**阿侖膦酸鈉**（alendronate）於 PLA 支架 | 兔橈骨模型中骨再生較早且優於未載藥組 |
| PLLA 奈米纖維官能化 **I 型膠原蛋白**＋ **BMP** | 間質幹細胞貼附、細胞密度與增殖上升；BMP 使孔隙與纖維尺寸縮小，並促進成骨細胞分化（alkaline phosphatase 與 osteocalcin 表現上升） |
| 羥基磷灰石－殼聚糖奈米纖維以 **genipin**（水果來源、水溶性雙功能交聯試劑）交聯 | 模數增加 **5 倍**；在**非負重**骨組織再生有潛力 |

> **Danger zone**：genipin 交聯雖使模數上升 5 倍，但該研究僅顯示「非負重」骨再生的潛力，不可外推至負重部位。

---

## 3. 製造技術與臨床轉譯 (Fabrication Techniques & Clinical Translation)

### 3.1 電紡絲的原理與兩種次分類

**電紡絲（electrospinning）**已被確立為具擴展性（scalable）、材料選擇彈性大、可在受控且可重現條件下進行的方法。原理為：聚合物溶液置於高電壓電場中作為電極，液滴經毫米級噴嘴輸送，在電場作用下變形為 **Taylor cone**；當電力超過液滴表面張力時，形成帶電射流（charged jet stream）朝對應電極射出。

| 次分類 | 纖維生成方式 |
|------|--------------|
| <span style="color:#60a5fa">溶液電紡絲</span>（solution electrospinning） | 聚合物溶於適當溶劑，收集樣品的溶劑在來源與收集器間的空氣間隙蒸發後形成纖維 |
| <span style="color:#60a5fa">熔體電紡絲</span>（melt electrospinning） | 無溶劑技術，使用加熱熔融聚合物，收集樣品冷卻後形成纖維，可產出連續纖維供後續加工 |

**方向控制**：透過預程式化的幾何形狀，以及聚合物來源與收集器的相對運動，可將纖維定向排列。所得非織狀奈米纖維墊模擬細胞外基質，具有高表面積／體積比與可調控孔隙率。**影響纖維形態的參數**包括施加電壓、溶液流速、溶劑與聚合物性質、收集器距離、流變行為等。

> **Pearl**：電紡絲可透過同一製程產生開放互通孔或封閉孔、規則或偽隨機排列的結構，設計自由度極高。

<!-- FIG: Figure 2 — PLA 支架比較載入阿侖膦酸鈉的殼聚糖微球（CM-Als 10%）與未載藥（CM-Als 0%）；放射影像顯示 10% 組骨再生較早且較佳；掃描式電子顯微鏡顯示 PLA 支架（黑箭頭）與整合的微球（白箭頭）（Adapted from Wu H, et al: Sci Rep 2017;7(1):359）。 -->

### 3.2 電紡絲的階層化設計

透過收集單一纖維並製成纖維墊後，可利用**逐層堆疊（layer-by-layer stacking）、3D 編織或模板注塑**重建原生肌肉骨骼組織複雜的異向性階層結構。多軸纖維結構可依需求排列為單軸平行、輻射狀平行或波浪狀。

| 研究 | 設計 | 結果 |
|------|------|------|
| 絲蛋白（silk）＋ PLGA 複合支架 | 以機械強韌的**微纖維絲支架**為主體，奈米纖維 PLGA 提供類 ECM 的表面拓撲；PLGA 纖維摻入 **bFGF**（basic fibroblast growth factor）以控釋 | 促進播種的間質前驅細胞朝**成腱細胞分化**（tenogenic differentiation） |
| 聚磷腈－聚酯可降解奈米纖維矩陣 | 纖維直徑 **50–500 nm**，與原生膠原蛋白同尺度；同心排列並保留中央開放空腔，重現外層板狀骨與中央骨髓腔 | 體外加入成骨細胞後可於整體結構貼附與增殖；相較聚酯奈米纖維呈更高成骨表型；ECM 生成速率可匹配或超過支架降解速率以維持承載構件力學性質；壓縮模數落在海綿骨數值範圍中段 |

| 聚磷腈－聚酯可降解奈米纖維矩陣 | 纖維直徑 **50–500 nm**，與原生膠原蛋白同尺度；同心排列並保留中央開放空腔，重現外層板狀骨與中央骨髓腔 | 體外加入成骨細胞後可於整體結構貼附與增殖；相較聚酯奈米纖維呈更高成骨表型；ECM 生成速率可匹配或超過支架降解速率以維持承載構件力學性質；壓縮模數落在海綿骨數值範圍中段 |

> **Pearl**：聚磷腈（polyphosphazene）可與 poly(lactide-co-glycolide) 形成互溶共混物（miscible blend），降解速率調控性提升，且降解產物具緩衝能力可避免不利的局部細胞反應，同時保有力學性質調控性。

### 3.3 電紡後的表面修飾與交聯

<!-- FIG: 圖 3 — Images showing electrospun silk-poly(lactide-co-glycolide) scaffold wi -->

| 修飾方式 | 具體做法 | 體外／體內結果 |
|------|----------|----------------|
| 官能化 | PLLA 奈米纖維接上 I 型膠原蛋白、摻入 BMP | 幹細胞貼附、細胞密度與增殖增加；成骨分化↑ |
| 直接交聯 | genipin 交聯羥基磷灰石－殼聚糖奈米纖維 | 模數 ×5；非負重骨再生潛力 |
| 塗層 | 磷酸鈣塗覆於嵌段共聚物 PEOT-PBT 電紡纖維矩陣 | 兩類支架在加入間質幹細胞後體外皆見細胞增殖；但**裸鼠皮下植入後僅表面塗覆組形成新骨** |

> **Danger zone**：磷酸鈣塗層研究中兩種支架在**體外**都支持細胞增殖，但**體內**僅塗覆組骨形成——體外表現不等於體內表現。

### 3.4 機械模組調控細胞命運

研究利用**聚醚碸（poly(ether sulfone)）與聚己內酯（polycaprolactone）共混**電紡支架，以**核心－殼層排列（core-shell）**形成共混物，使模數相較單獨電紡聚己內酯提高 **4 倍**。

| 設計 | 細胞反應 | 分子標記 |
|------|----------|----------|
| **低模組**聚己內酯 | 促進**軟骨生成**（chondrogenesis） | 軟骨特異性 ECM 生成↑；Sox9 mRNA、II 型膠原 mRNA、聚集蛋白聚醣（aggrecan）蛋白染色上升 |
| **高模組**核心－殼層共混 | 促進**成骨**（pro-osteoblastic）環境 | Runx2、鹼性磷酸酶、osteocalcin 表現增加 |

> **Pearl**：此研究兩組支架的**微結構與表面化學完全相同**，僅模組不同——可乾淨地歸因「材料力學性質」本身對細胞命運的調控作用。

### 3.5 三維列印：減材與增材

| 類別 | 定義 | 特徵 |
|------|------|------|
| **減材製造**（subtractive） | 對原料切割、銑削或成形以取得最終結構 | 浪費原料 |
| **增材製造**（additive） | 逐層堆疊建構最終產品 | 幾乎無材料浪費 |

**3D 列印流程**：依 CT、MRI 等影像資訊建立電腦輔助設計（CAD）模型並轉為體積模型，再逐層製造產品，最後完成表面處理。材料與製程可分為兩大類：

| 類別 | 材料要求 |
|------|----------|
| **非生物列印**（nonbiologic） | 材料須在極高溫度下保持熱穩定，且完全生物相容 |
| **生物列印**（biologic） | 必須多孔以利養分與廢物移動、支持細胞黏附生長與分化，並具機械穩定性以承受身體負荷 |

傳統骨科材料如金屬、陶瓷與聚合物皆可 3D 生體列印。列印產品的客製化能力，加上列印機價格下降帶來的成本效益，使其在骨科成為極具吸引力的研發領域。

### 3.6 3D 列印的骨科臨床應用

| 應用 | 說明 |
|------|------|
| **術前規劃** | 由影像建立解剖模型 |
| **病人與住院醫師教育** | 3D 模型用於教學 |
| **術中截骨指引夾具**（custom jigs） | 客製化導板輔助截骨 |
| **病人專屬與非專屬植入物** | 醫材公司以增材製造原理生產人工髖關節植入物 |

**關鍵臨床發現（2021 年檢體研究）**：無菌性鬆動（aseptic loosening）仍是髖關節置換失敗的主要原因之一。2021 年一項檢體研究顯示，藉由增加摩擦係數並設計高度多孔結構，3D 列印可望解決此問題；其中 **3D 列印髖臼元件獲致更多的骨長入（bone ingrowth）**，提示更好的骨整合。因屬新技術，長期追蹤與檢體研究仍有限。

> **Pearl**：3D 列印對「骨整合」的第一個臨床級證據來自**髖臼檢體研究**，而非前瞻性 RCT——這是現階段的證據天花板。

### 3.7 3D 列印在再生工程的應用

骨是肌肉骨骼損傷處置中最常移植的組織；骨自體移植與同種異體移植的分別劣勢為**取骨部位病變**（donor site morbidity）與**傳染性疾病傳播**風險。**矽酸鹽生物活性陶瓷**（silicate bioactive ceramics）在體外與體內皆具優秀的成骨與血管新生活性；但理想骨支架可能是複合材料，以兼顧高生物活性與穩定性。由於骨支架最終要由宿主骨置換，**孔隙率對細胞貼附、增殖與分化至關重要**。

> **Danger zone**：單一矽酸鹽陶瓷雖具成骨活性，卻無法同時滿足結構與穩定性需求——正是複合材料路線的理由。

### 3.8 3D、4D 與 5D 列印

| 技術 | 原理 | 限制與展望 |
|------|------|----------|
| **3D 列印** | 三軸（X、Y、Z）增材製造 | 難以匹配複雜曲面結構——多數骨科組織具有複雜巨觀幾何形狀 |
| **4D 列印** | 與 3D 相同原理，但特定材料可**隨環境刺激改變形狀**（溫度、pH、磁場） | 產品可輕易塑形以適應術中所遇特定缺損；**智慧材料（smart materials）**對機械性質隨病人活動量劇烈變化的組織（如肌肉）再生具極大潛力 |
| **5D 列印** | 列印頭除列印床移動外，另動用**五個獨立軸向** | 現行機器同時採用增材與減材原理以降低材料浪費與生產成本；兩個額外軸可直接製造曲面結構，創造更強韌、幾何更複雜的構件，克服 3D 列印平坦分層結構的限制 |

### 3.9 電紡絲與 3D 列印的複合支架

| 研究 | 設計與結果 |
|------|------------|
| **BMP-2 雙相 PCL－透明質酸水凝膠** | 外周為類皮質骨殼層（水凝膠）提供最佳機械強度；第二相為多孔類海綿骨的熔體電紡微纖維網，允許骨生成與血管生成並支撐水凝膠相承重。骨生成標記（osteopontin、osteocalcin、I 型膠原）至第 14 天上升；細胞存活超過 21 天；兔體內出現新生骨 |
| **軟骨細胞 + PCL 複合支架** | 兩階段製程：以 PCL 溶於氯仿／乙醇作黏著劑，將電紡奈米纖維黏合於 3D 列印單層網格；黏著劑結合多層可控制支架最大厚度。軟骨細胞呈優異浸潤、存活與增殖，但**出現部分去分化（dedifferentiation）** |
| **成肌細胞列印（骨骼肌）** | PCL 支撐條提供結構形狀，電紡排列奈米纖維提供拓撲訊號；成肌細胞直接自含細胞支撐條列印至支架。細胞排列與密度控制更佳；肌源性基因表現上升，且**大幅受纖維排列方向影響** |
| **成肌細胞＋HUVEC 共培養** | 將人臍帶靜脈內皮細胞加入同一支架與列印成肌細胞共培養以促進血管新生。肌源性基因表現更高，肌球蛋白重鏈高度表現並具條紋樣排列 |

> **Pearl**：纖維的「排列方向」是跨組織共通的關鍵設計變項——排列奈米纖維同時改變成肌分化與骨骼肌構形。

### 3.10 無支架生物 3D 列印

2020 年一項研究探討**不需支架支持、直接 3D 列印幹細胞**用於軟骨再生：將脂肪來源間質幹細胞收集進入 3D 構形，待細胞密度足夠後即可操作與植入。bio-3D 列印結構植入**兔滑車溝（trochlear groove）直徑 4.8 mm 全層軟骨缺損**（full-thickness cartilage defect），植入後 3 個月評估：相較僅有全層缺損的對照標本，顯示**更佳的軟骨組織再生與移植物整合**。

<!-- FIG: Figure 4 — 用於軟骨再生的生物 3D 列印脂肪來源間質幹細胞移植物。A、B 針陣堆疊後列印構形的俯視與側視照片；C、D 細胞培養 6 天後照片；E、F 兔軟骨缺損植入時與體內 3 個月後照片；G、H 移植物植入 3 個月後與未植入對照缺損的組織學影像（Adapted from Murata D, et al: Regen Ther 2020;15:77-89）。 -->

> **Pearl**：bio-3D 列印（needle-array 針陣）讓「無支架自體細胞移植物」在體外即可塑形成可植入構形，是目前最接近臨床可轉譯的軟骨再生途徑之一。

---

## 4. 陷阱、限制與爭議 (Pitfalls, Limitations & Controversies)

### 4.1 電紡絲的固有不穩定

纖維方向的完全控制受製於製程本身的不穩定性：

| 不穩定類型 | 說明 |
|------------|------|
| **軸對稱 Rayleigh 不穩定** | 射流軸向收縮產生的波動 |
| **電場誘導軸對稱不穩定** | 高電場造成的軸向擾動 |
| **甩鞭／彎曲不穩定**（whipping/bending） | 射流擺動造成的 chaotic 纖維沉積 |

不穩定的**主要類型與影響程度**受合成參數影響，例如射流的表面電荷密度與半徑。舉例而言：**提高電場強度會增強電不穩定、但減弱 Rayleigh 不穩定**，其結果是纖維出現更大程度的 chaotic 甩鞭，進而**削弱引導纖維空間方向的能力**。

> **Danger zone**：「提高電壓＝更好纖維」是典型誤判——提高電場強度反而使甩鞭不穩定加劇、方向可控性變差。

**改良方向**：near-field electrospinning（近場電紡絲）與 melt electrowriting（熔體電寫）等技術已被研究，作為傳統電紡絲的改良，以減少 chaotic 纖維沉積。未來電紡絲最可能的定位，是作為**複合或多相支架中的一個構成要素**，用於需控制次微米尺度拓撲與功能的部位。

### 4.2 臨床轉譯的落差

> **Danger zone**：「體外表現」與「臨床結果」之間存在系統性落差，來源包括：細胞來源與動物模型差異、缺乏血管化、降解速率與再生速率不匹配、宿主免疫反應，以及負重條件下的力學需求。本章文獻多屬體外與小動物模型，臨床轉譯仍處早期。

### 4.3 3D／4D／5D 列印的現況

3D、4D 與 5D 列印技術在骨科與再生工程應用上**仍處於起步階段（infancy）**，但皆展現極大潛力，可推進快速原型化、複雜、大尺度組織再生的能力。

### 4.4 「修復」與「再生」之別

> **Pearl**：本章反覆出現的核心區分——再生工程的終極目標是**再生**複雜組織與器官系統，而非**替換**單一組織。判斷新材料價值時，應問「它讓宿主重新長出原本的組織結構了嗎？」而非「它暫時填上了缺損嗎？」

---

## 5. 實證更新與 OKU 14 重點 (Recent Evidence & Take-Home Points)

### 5.1 重要研究與技術進展一覽

| 主題 | 來源 | 要點 |
|------|------|------|
| **再生工程的典式** | Laurencin CT, Nair LS: Regen Eng Transl Med 2015 | 自上而下與自下而上兩條路徑 |
| **自體／異體／替代植體** | Baldwin P, et al: J Orthop Trauma 2019 | 骨移植選項證據多為低層級研究 |
| **ECM 與幹細胞命運** | Muncie JM, Weaver VM: Curr Top Dev Biol 2018 | ECM 兼具結構支撐與訊息傳遞；機械調控分化 |
| **基質黏稠度與機械轉導** | Cantini M, et al: Adv Healthc Mater 2020 | 分子離合（molecular clutch）模型 |
| **支架材料設計** | Koons GL, et al: Nat Rev Mater 2020 | 材料設計總覽；原生骨材料－機械功能關係 |
| **傳統支架製程** | Koyyada A, Prabhakar O: Reg Eng Trans Med 2020 | 凍乾、SCPL、氣泡發泡等製程選項與侷限 |
| **電紡絲技術** | King WE III, Bowlin GL: Polymers 2021 | 溶液／熔體電紡絲、近場電紡絲、熔體電寫 |
| **3D 列印與臨床應用** | Wixted CM, et al: J Am Acad Orthop Surg Glob Res Rev 2021 | 增材製造用於植入物、規劃與教育 |
| **骨整合檢體研究** | Dall'Ava L, et al: Bone Joint Res 2021 | 3D 列印髖臼元件骨長入優於傳統植入物 |
| **4D／5D 列印** | Reddy PR, Devi PA: Int J Mech Prod Eng Res Dev 2018 | 增材製造由 3D 至 4D、5D 的進展 |

### 5.2 OKU 14 關鍵研究要點（Key Study Points）

1. **支架原則**：再生工程應用的支架原則包含生物相容性、組織特異性最佳化的機械強度，以及允許細胞遷移與增殖的孔隙率。
2. **孔隙密度與壓縮模組可指導細胞命運**：置於**低模組**環境可將多能幹細胞引導至**促軟骨生成**（pro-chondrogenesis）細胞系；置於**高模組**環境則引導至**促成骨**（pro-osteoblastic）細胞系。
3. **電紡絲**：可透過帶電聚合物溶液（需溶劑蒸發形成纖維）或加熱聚合物熔體（需冷卻形成纖維）製造奈米尺度纖維支架；兩種製程皆能形成高度組織化的纖維排列，但受各種製程不穩定性限制。
4. **3D 列印**：使用增材製造原理，以多層聚合物形成複雜結構；**4D 列印**使用可回應環境訊號的特定聚合物；**5D 列印**藉由聚合物來源與列印收集床的相對運動（同時運用增材與減材製造原理），具備形成更強韌複雜結構的潛力。
5. **未來方向**：未來在電紡絲製程、結合智慧生物材料的 4D 列印，以及 5D 複雜且強度最佳化支架製造方面的工作，將引導再生工程領域走向提供可轉譯的醫療器材，用於肌肉骨骼組織、關節與肢體的置換。

### 5.3 骨科專科考試核心總結（Take-Home Points）

1. **三屬性 + 三準則**：骨支架必須兼具 **osteoconductive／osteoinductive／osteointegrative**，並符合生物相容性、依原生功能設定的機械完整性、產物可被代謝且不引起局部不良反應。
2. **ECM 是設計藍圖**：細胞外基質以階層結構連結奈米訊號與巨觀性質；膠原蛋白與蛋白聚醣提供孔隙度、拓撲與生長因子運輸。
3. **機械轉導是隱藏變項**：模組、黏稠度與纖維排列方向都可改變幹細胞命運；低模組 → 軟骨，高模組 → 骨。
4. **製程即材料**：凍乾／SCPL／氣泡發泡受放大製造限制；電紡絲可控但有甩鞭不穩定；3D／4D／5D 列印帶來幾何與智慧材料能力。
5. **臨床證據現況**：最接近臨床的證據為 **3D 列印髖臼元件骨長入檢體研究**與**兔模型軟骨再生研究**；體外結果都必須以體內與臨床資料重新確認。

---

## Summary

- **研究典式**：再生工程有自上而下（病理生理導向）與自下而上（幹細胞與訊息傳遞導向）兩條路徑；終極目標是**再生**而非修復複雜組織與器官系統。
- **支架三屬性**：骨傳導、骨誘導、骨整合；加上生物相容性、機械完整性、可生物降解產物三項準則。
- **ECM 與機械轉導**：細胞外基質的階層結構（奈米 → 微米 → 巨觀）決定材料性質；基質黏稠度經 YAP/TAZ 影響細胞命運；孔隙密度與壓縮模組可把多能幹細胞導向促軟骨生成或促成骨分化。
- **製造技術**：傳統為凍乾、溶劑鑄造顆粒浸出、氣泡發泡（受放大製造限制）；電紡絲（溶液型／熔體型）提供奈米拓撲與高表面積，但受 Rayleigh、電場與甩鞭不穩定限制；3D／4D／5D 列印分別帶來客製幾何、環境反應形變與五軸曲面強度。
- **臨床證據**：3D 列印髖臼檢體研究顯示骨長入與骨附著優於傳統植入物；bio-3D 列印脂肪來源間質幹細胞於兔 4.8 mm 全層軟骨缺損中再生優於對照；BMP-2 雙相 PCL－透明質酸支架在兔體內形成新骨。
- **主要陷阱**：體外表現不等於體內表現（磷酸鈣塗層僅表面塗覆組在體內成骨）；提高電場強度反而加劇甩鞭不穩定；非負重骨再生結果不可外推至負重部位；3D／4D／5D 列印在骨科應用仍屬起步階段。

---

## 參考文獻 (References)

1. Laurencin CT, Nair LS: Regenerative engineering approaches to limb regeneration and other grand challenges. Regen Eng Transl Med 2015;1(1):1-3.
2. Laurencin CT, Khan Y: Regenerative engineering. Sci Transl Med 2012;4(160):160ed9.
3. Murphy MB, Moncivais K, Caplan AI: Mesenchymal stem cells: Environmentally responsive therapeutics for regenerative medicine. Exp Mol Med 2013;45(11):e54.
4. Baldwin P, Li DJ, Auston DA, et al: Autograft, allograft, and bone graft substitutes: Clinical evidence and indications for use. J Orthop Trauma 2019;33(4):203-213.
5. Ogueri KS, Jafari T, Escobar Ivirico JL, Laurencin CT: Polymeric biomaterials for scaffold-based bone regenerative engineering. Regen Eng Transl Med 2019;5(2):128-154.
6. Koons GL, Diba M, Mikos AG: Materials design for bone-tissue engineering. Nat Rev Mater 2020;5:584-603.
7. Muncie JM, Weaver VM: The physical and biochemical properties of the extracellular matrix regulate cell fate. Curr Top Dev Biol 2018;130:1-37.
8. Steward AJ, Kelly DJ: Mechanical regulation of mesenchymal stem cell differentiation. Anat 2015;227(6):717-731.
9. Cantini M, et al: The plot thickens: The emerging role of matrix viscosity in cell mechanotransduction. Adv Healthc Mater 2020;9(8):2192-2264.
10. Karamanos NK, et al: A guide to the composition and functions of the extracellular matrix. FEBS J 2021;288(24):6850-6912.
11. Koyyada A, Prabhakar O: Recent advancements and associated challenges of scaffold fabrication techniques in tissue engineering applications. Reg Eng Trans Med 2020;7:147-159.
12. Shi C, Yuan Z, Han F, Zhu C, Li B: Polymeric biomaterials for bone regeneration. Ann Joint 2016;1(9).
13. Wu H, Lei P, Liu G, et al: Reconstruction of large-scale defects with a novel hybrid scaffold made from poly(L-lactic acid)/nanohydroxyapatite/alendronate-loaded chitosan microsphere. Sci Rep 2017;7(1):359.
14. King WE III, Bowlin GL: Near-field electrospinning and melt electrowriting of biomedical polymers-progress and limitations. Polymers 2021;13(7):1097.
15. Li WJ, Laurencin CT, Caterson EJ, Tuan RS, Ko F: Electrospun nanofibrous structure: A novel scaffold for tissue engineering. J Biomed Mater Res 2002;60(4):613-621.
16. Sahoo S, Toh SL, Goh JC: A bFGF-releasing silk/PLGA-based biohybrid scaffold for ligament/tendon tissue engineering using mesenchymal progenitor cells. Biomaterials 2010;31(11):2990-2998.
17. Deng M, Kumbar SG, Nair LS, et al: Biomimetic structures: Biological implications of dipeptide-substituted polyphosphazene-polyester blend nanofiber matrices for load-bearing bone regeneration. Adv Funct Mater 2011;21(14):2641-2651.
18. Ogueri KS, Escobar Ivirico JL, Nair LS, Allcock HR, Laurencin CT: Biodegradable polyphosphazene-based blends for regenerative engineering. Regen Eng Transl Med 2017;3(1):15-31.
19. Nam J, et al: Modulation of embryonic mesenchymal progenitor cell differentiation via control over pure mechanical modulus in electrospun nanofibers. Acta Biomater 2011;7:1516-1524.
20. Hohman M: Electrospinning and electrically forced jets: I. Stability theory. Phys Fluids 2001;13(8):2201.
