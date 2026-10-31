---
title: "Chapter 19: Applications of Three-Dimensional Technologies in Orthopaedic Surgery (骨科手術三維度技術的應用)"
date: 2026-10-31
draft: false
tags: ["Orthopaedics", "OKU14", "3D Printing", "Robotics", "Emerging Technology"]
categories: ["General Topics"]
weight: 19
summary: "本章介紹三維列印、電腦導航與機器人輔助手術、自訂植入物、術中三維影像、生物列印與四維列印及擴增實境等新興技術在骨科的應用，涵蓋個人化器械與術前規劃流程、各技術的臨床效益與證據層級，以及監管核准、學習曲線與手術時間延長等爭議與陷阱。"
---

# Chapter 19: Applications of Three-Dimensional Technologies in Orthopaedic Surgery — 骨科手術三維度技術的應用

## 章節導讀

本章屬於「轉譯科學與新興技術」範疇，而非傳統解剖學章節。本章依原文脈絡回顧 <span style="color:#e2e8f0">3D printing</span>、<span style="color:#e2e8f0">computer navigation</span>、<span style="color:#e2e8f0">robotics</span>、自訂植入物、術中三維影像、<span style="color:#e2e8f0">bioprinting</span>／<span style="color:#e2e8f0">4D printing</span> 與 <span style="color:#e2e8f0">augmented reality</span> 在骨科的應用現況與證據層級。核心訊息是：3D 技術正以穩定步調進展，未來數年將聚焦於醫院內 <span style="color:#fbbf24">point-of-care printing center</span>、FDA 對自訂植入系統的核准，以及機器人手術的接受與標準化。

---

## 1. 核心概念與背景：骨科 3D 技術的應用版圖

本章非解剖學章節，「核心概念」係指三維技術在骨科應用中的**技術類別**、**工作流程**與**臨床定位**；骨科醫師在評估任何一項新技術時，必須先辨識它屬於「術前規劃工具」「術中執行工具」還是「植入物本體」，三者帶來不同的風險與法規路徑。

### 1.1 個人化器械與術前規劃（Patient-Specific Instrumentation）

3D 列印器械用於**矯正畸形**。這些器械於術前完成 3D 列印與滅菌，術中協助醫師完成 <span style="color:#22d3ee">drill trajectory（鑽孔軌跡）</span>、<span style="color:#22d3ee">osteotomies（截骨）</span>，以及<span style="color:#22d3ee">component positioning and orientation（假體位置與定向）</span>。

- 此類器械在 **total knee arthroplasty（TKA）**已有明確的應用紀錄與有效性，並正逐步於脊柱、上肢、畸形矯正與創傷領域獲得接受。
- **脊柱手術**：3D 列印的 drill guide 可提供 screw trajectory、depth 與 size 的指引，降低神經血管損傷風險。
- **2021 年研究**顯示，3D 列印 drill guide 可改善 pedicle screw 置入的準確度、減少失血量、縮短手術時間並減少透視（fluoroscopy）時間。
- 上述「減少失血、減少透視時間、縮短手術時間」的效益，亦已在**小兒骨科**、**total joint arthroplasty** 與**創傷手術**中獲得證實。

<!-- FIG: 圖 2 — 畸形手術之 patient-specific instrumentation 流程。A 膝關節 AP X 光；B 膝關節軸位 MRI；C 脛骨骨關節炎變形、計畫截骨、3D 虛擬脛骨 baseplate 置放，以及用於調整 varus/valgus、slope 與 rotation 的病人專屬器械；D 3D 導引之截骨與全膝關節置换；E 術後 X 光。（Yale School of Medicine 授權轉載） -->

### 1.2 個人化器械的標準工作流程（Figure 2）

| 步驟 | 執行者 | 內容 |
|------|--------|------|
| 1 | 外科醫師 | 篩選**骨關節炎且可從全膝關節置換獲益**的臨床候選者 |
| 2 | 外科醫師 | 以 **special MRI 與 full-length x-ray** 提供膝關節高解析度影像及肢體對位 |
| 3 | 臨床工程師 + 外科醫師 | 合作建立**虛擬 3D 術前計畫**（surgical resection guides 與 models） |
| 4 | 3D 列印 | 以 **nylon** 製作 3D 列印模型，備妥並於術中使用 |
| 5 | 外科醫師 | 依術前計畫進行 3D 導引之截骨與假體置放 |
| 6 | 外科醫師 | 以 **X 光**確認植入物位置與術前計畫一致 |

> **Pearl**：整條流程的關鍵在於第 3 步的「臨床工程師 + 外科醫師」共同作業；把術前計畫完全外包給工程師而未讓術者參與，是導致截骨角度與最終假體位置不符最常見的原因。

---

## 2. 技術分類與決策矩陣 (Classification & Decision Making)

本章「分類」指各項 3D 技術的臨床功能定位，而非疾病分型系統。決策的核心問題是：**這項技術要解決的是術前計畫、術中執行，還是植入物製造的問題？**

### 2.1 技術類別總覽

| 技術類別 | 代表工具／公司 | 主要解決的問題 | 現況 |
|----------|---------------|----------------|------|
| **3D 列印病人專屬器械** | Patient-specific instrumentation | 畸形矯正、截骨與假體定位的再現性 | TKA 已確立；脊柱、上肢、創傷逐步推展 |
| **機器人輔助關節置換** | Robotic-arm-assisted TKA / UKA | 依 3D 計畫執行切骨與假體置放 | TKA 與 medial unicompartmental knee arthroplasty（UKA）已具證據 |
| **3D 自訂植入物** | Conformis（客製化 hip／knee）、Zimmer Biomet（客製化 acetabular cup、custom hip stem、reverse TSA glenoid） | 嚴重骨缺損與異常解剖的重建 | 歐洲與中國已用於脊柱；美國部分產品**尚未核准** |
| **術中三維影像** | O-arm（Medtronic）、Iso-C 3D（Siemens）、Airo（Brainlab） | 術中導航複雜解剖、微創手術 | 顯著提升置位準確度，但可能延長手術時間 |
| **生物列印／四維列印** | Nylon／titanium／polyether ether ketone 等材料 | 製造客製化組織與可載藥、可生長的植入物 | 研究階段，多屬 Level V 專家評述 |
| **擴增實境（AR）** | Headset、3D 可視化演算法 | 術中 3D 重疊導引 | 仍處「嬰兒期」，需演算法與配準技術成熟 |

### 2.2 機器人與電腦導航（Robotics and Computer Navigation）

**機器人輔助全關節置換的執行要點：**

1. 先由**高解析度 CT scan** 建立 3D 模型。
2. 完成 3D 術前計畫後，將**骨性解剖配準（registered）到 3D 模型**上。
3. 機器人協助執行計畫，輔助 **drill trajectory、osteotomies 與假體置放**。

**已證實的效益**（相較 manual technique）：

| 效益面向 | 原文結論 |
|----------|----------|
| 切骨準確度 | 機器人系統提供**準確且可靠的切骨**，與 3D 計畫一致 |
| 假體置位 | 相較人工技術**置位更準確** |
| 功能評分 | 近期研究顯示**功能評分改善** |
| 植入物壽命 | 近期研究顯示**植入物壽命改善** |

> **Pearl**：機器人的價值不在「更會切」，而在於**把 3D 計畫轉譯成可重複執行的數值約束**；術者仍須負責計畫本身是否正確。

### 2.3 3D 自訂植入物（3D Custom Implants）

**材料**：3D 列印植入物使用多種材料，包括 <span style="color:#fb923c">titanium（鈦）</span> 與 <span style="color:#fb923c">polyether ether ketone（PEEK，聚醚醚酮）</span>。

- **歐洲與中國**：以**多孔鈦（porous titanium）**3D 列印**自訂脊柱植入物**，用於治療腫瘤切除所造成的骨缺損。
- **美國 Conformis**：依病人獨特解剖，製造客製化與個人化的 **hip（鈦）**與 **knee（cobalt-chromium、鈦、polyethylene）** 置換物。
- **美國 Zimmer Biomet**：為**嚴重 acetabulum 骨缺損與異常股骨解剖**的病人，客製化製造由鈦原料以 **computer numerical control（CNC）** 加工之 acetabular component。
- **Zimmer Biomet** 亦製造**數量有限**的 machined custom hip stem（total hip arthroplasty 用）與 reverse total shoulder arthroplasty 的 custom glenoid implant。
- **法規現況**：3D 列印之客製化 revision component **目前尚未在美國核准**。

<!-- FIG: 圖 3 — 3D 自訂植入物之製作流程。A 大腿 CT scan；B 股骨 3D 模型；C 植入物之 computer-aided design（CAD）圖；D 保留 rich voxel bone density data 之 meshed model；E 用於 implant selection 之有限元素分析（FEA）。示例為骨質疏鬆模型中使用 blade plate 固定之近端股骨骨折。（Yale School of Medicine 授權轉載） -->

**3D 自訂植入物之設計與分析流程（Figure 3）：**

| 步驟 | 內容 |
|------|------|
| 1. 取得高解析度 CT scan | 對 cadaver bones 進行 CT 掃描 |
| 2. 建立 3D 模型 | 以影像處理軟體（eg, Simpleware, Mimics）自 CT 建立 bone 之 3D 模型 |
| 3. CAD 設計 | 依 3D 模型虛擬定位植入物之 CAD 圖 |
| 4. Mesh 與 FEA | 模型被 mesh，保留 rich voxel bone density data，可轉換為 material properties；匯出至 FEA 套件分析 load 與 failure（eg, Abaqus, Comsol） |

### 2.4 術中三維影像（Intraoperative 3D Imaging）

新的**高解析度術中 CT 影像技術**協助醫師術中導航複雜解剖並執行微創手術，代表性系統包括 <span style="color:#60a5fa">O-arm（Medtronic）</span>、<span style="color:#60a5fa">Iso-C 3D（Siemens）</span>、<span style="color:#60a5fa">Airo（Brainlab）</span>。

- **效益**：已證實能**顯著改善植入物置位準確度**。
- **代價**：**2021 年一項研究**顯示此技術會導致**手術時間延長**。
- **技術演進**：現代術中 3D scanner 已改善解析度、擴大 field of view，並改進影像處理軟體——該軟體可**減少金屬假體造成的 artifact 失真**。
- **已確立用途**：足踝、創傷、脊柱與腫瘤手術。

> **Danger zone**：術中 CT 的「準確度提升」並非免費午餐；延長的手術時間會增加麻醉暴露、耗材成本與感染風險，在傷患無法承受長時間手術時應審慎使用。

### 2.5 新興技術：生物材料、生物列印與擴增實境

**生物材料與生物列印（Biologic Materials / Bioprinting）**

- 以 3D 列印製造**生物性肌肉骨骼組織**（ie, cartilage、bone、tendons）正在積極研究中。
- **2020 年研究**：解析度提升的 3D 列印技術提升了製造**複雜複合組織**（具有不同材料性質）的能力。
- 研究重點集中於複製 **articular cartilage（關節軟骨）、bone（骨）、meniscus（半月板）與 intervertebral disks（椎間盤）**。
- 將**活體人源多能細胞（pluripotent cells）**整合進 cartilage 3D 列印，「前景可期」。
- **四維列印（4D printing）**：可載入藥物、生物製劑與蛋白質作為載體的**解剖複雜骨替代物**正在開發中。

**四維列印的當前研究方向：**

| 方向 | 內容 |
|------|------|
| 載體釋放 | 映射 vascular progenitor cells 與 signaling molecules 的**客製化骨移植** |
| 生長適應 | 改變 biomaterial 性質，使植入物可**隨小兒病人一起生長與適應** |

**擴增實境（Augmented Reality）**

- 術中使用 3D AR 系統的開發正在**口腔手術、髖關節與膝關節手術、脊柱手術**中推進。
- 這些系統仍處於**「嬰兒期」**，需要 3D 可視化演算法、準確的模型配準方法，以及建立**共同參考點與陣列（common reference points and arrays）**的可靠方法等技術精煉。
- 隨著技術（如 headsets、演算法）成熟，AR 系統**可能會更廣泛普及**。

---

## 3. 臨床效益與證據層級 (Treatment Algorithm & Evidence)

本章不涉及「手術 vs. 保守」的治療取捨；其「治療指引」對應的是**該選用哪一項 3D 技術、以及各技術背後的證據強度**。以下依原文 Annotated References 所載之 **level of evidence** 整理。

### 3.1 各技術的證據層級總表

| 技術／主題 | 關鍵文獻與研究型態 | Level of evidence |
|------------|--------------------|-------------------|
| 病人專屬器械矯正截骨（兒童畸形） | Baraza 等，literature review | IV |
| 3D 列印病人專屬應用之總述 | Wong | —（綜述） |
| 3D 列印於骨科之現況與展望 | Bagaria 等，current concept review | —（綜述） |
| 3D 列印於遠端橈骨畸形癒合不良之虛擬規劃 | de Muinck Keizer 等，systematic review + meta-analysis | —（SR/MA） |
| 3D 列印於骨科創傷之應用 | Lal 與 Patralekh | —（綜述） |
| 3D 列印於脊柱手術 | Cai 等，book chapter | — |
| 醫療情境 3D 列印技術 | Tack 等，systematic literature review | —（SLR） |
| 複雜骨科創傷之虛擬術前規劃與 3D 列印 | Mishra 等，91 例觀察性研究 | **IV** |
| 軀幹複雜骨腫瘤之 3D 列印與導航 | Schulze 等，5 例 case series | **IV** |
| 術中 3D 影像（871 例） | Kumar 等，systematic review + meta-analysis | **IV** |
| 成人脊柱畸形之術前規劃與 pedicle screw | Lopez 等（PRISMA systematic review） | IV |
| 3D 列印模板預成型固定板 | Marinescu 等（PRISMA SLR） | IV |
| 脛骨平台骨折：3D 列印輔助 ORIF vs. 傳統 ORIF | Xie 等，systematic review + meta-analysis | —（SR/MA） |
| CT 為基礎之 3D 列印病人專屬墊塊（TKA） | Yaish 等 | — |
| Die-punch 骨折之 3D 列印治療 | Chen 等 | — |
| 導航模板輔助 vs. 傳統椎弓根固定 | Wen 等，meta-analysis（中文發表） | —（MA） |
| 頸椎融合之 3D 列印導航模板 | Azimi 等，systematic review + meta-analysis | **III** |
| 兒童前臂畸形之術前電腦模擬與病人專屬 guide | Bauer 等 | —（安全性與有效性） |
| 小兒骨科截骨之 3D 列印效果 | Raza 等（PRISMA SLR） | **IV** |
| 附肢骨骼骨折之 3D 列印 | Gonzalez-Alonso 等，SR + MA | **III** |
| 骨科手術 3D 列印之整體現況 | Levesque 等，scoping review | **III** |
| 骨盆骨折之 3D 列印可行性 | Wang 等，RCT 與前瞻比較研究之 SR/MA | **IV** |
| 機器人輔助 TKA 與人工技術之準確度 | Hampp 等 | —（準確度與精密性） |
| 機器人 vs. 人工 UKA | Iturriaga 等，systematic review | **IV** |
| 機器人輔助 medial UKA：至少 3 年追蹤 | Dretakis 與 Igoumenou，51 例 cohort | **IV** |
| 機器人輔助 medial UKA 之選擇與結果 | Lonner 與 Klement，review | **IV** |
| 3D 列印與生物列印於關節置換／骨科 | Trauner（editorial）、Zheng 等、Larsen 等 | **V** |
| 四維列印於骨科之重大進展 | Javaid 與 Haleem，expert review | **V** |
| 骨科 3D 可視化與擴增實境 | Ma 等 | — |
| 3D 列印自訂脊椎／骶骨重建 | Xu 等（Ewing sarcoma 上頸段）、Kim 等（sacral ostearcoma）、Wei 等（total en bloc sacrectomy） | —（病例與技術報告） |
| 翻修髋關節大型 acetabulum 骨缺損內 custom implant 之定位準確度 | Baauw 等 | — |

### 3.2 機器人輔助 UKA 的代表性追蹤結果

- **Dretakis 與 Igoumenou（2019）**：51 例接受**機器人輔助 unicompartmental knee arthroplasty** 的病人追蹤 **3 年**，屬 cohort study，Level of evidence IV。
- **Lunner 與 Klement（2019）**：回顧 robotic-assisted medial UKA 的選項與結果，Level of evidence IV。

> **Pearl**：整體而言，3D 技術相關研究的**最高證據層級僅到 Level III**（如 Azimi 的頸椎融合 SR/MA、Gonzalez-Alonso 的附肢骨折 SR/MA、Levesque 的 scoping review），多數為 Level IV 的觀察性研究、case series 或 SR/MA；生物列印與四維列印則完全停留在 **Level V 專家評述**。這意味著「3D 列印有前景」是可信的，但「3D 列印已優於傳統手術」在多數領域尚未被 RCT 證實。

### 3.3 個人化器械的流程與術式對應（Figure 2 再解析）

| 流程環節 | 對應的臨床決策 | 失敗後果 |
|----------|----------------|----------|
| Candidate identification | 誰適合病人專屬器械 | 納入不適合病人徒增成本與風險 |
| High-resolution imaging | 影像是否足以支撐 3D 重建 | 解剖變形或金屬 artifact 造成模型失真 |
| Virtual 3D preoperative plan | 截骨量與假體定位 | 計畫錯誤 → 假體位置偏差 |
| Nylon 3D printed models | 列印精度與滅菌 | 器械與計畫不符 → 術中偏移 |
| Implant positioning verification | X 光確認 | 未能即時察覺偏差 |

---

## 4. 陷阱與爭議 (Pitfalls & Controversies)

本章無手術入路內容；以下為原文所勾勒之**技術與法規層面陷阱**。

> **陷阱 1：機器人不是自動的正確答案**。機器人切骨「準確且可靠」，前提是**3D 計畫本身正確**；若 CT 建模或配準（registration）有誤，機器人只會把錯誤計畫執行得更精確。

> **陷阱 2：術中三維影像的代價**。準確度提升伴隨**手術時間延長**（2021 年研究），需納入整體效益評估。

> **陷阱 3：3D 自訂植入物的法規落差**。**3D 列印的客製化 revision component 目前尚未在美國核准**，美國以外（如歐洲、中國）已用多孔鈦列印脊柱植入物；臨床使用前務必確認當地法規狀態。

> **陷阱 4：AR 系統仍不成熟**。3D 可視化演算法、模型配準、common reference points 與 arrays 等關鍵技術仍在精煉階段，現階段不宜過度宣稱其臨床成熟度。

> **陷阱 5：多孔鈦與 PEEK 的臨床侷限**。原文指出自訂植入物材料包括鈦與 polyether ether ketone，但未提供對應的生物相容性或長期存活數據；評估時須注意此證據缺口。

> **陷阱 6：將單中心觀察性結果外推**。多數 3D 技術文獻為 Level IV 的觀察性研究或 case series（如 91 例創傷觀察性研究、5 例骨腫瘤 case series、51 例機器人 UKA cohort），其可推論範圍受限。

---

## 5. 實證更新與 OKU 14 重點 (Recent Evidence & Take-Home Points)

### 5.1 OKU 14 強調之趨勢與重點

| 主題 | 原文要點 |
|------|----------|
| **整體步調** | 3D 技術在骨科手術的應用**以穩定步調進展** |
| **未來數年預期成長** | ① 醫院系統內 **point-of-care printing center** 的成長；② **FDA 對 custom implant systems 的核准進展**；③ **機器人手術的接受與標準化** |
| **個人化技術的驅動力** | 改善病人預後與功能的**前景**將持續支撐對個人化手術技術、器械、植入物與機器人的投資 |
| **監管路徑** | FDA 正在發展 **point-of-care 3D printing pathway**，最終將允許在院內現場（onsite）客製化製造可植入裝置 |
| **機器人** | 機器人**提升準確度與客製化能力**，並**便利複雜病例處理**，已證實可改善病人預後 |
| **生物列印** | Bioprinting 是**新興技術**，前景在於**製造客製化組織** |

### 5.2 骨科專科考試核心總結（Take-Home Points）

1. **3D 技術讓病人專屬手術（custom surgery）成為可能**，目標為改善病人預後。
2. **術前規劃的價值鏈**：高解析度 CT／MRI → 3D 模型 → 病人專屬 plan／guide → 術中執行 → 術後 X 光驗證；每一步都需外科醫師參與。
3. **機器人輔助關節置換的三段式**：高解析度 CT 建立 3D 模型 → 骨性解剖配準 → 機器人依計畫執行切骨與假體置放；效益為切骨準確、置位更準、功能評分與植入物壽命改善。
4. **3D 自訂植入物材料**：鈦與 polyether ether ketone；歐洲與中國以多孔鈦列印脊柱植入物處理腫瘤切除後骨缺損；美國 Conformis（hip／knee）與 Zimmer Biomet（acetabular cup、custom hip stem、reverse TSA glenoid）已有產品，但 **3D 列印之 revision component 尚未在美國核准**。
5. **術中 3D 影像**（O-arm、Iso-C 3D、Airo）改善置位準確度但**延長手術時間**，並已確立於足踝、創傷、脊柱與腫瘤手術的用途。
6. **生物列印與四維列印**：目標為關節軟骨、骨、半月板、椎間盤；四維列印可載藥與載生長因子，並可能生長適應小兒病人。
7. **AR 仍在「嬰兒期」**，待演算法、配準與共同參考點技術成熟。
8. **證據層級現實**：多數 3D 技術研究為 Level IV，最高僅至 Level III；生物列印／四維列印為 Level V。

---

## Summary

- **3D 技術定位**：依功能分為術前規劃、術中執行（導航／機器人）、植入物製造（自訂植入物）、組織再生（bioprinting／4D printing）與 AR 導引五大類。
- **個人化器械**：術前 3D 列印並滅菌，術中協助鑽孔軌跡、截骨與假體定位；TKA 已確立，脊柱／上肢／創傷／小兒骨科逐步推展。
- **機器人**：CT 建 3D 模型 → 解剖配準 → 機器人執行計畫；切骨準確且與計畫一致，置位優於人工，功能與植入物壽命改善。
- **自訂植入物**：鈦與 polyether ether ketone；歐中已用多孔鈦做脊柱重建；美國 Conformis 與 Zimmer Biomet 有客製化產品，但 3D 列印 revision component 尚未核准。
- **術中 3D 影像**：改善置位準確度，但可能延長手術時間。
- **新興技術**：bioprinting 製造客製化組織；4D printing 載藥並可生長適應；AR 仍處嬰兒期。
- **未來數年三大成長點**：醫院 point-of-care printing center、FDA 對 custom implant 的核准、機器人手術的接受與標準化。
- **證據現實**：多數為 Level IV 觀察性研究／case series／SR-MA，最高至 Level III；生物與四維列印為 Level V。

---

## 參考文獻

1. Baraza N, Chapman C, Zakani S, Mulpuri K: 3D-Printed patient specific instrumentation in corrective osteotomy of the femur and pelvis: A review of the literature. J 3D Print Med 2020;6:34.

2. Wong KC: 3D-printed patient-specific applications in orthopedics. Orthop Res Rev 2016;8:57.

3. Bagaria V, Bhansali R, Pawar P: 3D printing—creating a blueprint for the future of orthopedics: Current concept review and the road ahead! J Clin Orthop Trauma 2018;9:207-212.

4. de Muinck Keizer RJO, Lechner KM, Mulders MAM, Goslings JC, Schep NWL, Eygendaal D: Three-dimensional virtual planning of corrective osteotomies of distal radius malunions: A systematic review and meta-analysis. Strategies Trauma Limb Reconstr 2017;12:77-89.

5. Lal H, Patralekh MK: 3D printing and its applications in orthopaedic trauma: A technological marvel. J Clin Orthop Trauma 2018;9:260-268.

6. Cai H, Liu Z, Wei F, Yu M, Xu N, Li Z: 3D printing in spine surgery, in Zheng G, Tian W, Zhuang X, eds: Intelligent Orthopaedics: Artificial Intelligence and Smart Image-Guided Technology for Orthopaedics. Springer, 2018;vol 1093:345-359.

7. Tack P, Annemans L, Victor J, Gemmel P: 3D-printing techniques in a medical setting: A systematic literature review. Biomed Eng Online 2016;15:115.

8. Mishra A, Verma T, Vaish A, Vaish R, Maini L, Vaishya R: Virtual preoperative planning and 3D printing are valuable for the management of complex orthopaedic trauma. Chin J Traumatol 2019;22:350-355.

9. Schulze M, Gosheger G, Bockholt S, et al: Complex bone tumors of the trunk—the role of 3D printing and navigation in tumor orthopedics: A case series and review of the literature. Pers Med 2021;11:517.

10. Lopez CD, Boddapati V, Lee NJ, et al: Three-dimensional printing for preoperative planning and pedicle screw placement in adult spinal deformity: A systematic review. Global Spine J 2020;11(6):936-949.

11. Marinescu R, Popescu D, Laptoiu D: A review on 3D-printed templates for precontouring fixation plates in orthopedic surgery. J Clin Med 2020;9:1-17.

12. Xie L, Chen C, Zheng W, Chen H, Cai L, Zhang Y: Three-dimensional printing assisted ORIF versus conventional ORIF for tibial plateau fractures: A systematic review and meta-analysis. Int J Surg 2018;57:35-44.

13. Yaish YA, Vijay V, Agarwal AK, Vaish A: Computed tomography based 3D printed patient specific blocks for total knee replacement. J Clin Orthop Trauma 2018;9:254-259.

14. Chen C, Cai L, Zhang C, Wang J, Guo X, Zhou Y: Treatment of die-punch fractures with 3D printing technology. J Invest Surg 2018;31:385-392.

15. Wen Z-J, Gao Z-C, Lu T, Wang Y-B, Liang H, He X-J: Comparison of the effect of navigation template assisted spinal pedicle fixation and traditional pedicle screw fixation: A meta-analysis. Zhongguo Gu Shang 2018;31:1069-1076.

16. Azimi P, Yazdanian T, Benzel EC, Azimi A, Montazeri A: 3D-printed navigation template in cervical spine fusion: A systematic review and meta-analysis. Eur Spine J 2021;30:389-401.

17. Bauer AS, Storelli DAR, Sibbel SE, McCarroll HR, Lattanza LL: Preoperative computer simulation and patient-specific guides are safe and effective to correct forearm deformity in children. J Pediatr Orthop 2017;37:504-510.

18. Raza M, Murphy D, Gelfer Y: The effect of three-dimensional (3D) printing on quantitative and qualitative outcomes in paediatric orthopaedic osteotomies: A systematic review. EFORT Open Rev 2021;6:130-138.

19. Gonzalez-Alonso M, Hermida-Sanchez M, Martinez-Seijas P, Ruano-Ravina A: Application of 3D printing in the treatment of appendicular skeleton fractures: Systematic review and meta-analysis. J Orthop Res 2021;39(10):2083-2092.

20. Levesque JN, Shah A, Ekhtiari S, Yan JR, Thornley P, Williams DS: Three-dimensional printing in orthopaedic surgery: A scoping review. EFORT Open Rev 2020;5:430-441.
