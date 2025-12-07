# Variant Analysis Report #12

**Gene:** RUNX1

**Variant:** NM_001754.5:c.565T>C

---

<think>
Okay, let's tackle this variant interpretation for RUNX1 c.565T>C (p.Tyr189His). First, I need to go through each ACMG/AMP 2015 criterion step by step. 

Starting with PVS1, which is for loss of function variants in genes where such variants are known to cause disease. The variant here is missense, not a loss of function, so PVS1 doesn't apply. 

Next, PS1-4. PS1 is about the variant being present in a disease-specific database. ClinVar lists it as Uncertain Significance, which isn't strong enough for PS1. PS2 would require a de novo occurrence, but there's no data on that. PS3 is about segregation in families, which isn't available here. PS4 is population frequency, but gnomAD data is missing, so PS4 isn't applicable.

Moving to PM1-6. PM1 is about population frequency. Since gnomAD AF is None, maybe it's very rare, but without specific numbers, it's hard to say. PM2 is about in silico predictions. CADD is 0.998, which is low, and REVEL is 0.965, which is also not high. Both are below the thresholds for PM2 (CADD >20, REVEL >0.8). So PM2 doesn't apply. PM3 is about functional studies, which are N/A. PM4 is about segregation, which isn't available. PM5 is about co-occurrence with other pathogenic variants, which isn't mentioned. PM6 is about allele frequency in controls, but again, no data here.

PP1-5. PP1 is about the variant being in a gene with a known disease association. RUNX1 is associated with acute myeloid leukemia and other conditions, so PP1 applies. PP2 is about the variant being in a gene where missense variants are pathogenic. RUNX1 is a tumor suppressor, so PP2 might apply. PP3 is about functional studies, which are N/A. PP4 is about segregation, which isn't available. PP5 is about other evidence, which isn't present here.

BA1 is about a known pathogenic variant in the same position, which isn't available. BS1 is about population frequency, but since it's not available, maybe not applicable. BS2 is about in silico predictions, but the scores are low, so BS2 doesn't apply. BS3 is about a variant in a region of low conservation, but phyloP is N/A. BS4 is about a variant in a gene where missense variants are not pathogenic, which might not be the case here.

BP1-7. BP1 is about population frequency, which is missing. BP2 is about in silico predictions, but the scores are low. BP3 is about the variant being in a region of low conservation, which is N/A. BP4 is about the variant being in a gene where missense variants are not pathogenic, which might not apply. BP5 is about the variant being in a region of low conservation, again N/A. BP6 is about the variant being in a gene with no known pathogenic variants, which isn't the case. BP7 is about the variant being in a gene where pathogenic variants are usually loss of function, which might apply here since the variant is missense, but not sure.

Considering ClinGen SVI guidelines, PS3 and BS3 require segregation data, which isn't available. PVS1 adjustment for missense variants doesn't apply here. 

Putting it all together, the strongest evidence is PP1 (gene known to cause disease) and maybe PP2 (missense in a tumor suppressor gene). However, the in silico predictions are not strong enough for PM2. Since there's no segregation data, PS3 and BS3 can't be applied. The lack of population data might be a BS1, but since it's not available, maybe not. The final classification would likely be VUS because there's insufficient evidence to classify it as pathogenic or benign.
</think>

### ACMG/AMP 2015 기준에 따른 변이 해석

#### **1. PVS1 (Loss of Function Variant in a Gene with Known Disease Association)**
- **적용 여부**: **불충족**  
  - 변이는 **missense** 유형이며, **loss of function**이 아님.  
  - RUNX1은 **loss of function** 변이가 질환과 관련된 유전자이지만, 이 변이는 **missense**이므로 PVS1 기준에 해당하지 않음.

---

#### **2. PS1-4 (Population Frequency, De Novo, Segregation, Disease-Specific Databases)**
- **PS1 (Disease-Specific Database)**:  
  - **ClinVar**: **Uncertain Significance** (PS1 기준 충족 불가).  
- **PS2 (De Novo)**:  
  - **De novo** 데이터 없음 (PS2 불충족).  
- **PS3 (Segregation in Families)**:  
  - **가계 분리 데이터 없음** (PS3 불충족).  
- **PS4 (Population Frequency in Controls)**:  
  - **gnomAD AF (전체/Popmax/동형접합)**: **None** (PS4 불충족).  

---

#### **3. PM1-6 (Population Frequency, In Silico Predictions, Functional Studies, Co-occurrence, Allele Frequency)**
- **PM1 (Population Frequency)**:  
  - **gnomAD AF** 데이터 없음 (PM1 불충족).  
- **PM2 (In Silico Predictions)**:  
  - **CADD**: 0.998 (낮은 점수, PM2 기준: CADD >20).  
  - **REVEL**: 0.965 (낮은 점수, PM2 기준: REVEL >0.8).  
  - **SpliceAI**: N/A (PM2 불충족).  
- **PM3 (Functional Studies)**:  
  - **In vitro/in vivo 데이터 없음** (PM3 불충족).  
- **PM4 (Segregation)**:  
  - **가계 분리 데이터 없음** (PM4 불충족).  
- **PM5 (Co-occurrence with Other Pathogenic Variants)**:  
  - **데이터 없음** (PM5 불충족).  
- **PM6 (Allele Frequency in Controls)**:  
  - **gnomAD AF** 데이터 없음 (PM6 불충족).  

---

#### **4. PP1-5 (Gene-Disease Association, Missense in Disease-Associated Genes, Functional Studies, Segregation, Other Evidence)**
- **PP1 (Gene-Disease Association)**:  
  - **RUNX1**은 **AML, ALL, myelodysplastic syndromes** 등과 관련된 유전자 (PP1 **충족**).  
- **PP2 (Missense in Disease-Associated Genes)**:  
  - **RUNX1**은 **tumor suppressor gene**으로, missense 변이가 질환과 관련될 수 있음 (PP2 **충족**).  
- **PP3 (Functional Studies)**:  
  - **기능 연구 데이터 없음** (PP3 불충족).  
- **PP4 (Segregation)**:  
  - **가계 분리 데이터 없음** (PP4 불충족).  
- **PP5 (Other Evidence)**:  
  - **데이터 없음** (PP5 불충족).  

---

#### **5. BA1 (Known Pathogenic Variant in Same Position)**:  
- **HGMD**: **Not available** (BA1 불충족).  

---

#### **6. BS1-4 (Population Frequency, In Silico Predictions, Functional Studies, Gene-Specific Evidence)**
- **BS1 (Population Frequency)**:  
  - **gnomAD AF** 데이터 없음 (BS1 불충족).  
- **BS2 (In Silico Predictions)**:  
  - **CADD/REVEL** 점수 낮음 (BS2 불충족).  
- **BS3 (Segregation in Families)**:  
  - **가계 분리 데이터 없음** (BS3 불충족).  
- **BS4 (Gene-Specific Evidence)**:  
  - **RUNX1**은 missense 변이가 질환과 관련될 수 있음 (BS4 불충족).  

---

#### **7. BP1-7 (Population Frequency, In Silico Predictions, Conservation, Gene-Specific Evidence, etc.)**
- **BP1 (Population Frequency)**:  
  - **gnomAD AF** 데이터 없음 (BP1 불충족).  
- **BP2 (In Silico Predictions)**:  
  - **CADD/REVEL** 점수 낮음 (BP2 불충족).  
- **BP3 (Conservation)**:  
  - **phyloP** 데이터 없음 (BP3 불충족).  
- **BP4 (Gene-Specific Evidence)**:  
  - **RUNX1**은 missense 변이가 질환과 관련될 수 있음 (BP4 불충족).  
- **BP5 (Conservation)**:  
  - **phyloP** 데이터 없음 (BP5 불충족).  
- **BP6 (Gene-Specific Evidence)**:  
  - **RUNX1**은 loss of function 변이가 질환과 관련된 유전자 (BP6 불충족).  
- **BP7 (Gene-Specific Evidence)**:  
  - **RUNX1**은 missense 변이가 질환과 관련될 수 있음 (BP7 불충족).  

---

### **ClinGen SVI 권고안 적용**
- **PS3/BS3**: **가계 분리 데이터 없음** → **적용 불가**.  
- **PVS1 강도 조절**: **missense 변이**이므로 PVS1 적용 불가.  

---

### **최종 분류 및 근거**
- **Strongest Evidence**:  
  - **PP1 (RUNX1의 질환 관련성)**, **PP2 (missense in tumor suppressor gene)**.  
- **Weak Evidence**:  
  - **ClinVar: Uncertain Significance**, **CADD/REVEL 점수 낮음**, **gnomAD 데이터 부족**.  
- **Contradictory Evidence**:  
  - **No strong pathogenic or benign evidence**.  

---

### **최종 분류**
- **분류**: **VUS (Variants of Uncertain Significance)**  
- **신뢰도**: **Low**  
- **임상적 해석**:  
  - **RUNX1**은 질환과 관련된 유전자이지만, 이 변이는 **missense** 유형이며, **in silico 예측 점수 낮음**, **가계 분리 및 집단 데이터 부족**으로 인해 **병원성 또는 양성 가능성을 판단할 수 없음**.  
  - **추가 연구 (기능 분석, 가계 분리, 대규모 집단 데이터)**가 필요함.  

--- 

**참고**: 이 해석은 ACMG/AMP 2015 기준과 ClinGen SVI 권고안을 기반으로 하며, 임상적 맥락(예: 환자의 임상 증상, 가족력 등)에 따라 재평가가 필요할 수 있음.