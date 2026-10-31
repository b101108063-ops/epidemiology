---
title: "Chapter 14: Musculoskeletal Mechanics and Kinesiology（肌肉骨骼力學與動作學）"
date: 2026-10-31
draft: false
tags: ["Orthopaedics", "OKU14", "Biomechanics", "Translational Science"]
categories: ["General Topics"]
weight: 14
summary: "本章依序介紹自由體圖與平衡方程式的應用、骨與肌腱韌帶的組織力學、髖與膝關節在步態中的六自由度運動學與接觸路徑，並說明動作捕捉、肌肉骨骼建模、雙平面透視成像與可穿戴裝置四大臨床技術及其侷限。"
---

# Chapter 14: Musculoskeletal Mechanics and Kinesiology — 肌肉骨骼力學與動作學

**章節導讀**：本章屬「轉譯科學與新興技術」單元，核心在於把生物力學與動作學的基礎原理，轉譯成可量測、可驗證的臨床工具。全章先以自由體圖與平衡方程式建立「如何算」的框架，再由骨、肌腱與韌帶的材料力學說明「組織如何受力」，接著以髖、膝關節的步態運動學連結「關節如何動」，最後介紹動作捕捉、肌肉骨骼建模、雙平面透視（dual fluoroscopy）與可穿戴裝置四大臨床應用，並點出各自的方法學限制與證據等級。

---

## 1. 核心概念與力學分析框架 (Core Concepts & Analytical Framework)

本章非解剖學章節，其「關鍵結構」係指**力學分析的基本單位與工具鏈**：從自由體圖（free-body diagram）、平衡方程式、到生物力學模型，構成一條可追溯、可驗證的推論路徑。

### 1.1 自由體圖與平衡方程式（Free-Body Diagrams & Equilibrium）

自由體圖用來辨識作用於肌肉骨骼系統某一節段（segment）上的**所有力與力矩（forces and moments）**；建立後即可用平衡方程式求解未知的近端力。

| 符號 | 意義 |
|------|------|
| `I` | 轉動慣量（moment of inertia） |
| `a` | 角加速度（angular acceleration） |
| `g` | 重力加速度（gravitational acceleration） |
| `m`、`a` | 分段質量（segmental mass）與線加速度（linear acceleration） |
| 下標 `g`／`k`／`a`／`h` | ground（足部）、knee（膝）、ankle（踝）、hip（髖） |
| `F` | 力（force） |
| `T` | 合力矩（resultant torque） |

沿 y 方向分析前臂平衡，可得：

```
R_F = F_B − W_F − W_O
```

> **Pearl**：求解順序是**由遠端往近端**推進——先從足部開始。小腿遠端的力與力矩，等於反向的踝關節力與力矩；知道小腿遠端的力與力矩後，才能求出小腿近端的力與力矩。

**數值範例（依原文參數）**：若 `a` = 4 cm、`b` = 15 cm、`c` = 35 cm、`W_O` = 80 N、`W_F` = 20 N，則可得 `F_B` = **775 N**、`R_F` = **675 N**。

> **Pearl**：自由體圖亦可用來計算不同關節在移動過程中的**節段間外力與力矩（intersegmental forces and moments）**。這正是後續步態運動學與關節接觸力估算的基礎。

<!-- FIG: Figure 4 — 下肢自由體圖。A, 慣性屬性（inertial properties）；B, 節段間力與力矩（intersegmental forces and moments）。 -->

### 1.2 從靜力學到動態量測的落差

<!-- FIG: 圖 8 — illustration shows contact path motion of the medial tion of these tec -->

<!-- FIG: 圖 7 — Graphs show kinematics of the knee during the gait extremities are hig -->

自由體圖屬於**模型驅動**的分析；要回答「活體上真實的負荷是多少」，必須引入實驗量測的驗證流程。模型數值輸出必須經過**充分的驗證與確認（validation and verification）**才具有臨床效用，而儀器化植入物與遙測正是此類驗證的主要手段。

> **Danger zone（解讀陷阱）**：缺乏獨立驗證的模型結果，僅為假設生成器，不可直接作為臨床決策依據。

---

## 2. 分型系統與組織力學 (Classification & Tissue Mechanics)

<!-- FIG: 圖 10 — Illustration shows optical motion capture experimental setup including -->

<!-- FIG: 圖 9 — Graph shows hip joint contact force during gait. -->

### 2.1 骨組織的階層結構與材料性質

骨是肌肉骨骼系統中含量最多的組織，其組成比例為：

| 組成成分 | 比例 | 功能角色 |
|----------|------|----------|
| 無機質（hydroxyapatite，羥磷灰石） | **40%** | 承載時提供**壓縮（compressive）**行為 |
| 有機基質（type I collagen，I 型膠原） | **35%** | 在骨的**張力（tensile）**性質中扮演主要角色 |
| 水 | **25%** | — |

**微觀階層結構**：骨在微米（micrometer）層級由**礦化的膠原纖維（mineralized collagen fibrils）**構成，嵌於有機細胞外基質中；纖維排列成**骨板（lamellae）**，厚度 **7–10 µm**；大量骨板環繞中央的哈弗氏管（haversian canal）形成**哈弗氏系統／骨單位（osteon）**，直徑約 **200 µm**。骨板與骨單位再在更高層級（大於 1 mm）構成**皮質骨（cortical bone）**與**海綿骨／小梁骨（cancellous bone）**。

| 類型 | 結構特徵 | 力學特性 |
|------|----------|----------|
| **皮質骨**（cortical bone） | 縱向排列的骨板與骨單位 | **異向性（anisotropic）**：縱向受力比橫向更 resists；**黏彈性（viscoelastic）**：隨載入速率改變剛度與強度 |
| **海綿骨**（cancellous bone） | 開放的細胞狀結構，小梁與支柱微結構多变 | 材料性質取決於**表觀密度（apparent density）**，以線性或指數關係量化 |

> **Pearl**：皮質骨在**壓縮**方向比在**張力**方向更強；載入速率越快，剛度越高但**破壞應變（failure strain）下降**。這對老年骨質疏鬆患者的跌倒衝擊傷害有直接意義。

> **Pearl**：日常功能活動（步行、跑步）使皮質骨**主要在縱向**受到最大負荷，因此縱向的抗力表現最具臨床意義。

<!-- FIG: Figure 5 — 骨的應力－應變曲線（stress-strain curve），標示 ultimate strength、yield strength、fracture 與 Young's modulus E。 -->

### 2.2 肌腱與韌帶力學（Tendon & Ligament Mechanics）

<!-- FIG: 圖 1 — Schematic representation of fracture repair. On fracture induction (mi -->

肌腱與韌帶的機械行為**相似但功能不同**：韌帶連接骨與骨以提供關節穩定；肌腱連接肌肉與骨，將肌肉產生的力量傳遞至骨骼以促成運動。

| 成分 | 肌腱 | 韌帶 |
|------|------|------|
| **Type I collagen**（占乾重） | 75%–80% | 75%–80% |
| **Proteoglycans**（蛋白聚醣，占乾重） | 1%–3% | 1%–3% |
| **Elastin**（彈性蛋白，占乾重） | **< 3%** | **10%–15%** |
| 膠原纖維排列 | 沿受力方向**均勻對齊** | 排列較不具結構性，反映韌帶承受更多變化的載入條件 |

兩者皆為**高度水合**，且機械性質呈**異向性**。

**張力載入下的非線性行為**：
1. **Toe region（趾區）**：低負荷時產生高變形量，纖維重新排列（fiber realignment）。
2. **Linear region（線性區）**：排列後的纖維承擔負荷，繼續伸長直至屈服與破壞。

> **Danger zone（概念陷阱）**：肌腱與韌帶的剛度排序為「**骨 > 肌腱／韌帶 > 軟骨**」；但韌帶的彈性蛋白比例較高並不代表其整體強度較高，切勿由單一成分比例推論整體機械性質。

---

## 3. 髖與膝關節的運動學與植入物力學 (Joint Kinematics & Implant Mechanics)

### 3.1 三個解剖平面與關節自由度

髖與膝皆為**滑膜關節（diarthrodial joints）**，允許關節面在滑膜腔內相對移動。關節運動在三個互相垂直的解剖平面上定義：

| 平面 | 旋轉定義 |
|------|----------|
| **冠狀面（coronal／frontal）** | 外展（abduction，腿離開身體中心）／內收（adduction，腿移回身體中心） |
| **矢狀面（sagittal／longitudinal）** | 屈曲（flexion，髖向前旋轉）／伸展（extension，髖向後旋轉回伸直位） |
| **橫斷面（transverse／horizontal）** | 內旋（internal rotation，繞縱軸朝身體中心旋轉）／外旋（external rotation，繞縱軸向外旋轉） |

| 關節 | 平移自由度 | 旋轉自由度 | 合計 |
|------|------------|------------|------|
| **髖關節** | 3 | 3（屈伸、內外展、內外旋） | **6 自由度（six degrees of freedom）** |
| **膝關節** | 3（三個解剖方向的關節面平移） | 3 | **6 自由度** |

> **Pearl**：目前的人工關節設計（total joint arthroplasty）保留上述自由度，以恢復關節功能。

### 3.2 步態中的髖關節旋轉

步態週期分為**站立期（stance phase）**與**擺動期（swing phase）**：站立期約佔步態週期 **60%**，自**足跟著地（heel strike）**開始至**足尖離地（toe-off）**結束；擺動期約佔 **40%**，自 toe-off 開始至下一次 heel strike 結束。

| 參數 | 數值／描述 |
|------|-----------|
| 矢狀面髖伸展 | 站立期內伸展近 **35°**，之後於擺動期屈曲回來 |
| 外展／內收角度 | 全步態週期覆蓋約 **10°** 範圍 |
| 內旋／外旋角度 | 全步態週期覆蓋約 **10°** 範圍 |
| 站立期前半 | 以**髖外展與內旋**為主 |
| 站立期後半 | 以**髖內收與外旋**為主，使關節回到平衡位置 |

> **Pearl**：髖為**球窩關節（ball-and-socket）**，故髖旋轉必然伴隨**股骨頭相對髖臼的相對滑動（relative sliding）**。在日常功能活動中，最大滑動需求出現在**屈曲／伸展旋轉**。

<!-- FIG: Figure 6 — 步態中髖關節旋轉的圖表（flexion/extension、abduction/adduction、internal/external rotation 對應 stance 與 swing phase）。 -->

### 3.3 步態中的膝關節運動學

膝關節在功能性活動中的複雜運動已有多項研究，其中以屈伸、內外旋、前後平移為代表（圖 7 數據來自病人平均值，並用於程式化膝關節模擬器以評估人工膝關節的磨耗型態）。

| 階段 | 膝屈曲角度 | 脛骨相對股骨運動 |
|------|------------|------------------|
| 足跟著地（heel strike） | 幾乎完全伸直 | 略有旋轉 |
| 站立期前 50% | 最高可達 **20°** 屈曲 | **內旋 + 前方平移** |
| 站立期後 50% | 幾乎完全伸直 | **外旋 + 後方平移** |
| 擺動期 | 可出現近 **60°** 屈曲，隨後回到完全伸直以迎接下一週期 | — |

> **Pearl**：**最大的負荷與接觸應力出現在站立期**（腿與地面接觸的階段）。

### 3.4 滾動與滑動：接觸路徑的移動

由於功能日常活動中膝旋轉與平移的複雜交互作用，膝關節同時出現**滾動（rolling）與滑動（sliding）**。因此，人工膝關節的脛骨與股骨元件之**接觸位置會隨功能活動而移動**；接觸位置的精確變化高度取決於**關節面（articulating surface）設計**。

| 項目 | 說明 |
|------|------|
| 內側髁接觸路徑 | 通常呈狹窄的 **「8」字形** |
| 外側髁接觸路徑 | 同樣呈狹窄的 **「8」字形** |
| 內側與外側髁路徑差異 | 有差異，有利於股骨元件相對脛骨元件的**內旋／外旋** |
| 相對參考 | 人工膝關節的接觸路徑以**聚乙烯襯墊（polyethylene liner）**的脛骨元件為基準描述 |


---

## 4. 臨床應用與新興技術 (Clinical Applications & Emerging Technologies)

### 4.1 遙測與儀器化植入物（Telemetry & Instrumented Implants）

肌肉骨骼模型的數值輸出，必須經**充分的驗證與確認**才具臨床效用；驗證方法包括儀器化植入物，以及以**遙測方式傳輸負荷、應變或壓力資料**。

| 關節 | 常見實驗方法 | 來源 |
|------|--------------|------|
| **髖關節** | 貼附於髖關節置換物**股骨頸**的**應變計（strain gauge）**；訊號傳至接收器後分析作用於股骨頭的力 | Rydell NW（1966）|
| **膝關節** | 數量有限的研究測試**儀器化膝植入物（股骨遠端）**，以遙測傳輸量測資料 | Taylor SJ, Walker PS（2001）|
| **膝關節（另一策略）** | 將**脛骨側膝假體**儀器化，量測功能任務期間的膝負荷 | — |

**Pearl**：**OrthoLoad**（https://orthoload.com/）提供多關節置換（髖、膝、肩、脊柱）與多種功能任務最完整的活體負荷資料庫。

**活體關節負荷量級**：

| 部位 | 活體負荷（相對體重） |
|------|--------------------|
| 肩關節 | 達 **1–2 倍體重** |
| 下肢關節（日常活動） | 更高，常達**數倍體重** |
| 髖與膝（跑步、跳躍等劇烈活動） | 最高達 **2–8 倍體重** |

**表 1：功能日常活動期間之髖關節接觸力峰值**

| 功能活動 | 最大髖關節力（體重倍數） | 參考文獻 |
|----------|--------------------------|----------|
| 平地慢走（slow level walking） | 4.8 | Paul (1976) |
| 平地慢走 | 2.4 | Bergmann et al (2001) |
| 平地正常走 | 2.3 | Bergmann et al (2001) |
| 平地正常走 | 3.0–3.3 | Prendergast et al (2005) |
| 平地快走（fast level walking） | 7.5 | Paul (1976) |
| 平地快走 | 2.5 | Bergmann et al (2001) |
| 下坡行走 | 5.1 | Paul (1976) |
| 上坡行走 | 5.9 | Paul (1976) |
| 下樓梯 | 7.2 | Paul (1976) |
| 下樓梯 | 2.6 | Bergmann et al (2001) |
| 上樓梯 | 2.4 | Bergmann et al (2001) |
| 上樓梯 | 2.8–3.2 | Prendergast et al (2005) |

> **Danger zone（數值解讀陷阱）**：同一活動在不同參考文獻間可相差數倍（如快走 7.5 vs. 2.5；上樓梯 2.4 vs. 2.8–3.2）。差異反映**測量方法、假設與個體差異**，引用時必須連同參考文獻一併標示，不可混用或取平均。

### 4.2 動作捕捉技術（Motion Capture Technology）

動作捕捉技術結合上、下肢的**計算式肌肉骨骼模型（computational musculoskeletal models）**，對肌肉骨骼疾病患者的臨床決策具有極大潛力，可提供肌肉力與關節接觸力等**臨床高度相關但活體難以測量**的變數（若要實測，需在肌腱內植入感測器或植入儀器化關節置換物）。

| 面向 | 內容 |
|------|------|
| **追蹤方式** | 感光感測器（optical）或非感光感測器：**慣性、磁力、伸展、聲學** |
| **研究與臨床工業主流** | 感光感測器——使用**逆反射材料**標記，因其**便宜、可靠且易用** |
| **追蹤設備** | 紅外線相機；擷取率**至少為目標動作頻率的 2 倍**，以避免誤差 |
| **相機數量** | 系統通常由 **5–10 具紅外線相機**組成，以取得受測者的 **360°** 視野 |
| **最小可追蹤條件** | 至少需 **3 具**相機能捕捉同一標記，才能準確追蹤該體節的運動 |
| **標記位置** | 放置於特定**解剖位置（骨性標誌）**，用以建立各體節的**座標框架（coordinate frames）** |
| **標誌來源** | **International Society of Biomechanics（ISB）**建立的解剖標誌，具高可靠性與準確性 |

| **臨床與研究應用** | 評估**矯具（orthoses）**、協助**外科決策**、協助**新的復健方案**開發、設計**新的外科介入**、協助**新的關節置換物**開發。 |

| **臨床與研究應用** | 評估**矯具（orthoses）**、協助**外科決策**、協助**新的復健方案**開發、設計**新的外科介入**、協助**新的關節置換物**開發。 |

### 4.3 肌肉骨骼建模（Musculoskeletal Modeling）

上、下肢關節的肌肉骨骼模型，是估算移動過程中肌肉骨骼系統負荷的**計算工具**：以動作捕捉資料為輸入，計算完成所記錄動作所需的**肌肉力**，以及伴隨的**關節接觸力**。

**模型建構要素**

| 要素 | 說明 |
|------|------|
| **骨骼系統** | 由所有人體骨性體節與所有肌肉附著點構成 |
| **骨骼解剖與肌肉形態** | 常用**屍體解剖與數位化**取得，用以參數化模型 |
| **肌肉表示法** | 以繞過**類似關節之幾何物體**的**緊繃繩索**表示 |
| **個體化縮放** | 依**身高與體重**將通用骨骼幾何縮放至個別受試者 |
| **進階個體化** | 近期研究運用**醫學影像與統計形狀建模**進行縮放，以提升臨床適用性 |

**逆動力學（inverse dynamics）與負荷分擔最佳化（load-sharing optimization）**

1. 逆動力學使用**牛頓方程式**，計算所記錄動作資料**每一時間格（time frame）**的節段間力與力矩。
2. 隨即進行負荷分擔最佳化，確保計算所得的肌肉力與合力關節接觸力與逆動力學的計算結果處於**平衡狀態**。
3. 負荷分擔最佳化**通常最小化肌肉應力的平方和**，以確保跨越關節的所有肌肉都被活化，整體目標是**最小化能量消耗**。

**驗證方式**：上、下肢肌肉骨骼模型已對照**儀器化植入物量測**、**肌電圖（EMG）量測**，以及**屍體標本的肌肉力臂（muscle moment arms）量測**進行驗證。

**臨床應用**

| 類別 | 具體研究內容 |
|------|--------------|
| **非手術治療** | 肉毒桿菌毒素對**股直肌（rectus femoris）**力量的影響；**雄性激素去除療法（androgen deprivation therapy）**對偏癱（hemiparetic）病人步行中垂直穩定相關肌肉使用量的影響 |
| **矯具** | 以**關節接觸力**評估**鞋墊（insoles）、外側足楔（lateral foot wedges）、膝支架（knee braces）**對膝骨關節炎的治療效果 |
| **外科介入** | **前十字韌帶重建（ACL）**後病人的預後；改變關節負荷所引起骨關節炎的發生 |
| **運動與復健** | 評估運動與復健策略在**改善關節接觸力與肌肉負荷**上的效果 |

| **運動與復健** | 評估運動與復健策略在**改善關節接觸力與肌肉負荷**上的效果 |

### 4.4 雙平面透視成像系統（Dual Fluoroscopy, DFIS）

<!-- FIG: 圖 11 — Illustration depicts a musculoskeletal shoulder model tillator and con -->

**透視的物理原理**：透視提供即時、互動式的 X 射線投影影像，常使用**影像增強管（image intensifier）**，藉**防散射光柵（antiscatter grid）**移除散射輻射後偵測 X 射線圖型。X 射線由**碘化銫（CsI）閃爍體**捕捉並轉換為光光子，再導向閃爍體背面的**光陰極（photocathode）**。

| 參數 | 數值／說明 |
|------|-----------|
| 光陰極與陽極間電壓 | **> 20,000 V**，產生並加速電子 |
| 電子束聚焦 | 由**電磁聚焦線圈**維持，並將大面積電子分布縮小至光陰極面積 |
| 影像放大 | **> 5,000 倍** |
| 影像擷取 | **每秒 30 影格**；X 射線管可用連續電流或間歇電流，後者可產生一連串投影影像並**降低整體輻射曝露** |
| 顯示 | 電視攝影機偵測光型並顯示於螢幕 |

**DFIS 的建置流程**

1. 先以 **CT 掃描**建立病人關節的**3D 主體特異（subject-specific）骨性解剖模型**；同時產生關節置換物的 3D 模型，以獲得包含人工關節的**病人化 3D 骨性解剖重建**。
2. 骨性解剖與關節置換物皆依 **ISB** 指派**解剖座標框架**。
3. 採用 **3D 鏡像技術（3D mirroring technique）** 指派手術側關節的解剖座標系，使**術側殘餘骨與未手術側鏡像之間的表面對表面配準誤差最小化**。
4. 依指派的局部座標框架，以 **Cardan 角度序列（Cardan angle sequences）**計算關節旋轉。
5. 病人於兩台互相正交的透視裝置監測下執行日常功能任務；**兩台透視同步擷取，常見為 30 Hz**，產生正交角度的串聯影像（tandem view）。
6. 將透視影像與 3D 模型處理，使 3D 模型**虛擬對位**至正交透視影像中所見的病人解剖輪廓，產生一系列描繪病人在該活動中運動的 **3D 影像**。

**準確度與輻射劑量**

| 項目 | 數值 |
|------|------|
| 平移誤差 | **< 0.9 mm** |
| 旋轉誤差 | **< 0.6°** |
| 比較基準 | 與**金標準 radiostereometric analysis** 相當 |
| 輻射曝露 | DFIS 固有上高於 radiostereometric 方法，但現行技術維持於 **5–6 mSv** |

**臨床發現（DFIS 的最重要結論）**

| 議題 | 研究結論 | 證據等級 |
|------|----------|----------|
| 整體 | 儘管現今髖、膝人工關節**有潛力恢復健康關節運動學**，實際上**並未在功能性劇烈活動中完全恢復**健康關節運動學 | — |
| 機器人輔助 THA | 機器人輔助式全髖關節置換可獲得**更高的植入物位置精度**，但**未轉化為顯著改善的活體運動學** | III |
| 機器人輔助 THA（步態） | 恢復原生髖幾何的精度提升，**並未完全轉化為更好的步態對稱性** | III |
| 手術入路 | 前、外側與後側入路 THA 之**活體運動學存在差異** | — |
| BCR TKA（雙交叉韌帶保留） | 持續屈曲活動中可見**非對稱股骨 rollback、內側平移與外側 pivot**，約半數病人族群呈現；**活體脛股運動學參數未完全恢復** | III |
| BCR TKA（接觸路徑） | 步態中**矢狀面運動與脛股接觸特性未完全恢復**，前後平移與 varus 旋轉則與正常膝無顯著差異 | III |
| 保留交叉韌帶 TKA | 劇烈活動下仍持續存在**非對稱接觸運動學** | III |
| 性別差異 | 單側 BCR TKA 病人膝關節存在 3D 步態不對稱，**前後向的肢間不對稱在女性顯著大於男性** | III |
| 病理狀態 | cam 型股骨髖臼撞擊症候群、盂唇損傷、ACL 重建等病人，即使在**次最大活動範圍**中也可能改變骨盆運動 | IV |

> **Pearl**：機器人與客製化植入物的「幾何還原更準確」與「功能與步態更接近原生」是**兩個不同的命題**，前者成功並不代表後者成立。

<!-- FIG: Figure 12 — 透視成像系統示意（monitor、video camera、image intensifier、grid、patient、table、filtration、collimator、X-ray tube、X-ray generator）。 -->
<!-- FIG: Figure 13 — 由 CT 影像重建之單側全膝關節置換 3D 膝關節模型。 -->
<!-- FIG: Figure 14 — DFIS 設置。A, 動態活動下的 DFIS；B, 影像配準。 -->

### 4.5 可穿戴裝置（Wearable Devices）

可穿戴技術指所有**可佩戴於人體**的裝置。自數十年前手錶問世以來，此概念持續受到高度關注，並在**技術驅動型國家**日益普及。裝置蒐集資料並透過監測介面傳送給使用者。骨科醫師對其興趣主要來自**健身追蹤的成功先例**，以及其**簡化醫病溝通、優化病人照護、並可能降低攀升中的醫療成本**的潛力。

| 面向 | 內容 |
|------|------|
| **一般手腕裝置追蹤的資料** | **心率、活動量、睡眠型態、營養資訊** → 提供病人**基線（baseline）**評估，協助發展**病人特異治療計畫**，並讓病人**客觀回報結果** |
| **術後** | 可監測**術後恢復期的任何變化**，並指導**個人化物理治療方案** |
| **已證實效益** | 改善病人對**治療計畫、復健方案與自我管理**的**遵循度（adherence）** |
| **骨科專屬量測** | **活動範圍（ROM）、步幅長度、骨盆旋轉** → 可量化**疾病嚴重度**、監控**預後**、追蹤**復原過程** |
| **具體應用** | **脊椎狹窄**病人行動能力量化以偵測**步行耐受度惡化**；**中風**病人術後恢復監控；**ACL 重建**後 ROM 監控以確保遵守復健活動限制 |
| **遠端監控的價值** | 資料可**無線傳輸給醫師**，醫師可即時實施**預防性介入（preventative intervention）**以優化預後並**降低醫療成本** |

**四大採用障礙**

| 障礙 | 內容 |
|------|------|
| **年齡動態** | 老年人對可穿戴技術的**興趣增加**，但先前研究顯示其在老年人中的**整體使用率仍有限** |
| **成本** | 部分裝置**價格達數百美元**，可能**造成病人照護的分層**；研究顯示整體滿意度高，但**高成本是造成不滿的主要因素** |
| **安全** | 消費性產品**往往缺乏標準化的安全與使用者認證規範**；**保護病人機密資訊**仍是重大挑戰 |
| **效度（validity）** | 一項比較多種可穿戴裝置量測身體活動的研究，報告**準確度差異可高達 25%** |

> **Danger zone（臨床採用陷阱）**：可穿戴裝置的**量測效度不足**是根本問題；在不同品牌／演算法間數值不可直接互換，須先確認量測參數的效度與校正方式，才能用於臨床判讀。

---

## 5. 實證更新與 OKU 14 重點 (Recent Evidence & Take-Home Points)

### 5.1 核心研究要點（Key Study Points）

- **自由體圖（free-body diagrams）** 用於辨識作用於肌肉骨骼系統某一節段上的**所有力與力矩**。
- **遙測（telemetry）** 透過**儀器化植入物**的應用，為量測關節**活體負荷（in vivo loading）**提供有效工具。
- **動作捕捉技術與肌肉骨骼建模** 透過對動作的**計算分析**，提供肌肉與關節負荷的深入見解。
- **雙平面透視（dual fluoroscopy）** 透過將髖、膝的**電腦輔助設計（CAD）模型投影**與**動態透視影像**作最佳匹配，可準確評估**活體關節置換物運動學**。
- **可穿戴裝置** 佩戴於人體，用以研究肌肉骨骼系統的**外部參數**，例如**活動範圍**。

### 5.2 章節總結（Summary）

理解**生物力學與動作學的基本原理**——包括作用於肌肉骨骼系統之**力的分析**、**骨、肌腱與韌帶力學**，以及**髖與膝關節的生物力學**——是必要的。肌肉骨骼生物力學的應用包含**動作捕捉技術、雙平面透視成像系統與可穿戴技術**，它們使骨科醫師能夠評估人體上下肢**關節與關節置換物的表現**。

### 5.3 骨科專科考試核心總結（Take-Home Points）

1. **先算後驗**：所有活體負荷數字都建立在自由體圖與平衡方程式之上（如 `R_F = F_B − W_F − W_O`；範例參數得 `F_B` = 775 N、`R_F` = 675 N），解算順序為**由遠端往近端**。
2. **骨的材料性質速記**：**40% 無機質（hydroxyapatite）／35% 有機基質（I 型膠原）／25% 水**；骨板 **7–10 µm**、骨單位直徑約 **200 µm**；皮質骨**縱向強於橫向、壓縮強於張力**，且**載入越快越硬但破壞應變越小**。
3. **腱與韌帶速記**：I 型膠原占乾重 **75%–80%**、蛋白聚醣 **1%–3%**；**韌帶彈性蛋白 10%–15%，肌腱 < 3%**；張力曲線有 **toe region → linear region** 兩段。
4. **自由度**：髖與膝皆為 **6 自由度**（3 平移 + 3 旋轉）；步態站立期約 **60%**、擺動期約 **40%**；站立期前半髖**外展＋內旋**，後半**內收＋外旋**；膝在站立期前 50% 屈曲至多 **20°**，擺動期可達近 **60°**。
5. **負荷量級**：肩關節活體負荷達 **1–2 倍體重**；髖與膝在跑步、跳躍等劇烈活動可達 **2–8 倍體重**（表 1）。
6. **技術與陷阱**：動作捕捉需 **5–10 具紅外線相機**、每個標記至少 **3 具相機**可見、擷取率至少為目標頻率 **2 倍**；DFIS 誤差 **< 0.9 mm / < 0.6°**、輻射 **5–6 mSv**；可穿戴裝置準確度差異可達 **25%**，並有成本、資安、老年人使用率三大障礙。
7. **臨床現實**：現今髖、膝人工關節**未在劇烈活動中完全恢復健康運動學**；機器人輔助 THA 提高定位精度，卻**未轉化為更好的步態對稱性**。

---

## 參考文獻

1. Reilly DT, Burstein AH: The elastic and ultimate properties of compact bone tissue. J Biomech 1975;8(6):393-405.
2. McElhaney JH, Fogle JL, Melvin JW, et al: Mechanical properties of cranial bone. J Biomech 1970;3(5):495-511.
3. Rice JC, Cowin SC, Bowman JA: On the dependence of the elasticity and strength of cancellous bone on apparent density. J Biomech 1988;21(2):155-168.
4. Silver FH, Freeman JW, Bradica G: Structure and function of ligaments, tendons, and joint capsule. In Walsh WR, ed: Repair and Regeneration of Ligaments, Tendons, and Joint Capsule. Humana Press, 2006, pp 15-47.
5. Peng Y, Arauz P, Desai P, Byers A, Klemt C, Kwon Y-M: In vivo kinematic analysis of patients with robotic-assisted total hip arthroplasty during gait at 1-year follow-up. Int J Med Robot 2019;15(5):e2021.
6. Bergmann G, Deuretzbacher G, Heller M, et al: Hip contact forces and gait patterns from routine activities. J Biomech 2001;34(7):859-871.
7. Rydell NW: Forces acting on the femoral head-prosthesis. A study on strain gauge supplied prostheses in living persons. Acta Orthop Scand 1966;37(suppl 88):1-132.
8. Taylor SJ, Walker PS: Forces and moments telemetered from two distal femoral replacements during various activities. J Biomech 2001;34(7):839-848.
9. Klemt C, Prinold JA, Morgans S, et al: Analysis of shoulder compressive and shear forces during functional activities of daily life. Clin Biomech (Bristol, Avon) 2018;54:34-41.
10. Prinold JA, Masjcdi M, Johnson GR, Bull AM: Musculoskeletal shoulder models: A technical review and proposals for research foci. Proc Inst Mech Eng H 2013;227(10):1041-1057.
11. Smith SHL, Coppack RJ, van den Bogert AJ, et al: Review of musculoskeletal modelling in a clinical setting. Clin Biomech 2021;83:105292.
12. Klemt C, Nolte D, Ding Z, et al: Anthropometric scaling of anatomical datasets for subject-specific musculoskeletal modelling of the shoulder. Ann Biomed Eng 2019;47(4):924-936.
13. Wu G, van der Helm FCT, Veeger HEJD, et al: ISB recommendation on definitions of joint coordinate systems of various joints for the reporting of human joint motion—part II. J Biomech 2005;38(5):981-992.
14. Brandon SCE, Brown MJ, Clouthier AL, et al: Contributions of muscles and external forces to medial knee load reduction due to osteoarthritis braces. Knee 2019;26(3):564-577.
15. Tsai T-Y, Li J-S, Wang S, et al: A novel dual fluoroscopic imaging method for determination of THA kinematics: in vitro and in-vivo study. J Biomech 2013;46(7):1300-1304.
16. Petis S, Howard J, Lanting B, et al: Comparing the anterior, posterior and lateral approach: gait analysis in total hip arthroplasty. Can J Surg 2018;61(1):50-57.
17. Tsai T-Y, Liow MHL, Li G, et al: Bi-cruciate retaining total knee arthroplasty does not restore native tibiofemoral articular contact kinematics during gait. J Orthop Res 2019;37(9):1929-1937.
18. Lee J-M, Kim Y, Welk GJ: Validity of consumer-based physical activity monitors. Med Sci Sports Exerc 2014;46(9):1840-1848.
