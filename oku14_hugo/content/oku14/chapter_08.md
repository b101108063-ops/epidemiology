---
title: "Chapter 8: Musculoskeletal Biomechanics and Biomaterials（肌肉骨骼生物力學與生物材料）"
date: 2026-10-31
draft: false
tags: ["Orthopaedics", "OKU14", "Biomechanics", "Biomaterials", "Basic Science"]
categories: ["General Topics"]
weight: 8
summary: "本章為骨科基礎科學章節，依序介紹載荷與剛度量測、應力應變曲線、彈性模數、屈服點、極限抗拉強度與疲勞等材料力學概念，再闡述黏彈性、實驗測試方法，以及超高分子量聚乙烯、骨水泥、皮質骨與海綿骨、各類金屬合金與陶瓷的特性，最後聚焦於生物相容性與腐蝕（點狀、裂隙、機械輔助裂隙）之失效機轉與臨床陷阱。"
---

# Chapter 8: Musculoskeletal Biomechanics and Biomaterials — 肌肉骨骼生物力學與生物材料

## 章節導讀

本章提供骨科臨床不可或缺的兩大工具箱：**生物力學**（材料在載荷下如何反應）與**生物材料**（植入物由何種材質構成、又如何與人體共存）。前半段由載荷模式、剛度與應力—應變曲線談起，說明疲勞與黏彈性為何決定植入物的長期命運；後半段比較超高分子量聚乙烯、骨水泥、皮質骨／海綿骨、不鏽鋼、鈷鉻、鈦、陶瓷、鋯與鉭等材料，並以鈍化膜與三種腐蝕型態解釋全髖關節 <span style="color:#e2e8f0">trunnion</span>（頸柄錐狀接點）為何是臨床腐蝕的熱點。

---

## 1. 核心概念：載荷、應力與材料力學 (Core Concepts: Loading, Stress & Material Mechanics)

### 1.1 載荷模式與剛度的量測 (Loading Modes & Stiffness Measurement)

要評估長骨的剛度與強度，可將其置於單一或數種**具生理關聯性**的載荷組合下測試；實驗量測的基本變數是**力（force）**與**位移（displacement）**、**扭矩（torque）**與**旋轉（rotation）**。

| 載荷模式 | 量測變數 | 由力學曲線導出之剛度 | 影響因素 |
|---------|---------|------------------|---------|
| <span style="color:#e2e8f0">軸向載荷（axial）</span> | 力－位移 | 軸向剛度（axial rigidity） | 幾何形狀（<span style="color:#22d3ee">截面慣性矩</span>）＋材料彈性模數 |
| <span style="color:#e2e8f0">扭轉載荷（torsion）</span> | 扭矩－旋轉 | 扭轉剛度（torsional rigidity） | 慣性矩＋材料彈性模數 |
| <span style="color:#e2e8f0">彎曲載荷（bending）</span> | 力－位移 | 彎曲剛度 | 斷面係數＋模數；須用靜力平衡方程求最大彎曲力矩位置 |
| <span style="color:#e2e8f0">複合載荷</span> | 生理相關組合 | 綜合剛度 | 依載荷情境而定 |

- 力－位移（或扭矩－旋轉）曲線**線性段的斜率**即代表軸向或扭轉剛度。
- 剛度**不只**取決於材料本身的彈性模數，也取決於被測物體的**幾何形狀**。
- **較長的骨與植入物位移量整體上會比短的更大**。
- 對骨幹端（metaphysis）等**複雜幾何**或植入構造物，單純的實驗量測不足以解析；2021 年一篇研究指出需採用**有限元素（finite element）計算模型**等更精緻的方法。

### 1.2 彎曲試驗的三種配置 (Three Bending Configurations)

純彎曲力矩不易直接施加，通常以下列三種方式施力，再以**靜力平衡方程**推算最大彎曲力矩的位置：

1. **懸臂彎曲（cantilever bending）**：一端固定於空間，另一端施力 → 最大彎曲力矩在**固定端**。
2. **三點彎曲（three-point bending）**：兩個固定垂直支撐，中點施反向垂直力 → 最大彎曲力矩（**連同剪力**）位於**施力點**。
3. **四點彎曲（four-point bending）**：在三點彎曲的基礎上**再加一個垂直載荷點** → 最大彎曲力矩分布**不再集中於單一點**，而是形成一個**區帶（zone of maximum bending moment）**。

> **Pearl**：三點彎曲「一處最大力矩」與四點彎曲「一段最大力矩區」是判讀骨折固定構件受力時最常被混淆的差異；疲勞裂縫易沿恆定應力區生長。

### 1.3 應力—應變曲線 (Stress-Strain Curve)

<span style="color:#e2e8f0">Stress-strain relationship</span>：由力學實驗的載荷－位移關係換算而得，是研究天然組織與骨科植入物力學的核心。

- <span style="color:#e2e8f0">應力（stress）</span>：施加於**單位截面積**上的力量。
- <span style="color:#e2e8f0">應變（strain）</span>：材料因該應力而產生的**伸長量相對於原始長度**的比例。
- 應力－應變關係是針對**材料**定義；載荷－位移關係則是針對**整體構造物**評估，因此**還受結構幾何影響**。

| 曲線特徵 | 物理意義 | 臨床對應 |
|---------|--------|---------|
| 線彈性區（linear elastic region） | 彈性變形 | 正常承重下的骨與植入物行為 |
| 屈服點（yield point） | 材料開始變為塑性 | 永久損傷的臨界點 |
| 塑性區（plastic region） | 塑性變形 | 骨水泥微裂、植入物永久變形 |
| 極限抗拉強度（ultimate tensile strength） | 材料可承受的最大應力 | 急性載荷下的斷裂強度 |
| 破壞（failure） | 材料失效 | 骨折或植入物斷裂 |


> **Pearl**：圖 3C 顯示**載荷速率越快，材料表現越剛**——這正是骨與植入物在「跌倒」等高能量情境下比在步行等一般活動中更不易變形、卻更易碎裂的力學原因。

### 1.4 彈性模數與材料選擇 (Elastic Modulus)

<!-- FIG: 圖 3 — Graphs show stress-strain behavior. A, An idealized stress-strain curv -->

<span style="color:#e2e8f0">Young modulus</span>（彈性模數）是應力－應變曲線**彈性區的斜率**，代表材料的**剛度（stiffness）**。

- 用途：比較與篩選骨科材料。
- 臨床警訊：<span style="color:#f87171;font-weight:600">骨－植入物模數不匹配（bone-implant modulus mismatch）</span> 常被列為**應力遮蔽（stress shielding）**與**植入物失效**的原因之一。

### 1.5 屈服點、塑性變形與極限抗拉強度 (Yield Point, Plastic Deformation & UTS)

- **屈服點**：分隔彈性區與塑性區；**超過屈服點，材料可能承受永久性損傷**。屈服後材料在**應力增加極少**的情況下產生塑性伸長（yielding）。
- **應變硬化（strain hardening）**：因**原子與結晶結構改變**，塑性變形反而**提高材料抵抗進一步變形的能力**。
- **極限抗拉強度（UTS）**：材料破壞前能承受的**最大應力**；超過此點後延性材料仍可繼續伸長但**應力下降**，並伴隨**頸縮（necking）**——**截面積縮小**。

> **Danger zone**：骨科植入物在體內**通常以循環載荷而非急性載荷失效**，因此對植入物而言，**極限抗拉強度的相關性低於疲勞強度**；臨床判讀不應只引用 UTS。

### 1.6 疲勞特性 (Fatigue Properties)

體內生理載荷是**循環性**的——每一步行走、每一次手臂伸展都是一個載荷循環。

- <span style="color:#e2e8f0">疲勞強度／疲勞極限（fatigue strength / fatigue limit）</span>：材料在**特定循環次數**下所能承受的**最高應力**。
- **載荷循環次數逐步增加**，最終導致**脆性（brittle）**形式的破壞。
- **在低於屈服強度的反覆循環載荷下發生破壞**，稱為**疲勞破壞（fatigue failure）**。

> **Pearl**：疲勞破壞不需要超過屈服強度，這解釋了為何「材料強度合格」卻仍在數年後發生植入物斷裂。

### 1.7 黏彈性：遲滯、應力鬆弛與蠕變 (Viscoelasticity)

多數生物材料為**黏彈性（viscoelastic）**，同時呈現彈性與黏性行為。

| 概念 | 定義 | 意義 |
|------|------|------|
| <span style="color:#e2e8f0">Elasticity（彈性）</span> | 移除致變形應力後回復原形的能力 | 可逆變形 |
| <span style="color:#e2e8f0">Viscosity（黏性）</span> | 抵抗**速率依賴**變形的能力 | 變形速率相關 |
| <span style="color:#e2e8f0">Hysteresis（遲滯）</span> | 變形過程中**耗散部分能量** | 載卸载曲線不重疊；**載荷段高於卸載段** |
| <span style="color:#e2e8f0">Creep（蠕變）</span> | **恆定載荷下變形量增加** | 長期下陷／鬆弛 |
| <span style="color:#e2e8f0">Stress relaxation（應力鬆弛）</span> | **固定應變下應力隨時間下降** | 載荷被「吸收」 |

黏彈性材料在移除應力後會回到原形，但其反應含有黏性成分，因而**決定回復原形所需的時間**。

> **Danger zone**：應力鬆弛在骨科有非常實際的應用——**骨水泥填充於植入物柄周圍時，因應力鬆弛使張力隨時間下降，因此骨水泥永远不会達到造成疲勞破壞所需的應力水準**。

---

## 2. 實驗測試方法 (Experimental Testing)

### 2.1 平台實驗的定位

**平台實驗（benchtop test）**是預測植入物臨床前表現的有力工具：依應用情境施加軸向、彎曲、扭轉，或**六自由度（six-degrees-of-freedom）複合載荷**（例如**髖臼頭與骨螺絲**的接觸情境）。

- **靜態載荷（static loading）**：評估材料**剛度**。
- **動態載荷（dynamic loading）**：可決定**磨損（wear）特性**或**疲勞強度**。

### 2.2 載荷控制 vs 位移控制

| 測試方式 | 做法 | 用途 |
|---------|------|------|
| <span style="color:#60a5fa">載荷控制（load-controlled）</span> | 施加載荷，量測材料變形 | **最常見**的試驗類型 |
| <span style="color:#fbbf24">位移控制（displacement-controlled）</span> | 給定位移，量測反力 | 常用於模擬特定位移情境 |

2009 年 Schwenke 等人的研究即比較載荷控制與位移控制下全膝關節置換的**磨損差異**。

> **Pearl**：同一植入物在「載荷控制」與「位移控制」試驗台得到的磨損量可以不同；閱讀磨損文獻時必須先確認試驗的控制模式。

---

## 3. 生物材料類別與生物相容性 (Biomaterial Classes & Biocompatibility)

### 3.1 骨組織的力學特性 (Cortical & Cancellous Bone)

骨的力學行為複雜，因其具有**異質性（heterogeneous）**、**各向異性（anisotropic）**與**黏彈性（viscoelastic）**三重性質。

- 皮質骨與海綿骨**持續接受靜態與動態載荷**，因此**疲勞載荷**是其機械行為的核心。
- <span style="color:#60a5fa;font-weight:600">皮質骨在縱向載荷下比橫向更強、更剛；受壓時比受張時更強。</span>
- 皮質骨的強度與剛度**取決於載荷速率**：**載荷越快，剛度越高**。

### 3.2 超高分子量聚乙烯 (Ultrahigh-Molecular-Weight Polyethylene, UHMWPE)

<span style="color:#e2e8f0">UHMWPE</span> 是熱塑性聚乙烯，自 **1960 年代**起即廣泛用作**膝與髖植入物的承載面（bearing material）**，具較其他聚合物**更高的抗斷裂性與生物相容性**。

- **高結晶度**帶來高 **Young 模數**、高**屈服強度**、**抗蠕變變形**能力與**增強的疲勞強度**。
- 高分子量雖賦予良好的**耐磨性**，但**體外（ex vivo）與體內（in vivo）的氧化都會使其下降**。
- 上述疑慮促成**輻射交聯（radiation cross-linking）**的發展：**高度交聯 UHMWPE 於 1990 年代問世**，用以**降低氧化降解**。
- 高度交聯 UHMWPE 已成為**全髋關節置換的事實標準（de facto standard）**，並在**全膝關節**中逐漸普及。

> **Pearl**：交聯的代價是材料初始模數較高、韌性下降（微裂紋易於交聯區萌生）；這是「更耐磨但更脆」的典型取捨。

### 3.3 骨水泥：聚甲基丙烯酸甲酯 (Polymethyl Methacrylate, PMMA)

<!-- FIG: 圖 1 — Portable AP radiograph obtained in the trauma bay Atraumatic Evaluatio -->

<span style="color:#e2e8f0">PMMA</span>（壓克力）是**剛性熱塑性材料**，因具備良好生物相容性而用於骨水泥。

- **雖無黏著性（not adhesive）**，但可作為**空間填充劑**，並藉由**不規則骨表面與假體之間的機械性互鎖（mechanical interlock）**達到固定。
- 骨水泥**受壓強度高於受張強度**，且**Young 模數低**。
- 其性質**溫度依賴**：例如**溫度升高則蠕變增加**。
- 所有 PMMA 骨水泥皆會出現**蠕變與應力鬆弛**。

### 3.4 合金選擇的原則 (Alloy Selection Principles)

骨科合金**並非**嚴格依機械性能（如強度）來選擇，而是依據「**適當的機械性能 + 生物相容性**」。

| 主要合金 | 特性定位 | 典型角色 |
|---------|--------|---------|
| <span style="color:#e2e8f0">鈦（Titanium）</span> | 最佳耐蝕性、延性較佳 | 多孔塗層（fiber metal）、部分關節置換部件 |
| <span style="color:#e2e8f0">鈷鉻（Cobalt-Chromium）</span> | 剛度與整體硬度高 | **承載面（bearing surface）**理想材料 |
| <span style="color:#e2e8f0">不鏽鋼（Stainless Steel）</span> | 韌性佳、成本低 | 骨折固定器材、暫時性植入物 |

- 各合金在**強度、延性、硬度**上的差異，一般決定其被用於何種應用或植入物部件。
- 存在機械性能更佳的其他合金，但**正是這三大合金的高生物相容性與耐蝕性**，使其被廣泛用於**承重植入物**。

> **Danger zone**：骨科合金之所以被選用，**不是因為機械性能（強度）最佳，而是因為耐蝕性最佳**；評估新型合金時務必納入耐蝕性與鈍化膜穩定性。

### 3.5 不鏽鋼 (Stainless Steel)

- 骨科最常用型號為 **316L**（**ASTM F138**）。
- 加入**鉬（molybdenum）**以**增強晶界的耐蝕性**。
- **鉻**均勻散布於微結構中，使金屬表面可形成**氧化鉻（Cr₂O₃）**。
- 不鏽鋼皆經**表面處理**（例如**硝酸**）以促進**鈍化氧化層的生長與增厚**。

### 3.6 鈷鉻合金 (Cobalt-Chromium)

骨科使用最常見的兩種鈷鉻合金為：

1. **鈷鉻鉬（Co-Cr-Mo）**：**ASTM F75 與 F76**。
2. **鈷鎳鉻鉬（Co-Ni-Cr-Mo）**：**ASTM F562**。

因其**剛度與整體硬度**，此類合金**極適合作為承載面**。

### 3.7 鈦合金 (Titanium)

- 鈦表面氧化層的**穩定性**帶來**高耐蝕性**與**相對較高的延性**（可冷加工），因此常用於**人工關節假體的多孔塗層**（如 fiber metal）；**Ti-6Al-4V（ASTM F136）** 因**機械性能優於純鈦**而用於關節置換部件。

| 比較項目 | 數值／敘述 |
|---------|-----------|
| Ti-6Al-4V 相對 Co-Cr-Mo 的硬度 | 約 <span style="color:#fbbf24">15% 較軟</span> |
| Ti-6Al-4V 在承載面應用的磨損 | 比 Co-Cr-Mo **多 15%** |
| 結論 | <span style="color:#f87171">鈦合金在以耐磨為首要考量的部位極少使用</span> |

> **Danger zone**：鈦的生體相容性極佳，但**在承載面耐磨性不足**；將鈦合金頭用於全髖或全膝承載面，磨損量可比 Co-Cr-Mo **高出 15%**。

### 3.8 陶瓷 (Ceramics)

陶瓷因其**優越的耐磨性與生物相容性**而被引進作為**承載面**；其硬性、剛性、低摩擦，以及因**離子鍵**與**化學穩定性（inertness）**而賦予的**抗進一步氧化能力**，使其機械性能與生物相容性俱佳。

- 陶瓷機械性能主要受**晶粒尺寸細小**與**完全致密度**控制：**晶粒尺寸小** → 控制冷卻時**熱收縮**所生的**內部應力**；**完全致密** → 任何**孔隙（void）** 都會**增加機械應力**；兩者共同**提高硬度、降低脆性與斷裂率**。
- 主要陶瓷：**氧化鋁（alumina, Al₂O₃）** 與**氧化鋯（zirconia, ZrO₂）**。

**氧化鋁基質股骨頭（alumina matrix femoral head）** 的組成：

| 成分 | 比例 | 作用 |
|------|------|------|
| <span style="color:#e2e8f0">氧化鋁（alumina）</span> | 75% | 基質 |
| <span style="color:#e2e8f0">氧化鋯（zirconia）</span> | 24% | 分散顆粒**增加韌性** |
| <span style="color:#e2e8f0">氧化鉻（chromium oxide）</span> | 1% | **增加硬度**；同時造成材料呈**粉紅色** |

> **Pearl**：氧化鋁基質股骨頭的「粉紅色」來自其中 1% 的氧化鉻，來源於氧化鋯基陶瓷的製造方式，而非染色處理。

### 3.9 鋯與鉭 (Zirconium & Tantalum)

<span style="color:#e2e8f0">鋯（Zr）與鉭（Ta）</span> 屬於**耐火金屬（refractory metals）**，**極度耐磨**（其他耐火金屬尚包括**鉬**與**鎢**）。

| 比較項目 | 數值／敘述 |
|---------|-----------|
| 耐火金屬硬度與耐磨性 | 約為 **Co 與 Ti 合金的 10 倍** |
| <span style="color:#e2e8f0">Oxinium</span> | **氧富集**處理的鋯合金，外層轉為**陶瓷性氧化鋯表面** |
| <span style="color:#e2e8f0">多孔鉭（porous tantalum）</span> | **惰性（inert）**，限制與骨之間的交互作用 |
| 多孔鉭表面處理 | **鹼性環境熱處理**形成**羥磷灰石（hydroxyapatite）**，增加**骨交錯（bone interdigitation）** |
| 多孔鉭力學調整 | 高孔隙率使**彈性模數接近海綿骨**；**摩擦係數高** → 與海綿骨初期固定較佳 |
| 多孔鉭耐蝕性 | **極高**（表面有厚而穩定的鈍化層）→ 生物相容性高 |

> **Pearl**：多孔鉭的「高摩擦係數 + 接近海綿骨的彈性模數」是骨長入（osseointegration）的兩大設計槓桿，與鈦合金的「低模數、可冷加工」策略形成互補。

---

## 4. 失效模式、磨損與腐蝕 (Failure Modes, Wear & Corrosion)

### 4.1 腐蝕的驅動力與三個步驟 (Corrosion: Driving Force & Steps)

腐蝕由材料**趨向較低化學能狀態**的傾向所驅動，發生於**電子由陽極（失去電子）流向陰極（獲得電子）**之際。這是**放熱過程，活化能極低**，因此反應可自發發生——可快可慢。

- **裸露金屬表面**（無保護性氧化膜）直接暴露於空氣或水溶液時，反應會**劇烈放熱**。極佳例子是**鈦**：真空製程鈦粉的氧化速率與釋放能量如此驚人，以致**曾被用作固態火箭推進劑**；而 **ASTM 鈦合金腐蝕速率極低**，是理想植入材料。差異在於 **ASTM 鈦合金暴露於氧氣時迅速形成保護性氧化膜（鈍化層）**，此過程稱**鈍化（passivization）**；2019 年研究指出該膜幾乎**完全停止金屬表面腐蝕**。

**腐蝕的三個基本步驟**：

| 步驟 | 名稱 | 內容 |
|------|------|------|
| 1 | **氧化（oxidation）** | 表面金屬溶入水性環境，**陽離子被移除** |
| 2 | **還原（reduction）** | 剩餘電子被表面另一處的**差異電荷**吸引，形成**電流**並推動反應 |
| 3 | **產物形成** | 形成**金屬氧化物**或**金屬氫氧化物（鏽）**副產物，在表面構成**絕緣層**，抑制反應動力學並隔絕金屬免於進一步腐蝕 |

### 4.2 鈍化膜 (Passive Film)

- 鈍化膜是**防止骨科植入物腐蝕的關鍵**。
- **金屬氧化物**比**金屬氫氧化物**更**穩定、溶解度更低、絕緣性更佳**。
- 鈍化膜**不具導電性**，可阻止離子（電流）由水溶液層流向金屬表面，因而**限制腐蝕速率**。
- 此類膜**僅能由特定種類的金屬合金形成**：具有**穩定鈍化性能**的金屬包括 **Ti、Cr、Ta、Nb、Zr**。
- 相對地，**Cu、In、Sn** 雖可形成金屬氧化層，但這些保護層在**氯離子**（生理溶液主要成分之一）存在時**會迅速溶解**；殘留金屬元素則腐蝕形成**金屬氫氧化物（鏽）**層，**限制離子移動與腐蝕的能力有限**。
- 鈍化膜**並非靜態**，而是**持續的穩態平衡**：厚度與保護能力是**侵蝕反應與生成反應**的平衡結果。

<!-- FIG: Figure 4 — 腐蝕類型示意。A，基本腐蝕：氧化還原反應形成金屬氫氧化物（鏽）或金屬氧化物（鈍化膜）。B，點狀腐蝕：鈍化膜阻止腐蝕，膜上缺陷讓腐蝕得以發生。C，裂隙腐蝕：同點狀機轉但發生於密閉空間，受限擴散造成 pH 下降與氧張力降低。D，機械輔助裂隙腐蝕（MACC）：同裂隙機轉但有機械剪力跨過鈍化膜，提高腐蝕速率。（Courtesy of Kenneth Urish, MD, PhD, Pittsburgh, PA） -->

### 4.3 三種腐蝕型態 (Pitting, Crevice & MACC)

這三種型態皆屬於**同一連續光譜**，反映合金避免**保護性鈍化層崩解**的能力。

| 型態 | 定義與機轉 | 臨床對應 |
|------|-----------|---------|
| <span style="color:#f87171;font-weight:600">點狀腐蝕（pitting）</span> | 鈍化膜的**細微不一致**導致**小面積**膜崩解，形成**聚焦的陽極**與**局部電偶腐蝕**；遠端大面積表面形成**差異陰極**，兩點間產生**極大電位差**與電流，性質類似**電池兩極的電壓差** | 表面點蝕破壞 |
| <span style="color:#fbbf24;font-weight:600">裂隙腐蝕（crevice）</span> | 發生於**離子擴散受限**環境的點狀腐蝕，形成**腐蝕的理想環境**；全髋 **trunnion** 為**密閉環境** | 頸柄錐狀接點 |
| <span style="color:#60a5fa;font-weight:600">MACC／微動腐蝕（fretting）</span> | **物理剪力**移除保護性鈍化膜，使裂隙腐蝕環境更趨理想、腐蝕面積更大 | 假體鬆動、摩擦界面 |

**裂隙腐蝕的細節**：在頸—頭錐狀接點上，**水密封只在有限的一點建立**，並非涵蓋整個錐狀接觸面；此密封阻止離子擴散 → **氧氣被耗盡**、**再鈍化（repassivation）能力受限** → **氫離子與氯離子濃度上升** → 形成**低 pH 環境**，進一步**加速腐蝕**。

**MACC 的細節**：錐狀表面間可能的**剪力位移**會移除更多鈍化膜；**股骨頭尺寸增大**與**股骨柄偏移增加**會**增加 trunnion 上的力量**，也**提高剪力位移的機會**；缺乏保護膜加上受限擴散環境，構成**侵蝕性腐蝕的理想條件**。

> **Danger zone**：全髋關節 **trunnion 是腐蝕的熱點**——原因包括**液體擴散受限、酸性環境、以及彎曲力矩增加**三者疊加；因此大尺寸股骨頭與長柄設計在評估翻修風險時必須一併納入。

> **Pearl**：**MACC 與 fretting corrosion 實質上是同一個名詞的兩種說法**，二者不可視為兩種不同的腐蝕機轉。

### 4.4 從材料到臨床的整合 (From Material Science to Clinical Practice)

- **疲勞破壞**：循環載荷低於屈服強度即可能致壞 → 植入物斷裂、骨折不癒合。
- **磨損**：UHMWPE 氧化降解降低耐磨性；鈦承載面磨損比 Co-Cr-Mo 多 **15%** → 骨溶解、假體鬆動。
- **應力遮蔽**：骨－植入物**模數不匹配** → 骨吸收、假體下沉與鬆動。
- **點狀／裂隙／MACC 腐蝕**：鈍化膜缺陷、離子擴散受限、機械剪力 → 頸柄處金屬離子釋放與骨溶解。

> **Pearl**：理解生物力學與生物相容性是臨床骨科醫師的有力工具；三者的應用是骨科治療與介入的**核心原理**，也是創新（innovation）的基礎。

---

## 5. 實證更新與 OKU 14 重點 (Recent Evidence & Take-Home Points)

### 5.1 本章要點整理 (Key Study Points)

| 主題 | 要點 |
|------|------|
| **Young 模數** | 用於比較與篩選骨科材料；**骨－植入物模數不匹配**是植入物失效原因之一 |
| **骨的異向性** | 縱向比橫向更強更剛；受壓比受張更強；載荷越快剛度越高 |
| **鈍化膜** | 對防止骨科植入物腐蝕具有關鍵作用 |
| **合金選擇** | **不是因為機械性能（強度）最佳，而是因為耐蝕性最佳** |
| **trunnion** | 因**液體擴散受限、酸性環境、彎曲力矩增加**形成腐蝕的理想環境 |
| **疲勞** | 植入物以循環載荷失效 → 疲勞強度較 UTS 更相關 |
| **黏彈性** | PMMA 骨水泥因**應力鬆弛**而不致達到疲勞破壞應力 |

### 5.2 骨科專科考試核心總結 (Take-Home Points)

1. **剛度不是材料單一屬性**：力－位移斜率同時反映**幾何（慣性矩）**與**材料（彈性模數）**；長骨與長植入物位移更大。
2. **三點與四點彎曲的差別**：三點彎曲最大彎曲力矩在**施力點**；四點彎曲形成**最大力矩區帶**。
3. **UTS 不等於植入物壽命**：植入物以**循環載荷**失效，疲勞強度優先；載荷越快材料越剛（圖 3C）。
4. **黏彈性三現象**：遲滯、蠕變（恆載下變形增加，溫度高則更明顯）、應力鬆弛。
5. **交聯 UHMWPE 的取捨**：1990 年代問世以降低氧化降解，已是全髋事實標準並拓展至全膝；代價是初始模數較高、韌性較低。
6. **骨水泥的定位**：PMMA **不黏著**，靠機械互鎖固定；**受壓強於受張、模數低**；靠應力鬆弛保護植入柄。
7. **合金選擇的真正理由**：耐蝕性與生物相容性，而非強度；鈦延性佳但承載面磨損比 Co-Cr-Mo 多 **15%**。
8. **陶瓷的力學關鍵**：晶粒細小 + 完全致密 → 硬度↑、脆性與斷裂率↓；氧化鋁基質頭 = **75% 氧化鋁 / 24% 氧化鋯 / 1% 氧化鉻**。
9. **耐火金屬**：鋯與鉭（另有鉬、鎢）硬度與耐磨性約 Co、Ti 合金的 **10 倍**；多孔鉭形成羥磷灰石，模數接近海綿骨、初期固定佳。
10. **腐蝕三步驟**：氧化 → 還原（電子流動產生電流）→ 氧化層／氫氧化物產物形成絕緣層。
11. **鈍化膜穩定金屬**：Ti、Cr、Ta、Nb、Zr；Cu、In、Sn 的氧化層遇氯離子迅速溶解。
12. **三種腐蝕是同一光譜**：點狀 → 裂隙（擴散受限、低 pH、低氧）→ MACC／fretting（再加機械剪力破壞鈍化膜，**兩者為同一名詞**）。
13. **trunnion 的三重惡因**：液體擴散受限、酸性環境、彎曲力矩增加；大頭與增加柄偏移提高剪力位移機會。

---

## References

1. Bergmann G, Graichen F, Rohlmann A, et al: Realistic loads for testing hip implants. Bio Med Mater Eng 2010;20:65-75.
2. Lewis GS, Mischler D, Wee H, Reid JS, Varga P: Finite element analysis of fracture fixation. Curr Osteoporos Rep 2021;19:403-416.
3. Schwenke T, Orozco D, Schneider E, Wimmer MA: Differences in wear between load and displacement control tested total knee replacements. Wear 2009;267:757-762.
4. Brach Del Prever EM, Bistolfi A, Bracco P, Costa L: UHMWPE for CR and PS total knee arthroplasties. J Arthroplasty 2008;23:559-566.
5. Bundy K: Bone Prosthesis and Implant Materials. CRC Press Inc, 1989, pp 160-184.
6. Park JB: Biomaterials Science and Engineering. Plenum Press, 1984.
7. Silver FH, Christiansen DL: Biomaterials Science and Biocompatibility. Springer, 1999.
8. Jacobs JJ, Gilbert JL, Urban RM: Corrosion of metal orthopaedic implants. J Bone Joint Surg Am 1998;80:268-282.
9. Breme J, Biehl V: Metallic Biomaterials. Chapman and Hall, 2001, pp 135-214.
10. Black J: Orthopaedic Biomaterials in Research and Practice. Churchill Livingstone, 1988.
11. Black J: Biomaterials. Marcel Dekker, Inc, 1992.
12. Black J: Prosthetic Materials. VCH Publishers, Inc, 1996.
13. Urish KL, Giori NJ, Lemons JE, Mihalko WM, Hallab N: Trunnion corrosion in total hip arthroplasty—basic concepts. Orthop Clin North Am 2019;50:281-288.
14. Hodgson AW, Mischler S, Von Rechenberg B, Virtanen S: An analysis of the in vivo deterioration of Co-Cr-Mo implants through wear and corrosion. Proc Inst Mech Eng H 2007;221:291-303.
15. Szklarska-Smialowska Z; NACE: Pitting Corrosion of Metals. National Association of Corrosion Engineers, 1986.

---

## Summary

- <span style="color:#60a5fa;font-weight:600">剛度是幾何 × 材料</span>：力－位移斜率受慣性矩與彈性模數共同決定；長骨與長植入物位移更大；複雜幾何需**有限元素模型**。
- <span style="color:#60a5fa;font-weight:600">彎曲試驗</span>：懸臂（固定端最大力矩）、三點（施力點最大力矩 + 剪力）、四點（**最大力矩區帶**）。
- <span style="color:#60a5fa;font-weight:600">應力—應變曲線</span>：彈性區 → 屈服點 → 塑性區（應變硬化）→ 極限抗拉強度（伴隨頸縮）→ 破壞；**載荷速率越快越剛**。
- <span style="color:#f87171;font-weight:600">疲勞優先於 UTS</span>：植入物以循環載荷失效；疲勞破壞可在**低於屈服強度**時發生，且為脆性。
- <span style="color:#60a5fa;font-weight:600">黏彈性</span>：遲滯（載荷段高於卸載段）、蠕變（恆載下變形增加，溫度高則更明顯）、應力鬆弛（定應變下應力下降，使骨水泥柄免於疲勞破壞）。
- <span style="color:#60a5fa;font-weight:600">測試模式</span>：靜態載荷評估剛度；動態載荷評估磨損與疲勞；**載荷控制 vs 位移控制**給出不同磨損結果。
- <span style="color:#60a5fa;font-weight:600">UHMWPE</span>：1960 年代起之承載面材料；高結晶度帶來高模數、屈服強度、抗蠕變與疲勞強度；**氧化**降低耐磨性 → 1990 年代**高度交聯**成為全髋事實標準並拓展至全膝。
- <span style="color:#60a5fa;font-weight:600">PMMA 骨水泥</span>：**不黏著**，靠機械互鎖固定；受壓強於受張、模數低；溫度升高蠕變增加。
- <span style="color:#60a5fa;font-weight:600">合金選擇</span>：依**耐蝕性與生物相容性**而非強度；Ti（延性、多孔塗層）、Co-Cr（承載面）、不鏽鋼 316L（骨折固定）。
- <span style="color:#f87171;font-weight:600">鈦的弱點</span>：Ti-6Al-4V 比 Co-Cr-Mo **約軟 15%**，承載面磨損**多 15%**，故不作為耐磨首選。
- <span style="color:#60a5fa;font-weight:600">陶瓷</span>：晶粒細小 + 完全致密 → 硬度↑、脆性與斷裂率↓；氧化鋁基質股骨頭 = **75% 氧化鋁、24% 氧化鋯、1% 氧化鉻**（粉紅色來自氧化鉻）。
- <span style="color:#60a5fa;font-weight:600">鋯與鉭</span>：耐火金屬，硬度與耐磨性約 Co、Ti 合金的 **10 倍**；多孔鉭形成羥磷灰石，模數接近海綿骨、摩擦係數高、初期固定佳。
- <span style="color:#f87171;font-weight:600">腐蝕三步驟</span>：氧化（陽離子溶出）→ 還原（電子流動產生電流）→ 氧化層／鏽層形成絕緣層；**鈍化膜是防止腐蝕的關鍵**。
- <span style="color:#f87171;font-weight:600">鈍化穩定金屬</span>：Ti、Cr、Ta、Nb、Zr；Cu、In、Sn 的氧化層遇氯離子迅速溶解。
- <span style="color:#f87171;font-weight:600">腐蝕光譜</span>：點狀（膜缺陷→聚焦陽極→遠端差異陰極）→ 裂隙（擴散受限、低 pH、低氧）→ **MACC = fretting**（再加機械剪力破壞鈍化膜）。
- <span style="color:#f87171;font-weight:600">trunnion</span>：液體擴散受限、酸性環境、彎曲力矩增加，构成腐蝕理想環境；**大尺寸股骨頭與增加柄偏移**提高剪力位移與 MACC 風險。
