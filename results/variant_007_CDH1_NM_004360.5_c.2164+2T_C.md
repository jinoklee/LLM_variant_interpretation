# Variant Analysis Report #7

**Gene:** CDH1

**Variant:** NM_004360.5:c.2164+2T>C

---

<think>
Okay, let's tackle this variant interpretation for CDH1 c.2164+2T>C. First, I need to recall the ACMG/AMP 2015 guidelines and the ClinGen SVI recommendations. The variant is a splice site mutation, specifically at the +2 position of the intron. 

Starting with PVS1: This is for variants in a critical splice site. The +2 position is part of the splice donor site, so this might qualify. But I should check if it's a canonical splice site. The c.2164+2T>C is in the intron, so the splice donor site is usually at the 5' end of the intron. The +2 position is part of the GT dinucleotide, which is the splice donor. Changing T to C at +2 would disrupt the GT, so this is a strong PVS1. But I need to confirm if it's a canonical site. Since it's the +2 position, it's part of the GT, so PVS1 applies here.

Next, PS1-4. PS1 is for population frequency. The gnomAD data is None, so no evidence against pathogenicity. PS2 is for de novo, but that's not available here. PS3 is for segregation, which is also not available. PS4 is for functional studies, which are N/A. So PS1 might be applicable if the variant is absent in population databases, but since it's not present, maybe PS1 is not applicable because the absence isn't confirmed. Wait, the gnomAD AF is None, which could mean it's not present in the database. But the user might have meant that the data isn't available. Hmm, the user wrote "None" for gnomAD AF, which might indicate that the variant isn't present in the database. If that's the case, then PS1 (population frequency) would be in favor of pathogenicity. But I need to be careful here. If the variant is not found in gnomAD, that's a PS1. But if the data is not available, then it's not applicable. The user's input says "None" for all gnomAD data, which might mean the variant isn't present. So PS1 would be applicable here.

PM1-6: PM1 is for location in a known functional element. Since it's a splice site, that's a PM1. PM2 is for conservation, but phyloP is N/A. PM3 is for segregation, which is N/A. PM4 is for functional studies, which are N/A. PM5 is for co-occurrence with other pathogenic variants, which isn't mentioned. PM6 is for predicted effect, but SpliceAI is N/A. So PM1 applies here.

PP1-5: PP1 is for de novo, which is N/A. PP2 is for recessive inheritance, but CDH1 is usually autosomal dominant. PP3 is for functional studies, which are N/A. PP4 is for segregation, which is N/A. PP5 is for computational prediction, but SpliceAI is N/A. So no PP criteria apply.

BA1 is for a known pathogenic variant in the same position, but ClinVar and HGMD don't have data. So BA1 is not applicable.

BS1-4: BS1 is for population frequency. If the variant is not present in gnomAD, that's a BS1. But if the data is not available, then it's not applicable. The user's input says "None" for gnomAD AF, which might mean the variant isn't present. If that's the case, then BS1 would be in favor of pathogenicity. Wait, no, BS1 is for presence in population databases. If the variant is not present, that's a PS1, not BS1. BS1 is when the variant is present in population databases. So if the variant isn't present, that's PS1. So BS1 is not applicable here.

BP1-7: BP1 is for population frequency, which is not applicable. BP2 is for benign variants in the same position, but no data. BP3 is for functional studies, which are N/A. BP4 is for computational prediction, which is N/A. BP5 is for segregation, which is N/A. BP6 is for co-occurrence with benign variants, which is not mentioned. BP7 is for other factors, which aren't present. So no BP criteria apply.

Now, applying ClinGen SVI for PS3/BS3 and PVS1. Since the variant is a splice site, PVS1 is strong. The absence in population databases (gnomAD) supports PS1. However, if the variant is not present in gnomAD, that's a PS1. But if the data is not available, then it's not a PS1. The user's input says "None" for gnomAD AF, which might mean the variant isn't present. If that's the case, then PS1 is applicable. However, if the data is not available, then we can't confirm absence. This is a bit ambiguous. But assuming that "None" means absence, then PS1 applies.

For PVS1, the variant is in a critical splice site, so PVS1 is applicable. The ClinGen SVI says that PVS1 is strong, and if the variant is in a canonical splice site, it's a strong PVS1. Since this is the +2 position of the intron, which is part of the GT dinucleotide, it's a canonical splice site. So PVS1 is strong.

Combining all the criteria: PVS1 (strong), PS1 (if applicable), PM1. No other criteria. The absence in population databases (if confirmed) would support PS1. However, if the data is not available, then PS1 is not applicable. The user's input says "None" for gnomAD AF, which might mean the variant isn't present. If that's the case, then PS1 is applicable. But if the data is not available, then we can't confirm. This is a point of uncertainty.

Assuming that the variant is not present in gnomAD, then PS1 is applicable. So the criteria would be PVS1 (strong), PS1, PM1. No conflicting criteria. Therefore, the classification would be Pathogenic (P). However, if the absence in gnomAD is not confirmed, then PS1 is not applicable, and the classification would be Pathogenic (P) based on PVS1 and PM1.

But the user's input says "None" for gnomAD AF, which might mean that the variant isn't present. So I think PS1 applies here. Therefore, the final classification would be Pathogenic (P) with high confidence.
</think>

### **ACMG/AMP 2015 기준 평가 및 변이 해석**

#### **1. PVS1 (Pathogenic Variant in a Splice Site)**
- **충족 여부**: **예**  
- **근거**:  
  - 변이는 **NM_004360.5:c.2164+2T>C**로, **스플라이스 도너 사이트**(intron의 5' 끝 GT dinucleotide)의 **+2 위치**에 위치합니다.  
  - 이 위치는 **정상적인 스플라이싱을 위해 필수적인 GT 서열**의 일부로, **T→C 변이**는 **스플라이싱 기능을 완전히 손상**시킬 수 있습니다.  
  - **ClinGen SVI 권고안**에 따르면, **정규 스플라이스 사이트**(예: GT dinucleotide)의 변이는 **PVS1 강도 조절**을 적용받아 **강한 증거**로 간주됩니다.  
- **결론**: **PVS1 (Strong)**

---

#### **2. PS1-4 (Population Frequency, De Novo, Segregation, Functional Studies)**
- **PS1 (Population Frequency)**:  
  - **충족 여부**: **예** (가정: gnomAD AF = None → 변이가 데이터베이스에 존재하지 않음)  
  - **근거**:  
    - gnomAD AF (전체 및 popmax)가 **None**으로 표기되어, **인구 집단에서의 빈도가 확인되지 않음**.  
    - 이는 **변이가 일반적인 유전적 변이가 아니며, 병원성 가능성을 높이는 증거**로 간주됩니다.  
- **PS2 (De Novo)**: **No** (데이터 없음)  
- **PS3 (Segregation)**: **No** (데이터 없음)  
- **PS4 (Functional Studies)**: **No** (데이터 없음)  
- **결론**: **PS1 (Moderate)** (gnomAD 데이터 부재로 인한 병원성 가능성을 높이는 증거)

---

#### **3. PM1-6 (Location, Conservation, Segregation, Functional Studies, Co-occurrence, Computational Prediction)**
- **PM1 (Location in Known Functional Element)**:  
  - **충족 여부**: **예**  
  - **근거**:  
    - 변이는 **스플라이스 도너 사이트**(intron의 5' 끝 GT dinucleotide)에 위치하며, 이는 **유전자 기능에 직접적인 영향을 미치는 영역**입니다.  
- **PM2 (Conservation)**: **No** (phyloP 데이터 없음)  
- **PM3 (Segregation)**: **No** (데이터 없음)  
- **PM4 (Functional Studies)**: **No** (데이터 없음)  
- **PM5 (Co-occurrence)**: **No** (데이터 없음)  
- **PM6 (Computational Prediction)**: **No** (SpliceAI 데이터 없음)  
- **결론**: **PM1 (Moderate)**

---

#### **4. PP1-5 (De Novo, Recessive Inheritance, Functional Studies, Segregation, Computational Prediction)**
- **PP1 (De Novo)**: **No** (데이터 없음)  
- **PP2 (Recessive Inheritance)**: **No** (CDH1은 일반적으로 **autosomal dominant** 유전)  
- **PP3 (Functional Studies)**: **No** (데이터 없음)  
- **PP4 (Segregation)**: **No** (데이터 없음)  
- **PP5 (Computational Prediction)**: **No** (SpliceAI 데이터 없음)  
- **결론**: **No PP criteria**

---

#### **5. BA1 (Known Pathogenic Variant in Same Position)**
- **충족 여부**: **No**  
- **근거**:  
  - ClinVar 및 HGMD에서 **동일 위치의 병원성 변이**가 기록되지 않음.  
- **결론**: **No BA1**

---

#### **6. BS1-4 (Population Frequency, Benign Variant, Functional Studies, Co-occurrence)**
- **BS1 (Population Frequency)**: **No** (gnomAD 데이터 부재는 **PS1**에 해당, **BS1**은 빈도가 높은 경우에 해당)  
- **BS2 (Benign Variant)**: **No** (데이터 없음)  
- **BS3 (Functional Studies)**: **No** (데이터 없음)  
- **BS4 (Co-occurrence)**: **No** (데이터 없음)  
- **결론**: **No BS criteria**

---

#### **7. BP1-7 (Population Frequency, Benign Variant, Functional Studies, Co-occurrence, Other Factors)**
- **BP1 (Population Frequency)**: **No** (gnomAD 데이터 부재는 **PS1**에 해당)  
- **BP2 (Benign Variant)**: **No** (데이터 없음)  
- **BP3 (Functional Studies)**: **No** (데이터 없음)  
- **BP4 (Computational Prediction)**: **No** (SpliceAI 데이터 없음)  
- **BP5 (Segregation)**: **No** (데이터 없음)  
- **BP6 (Co-occurrence)**: **No** (데이터 없음)  
- **BP7 (Other Factors)**: **No**  
- **결론**: **No BP criteria**

---

### **최종 분류 및 신뢰도**
- **ACMG/AMP 기준**:  
  - **PVS1 (Strong)** + **PS1 (Moderate)** + **PM1 (Moderate)**  
  - **총 점수**: **Strong + Moderate + Moderate = Pathogenic (P)**  
- **ClinGen SVI 권고안**:  
  - **PVS1**은 **강한 증거**로, **gnomAD 데이터 부재**(PS1)와 **스플라이스 기능 손상**(PM1)을 추가로 고려하여 **병원성 가능성이 매우 높음**.  
- **최종 분류**: **Pathogenic (P)**  
- **신뢰도**: **High** (PVS1, PS1, PM1의 강한 증거로 인해)  
- **임상적 해석**:  
  - **CDH1** 유전자의 **스플라이스 도너 사이트** 변이는 **유전자 기능을 완전히 손상**시킬 수 있으며, **가족 내 유전적 분리**나 **기능적 연구** 없이도 **병원성으로 분류**할 수 있습니다.  
  - **gnomAD 데이터 부재**는 **인구 집단에서의 빈도가 낮거나 없음을 시사**하며, **병원성 가능성을 높이는 추가 증거**로 작용합니다.  

---

### **결론**
**NM_004360.5:c.2164+2T>C** 변이는 **ACMG/AMP 2015 기준**에 따라 **Pathogenic (P)**으로 분류됩니다. 이는 **스플라이스 도너 사이트의 변이**(PVS1), **인구 집단에서의 빈도 부재**(PS1), **기능적 영역 위치**(PM1)의 강한 증거를 바탕으로 한 것입니다. **신뢰도는 High**이며, 임상적으로 **유방암 및 위암 관련 질환**의 유전적 위험성을 고려해야 합니다.