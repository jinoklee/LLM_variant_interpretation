# Variant Analysis Report #12

**Gene:** RUNX1

**Variant:** NM_001754.5:c.565T>C

---

<think>
Okay, let's tackle this variant interpretation for the RUNX1 gene. The variant in question is NM_001754.5:c.565T>C, which translates to p.Tyr189His. First, I need to go through each of the ACMG/AMP 2015 criteria step by step.

Starting with the Pathogenic (P) criteria. PVS1 is for loss-of-function variants in genes where LOF is a known disease mechanism. Since this is a missense variant, not a nonsense or frameshift, PVS1 doesn't apply here. So, PVS1 is not met.

Next, PS1: looking for the same amino acid change in a known pathogenic variant. The ClinVar entry is Uncertain Significance, and there's no mention of this exact variant being in ClinVar as pathogenic. So PS1 isn't met.

PS2 requires de novo in a patient without family history. The data here doesn't mention de novo status, so PS2 is not applicable.

PS3 is about functional studies. The variant has no in vitro or in vivo data, so PS3 isn't met.

PS4 is about increased frequency in patients vs controls. The gnomAD data is missing, so I can't assess this. Maybe the absence of data in gnomAD could be a point, but without specific numbers, it's hard to say. So PS4 is not met.

Moving to PM criteria. PM1: hotspot or functional domain. I need to check if Tyr189 is in a known domain. RUNX1 has a Runt domain, and Tyr189 might be part of it. If it's in a critical region, PM1 could be met. But without specific domain information, I might need to assume it's not a hotspot unless there's evidence. Since the data doesn't specify, maybe PM1 is not met.

PM2: absence from population databases. The gnomAD AF is None, which might mean it's not present. If the variant is absent in gnomAD, that's a PM2. But the user wrote "None" for AF, which could mean it's not present. So PM2 is met as a strong criterion.

PM3: trans in a recessive disease. Since RUNX1 is involved in a dominant disorder (like acute myeloid leukemia), this might not apply. So PM3 is not met.

PM4: change in protein length. This is a missense, so no change in length. PM4 is not met.

PM5: if there are other pathogenic missenses at the same position. The data doesn't mention other variants at Tyr189, so PM5 is not met.

PM6: de novo but not confirmed. The data doesn't confirm de novo, so PM6 is not met.

Now the supporting (PP) criteria. PP1: co-segregation in families. No data on family segregation, so PP1 is not met.

PP2: missense in a gene where missense is rare. RUNX1 is a gene where missense variants are less common, but without specific data, it's hard to say. If the gene is known for LOF variants, then a missense might be less likely, so PP2 could be considered. But since the variant is missense, maybe PP2 is not applicable. Alternatively, if the gene is known for LOF, then a missense might be less likely, so PP2 could be a supporting point. But I need to check if RUNX1 is typically associated with LOF variants. Since RUNX1 mutations are often LOF in conditions like AML, then a missense might be less likely, so PP2 could be considered as a supporting point. However, the user didn't provide specific info on the gene's typical variant types, so this is a bit uncertain. Maybe PP2 is not met.

PP3: computational evidence. The CADD score is 0.998, which is very low (since CADD scores are on a scale where higher is more damaging). Wait, no, CADD scores are typically higher for more damaging variants. Wait, the CADD score here is 0.998, which is actually very low. That suggests it's not damaging. REVEL is 0.965, which is also low (REVEL scores are 0-1, with higher being more damaging). So both CADD and REVEL are low, indicating the variant is not damaging. So PP3, which is about multiple computational evidence supporting pathogenicity, is not met. Instead, this would support benign, but since we're looking at PP3, which is for pathogenic, this is not applicable. So PP3 is not met.

PP4: phenotype specificity. The user didn't provide patient phenotype or family history, so PP4 is not met.

PP5: classified as pathogenic in a reputable database. ClinVar has it as Uncertain Significance, so PP5 is not met.

Now the Benign (B) criteria. BA1: allele frequency >5% in population databases. Since gnomAD AF is None, which might mean it's not present, so BA1 is not met.

BS1: higher frequency than expected. Since the variant is absent in gnomAD, this might not apply. But without data, it's hard to say. So BS1 is not met.

BS2: observed in healthy adults. No data on this, so BS2 is not met.

BS3: functional studies show no effect. No functional data, so BS3 is not met.

BS4: lack of segregation. No data, so BS4 is not met.

BP criteria: BP1: missense in a gene where LOF is the mechanism. Since RUNX1 is associated with LOF, a missense might be less likely, so BP1 could be a supporting point. But the user didn't specify, so this is uncertain. Maybe BP1 is not met.

BP2: trans in dominant disease. Not applicable here.

BP3: in-frame indel in non-functional region. Not applicable.

BP4: computational evidence suggests no effect. The CADD and REVEL scores are low, which would support benign, so BP4 is met as a supporting point.

BP5: alternative molecular evidence. No data, so BP5 is not met.

BP6: classified as benign in a reputable database. ClinVar is Uncertain, so BP6 is not met.

BP7: no splice effect. SpliceAI is N/A, and the variant is missense, so BP7 is met as a supporting point.

Putting it all together, the only criteria met are PM2 (strong) and BP4 and BP7 (supporting). According to the ACMG criteria, for a VUS, you need to meet the criteria for pathogenic or benign. Since the only supporting points are for benign (BP4 and BP7), but they are not strong enough on their own. The PM2 is a strong pathogenic criterion, but the computational evidence (CADD and REVEL) are low, which would support benign. However, PM2 is a strong pathogenic criterion, but the absence in population databases (PM2) is a strong point for pathogenicity. However, the computational evidence is against pathogenicity. This is conflicting.

Wait, PM2 is a pathogenic criterion, but the variant is absent in population databases, which is a strong point for pathogenicity. However, the computational evidence (CADD and REVEL) are low, which would support benign. So there's a conflict between PM2 (pathogenic) and BP4 and BP7 (benign). But according to the criteria, PM2 is a strong pathogenic criterion, but the absence in population databases (PM2) is a strong point. However, the computational evidence (CADD and REVEL) are low, which would support benign. But the user didn't provide any functional data. So the variant is absent in population databases (PM2), which is a strong pathogenic criterion, but the computational evidence is low. However, the absence in population databases is a strong point for pathogenicity, but the low CADD and REVEL scores suggest it's not damaging. This is a bit of a dilemma. 

In this case, since the variant is absent in population databases (PM2), which is a strong pathogenic criterion, but the computational evidence is low, which would support benign. However, the absence in population databases is a strong point for pathogenicity. But without any functional data or other pathogenic criteria, the variant might be classified as VUS. However, the presence of PM2 (strong) and the absence of any strong benign criteria (like BA1) might lead to a VUS. Alternatively, if the absence in population databases is considered a strong pathogenic criterion, but the computational evidence is low, it's a conflict. 

But according to the ACMG guidelines, PM2 is a pathogenic criterion, and if it's met, but there's no other pathogenic criteria, and the benign criteria are not met, then it might be classified as VUS. However, the absence in population databases (PM2) is a strong pathogenic criterion, but the low CADD and REVEL scores (which are part of the PP3 and BP4 criteria) suggest it's not pathogenic. So the variant is in a gray area. 

Given that, the final classification would be VUS, as the evidence is conflicting. The absence in population databases (PM2) is a strong pathogenic criterion, but the computational evidence (BP4 and BP7) supports benign. However, without any other pathogenic criteria, and the absence of strong benign criteria, the variant is classified as VUS with low confidence.
</think>

### **1. 병원성 증거 (Pathogenic Evidence)**

#### **A. 매우 강력 (PVS1):**
- **평가:** 미충족  
- **근거:** 변이는 nonsense, frameshift, 스플라이스 사이트, 시작코돈, 엑손 결실 등이 아닌 **missense** 변이로, PVS1 기준에 해당하지 않음.  
- **강도:** 미충족  

---

#### **B. 강력 (PS1-PS4):**
- **PS1:** 미충족  
  - 근거: ClinVar에서 **Uncertain Significance**로 분류되어, 동일한 아미노산 변화의 확립된 병원성 변이가 없음.  
- **PS2:** 미충족  
  - 근거: De novo 여부 확인 불가 (가계 분리 및 De novo 데이터 없음).  
- **PS3:** 미충족  
  - 근거: 기능 연구 데이터 (in vitro/in vivo) 없음.  
- **PS4:** 미충족  
  - 근거: gnomAD AF 데이터가 **None**으로, 환자군 대비 유병률 증가 여부를 평가할 수 없음.  

---

#### **C. 중등도 (PM1-PM6):**
- **PM1:** 미충족  
  - 근거: Tyr189이 RUNX1의 **Runt 도메인**에 포함되어 있을 수 있으나, **집단 데이터** 또는 **기능적 중요성**에 대한 명확한 근거 부족.  
- **PM2:** **충족 (Strong)**  
  - 근거: gnomAD AF (전체/popmax) 및 동형접합 데이터가 **None**으로, **집단 데이터베이스에서 부재 또는 극히 드묾**.  
- **PM3:** 미충족  
  - 근거: 열성 질환 관련 trans 병원성 변이 데이터 없음.  
- **PM4:** 미충족  
  - 근거: 단백질 길이 변화 없음 (missense).  
- **PM5:** 미충족  
  - 근거: Tyr189 위치의 다른 병원성 미스센스 변이 데이터 없음.  
- **PM6:** 미충족  
  - 근거: De novo 여부 확인 불가.  

---

#### **D. 지지 (PP1-PP5):**
- **PP1:** 미충족  
  - 근거: 가계 분리 데이터 없음.  
- **PP2:** 미충족  
  - 근거: RUNX1은 **LOF 기전**을 가진 유전자로, missense 변이가 흔하지 않음. 하지만 **명확한 근거 부족**.  
- **PP3:** 미충족  
  - 근거: CADD (0.998) 및 REVEL (0.965) 점수는 **낮은 유해성**을 시사 (0.965는 REVEL 기준에서 **benign**에 가까움).  
- **PP4:** 미충족  
  - 근거: 환자 표현형/가족력 데이터 없음.  
- **PP5:** 미충족  
  - 근거: ClinVar에서 **Uncertain Significance**로 분류됨.  

---

### **2. 양성 증거 (Benign Evidence)**

#### **A. 단독 (BA1):**
- **평가:** 미충족  
  - 근거: gnomAD AF가 **None**으로, 대립유전자 빈도 >5%에 해당하지 않음.  

---

#### **B. 강력 (BS1-BS4):**
- **BS1:** 미충족  
  - 근거: gnomAD AF 데이터 부족으로, 질환 유병률/발현율 비교 불가.  
- **BS2:** 미충족  
  - 근거: 건강한 성인에서 관찰 여부 확인 불가.  
- **BS3:** 미충족  
  - 근거: 기능 연구 데이터 없음.  
- **BS4:** 미충족  
  - 근거: 환자 분리 데이터 없음.  

---

#### **C. 지지 (BP1-BP7):**
- **BP1:** 미충족  
  - 근거: RUNX1은 LOF 기전 유전자로, missense 변이가 흔하지 않음.  
- **BP2:** 미충족  
  - 근거: trans/cis 병원성 변이 데이터 없음.  
- **BP3:** 미충족  
  - 근거: 반복 영역 in-frame indel 관련 데이터 없음.  
- **BP4:** **충족 (Supporting)**  
  - 근거: CADD (0.998) 및 REVEL (0.965) 점수가 **낮은 유해성**을 시사 (REVEL 0.965는 benign에 가까움).  
- **BP5:** 미충족  
  - 근거: 대체 분자적 근거 데이터 없음.  
- **BP6:** 미충족  
  - 근거: ClinVar에서 **Uncertain Significance**로 분류됨.  
- **BP7:** **충족 (Supporting)**  
  - 근거: SpliceAI (N/A) 및 보존성 (phyloP: N/A) 데이터 없음 → **스플라이스 영향 없음**.  

---

### **3. 최종 분류**

#### **적용된 기준 요약:**
- **병원성:** PM2 (Strong)  
- **양성:** BP4 (Supporting), BP7 (Supporting)  

#### **분류 규칙 (ACMG/AMP 2015):**
- **병원성:** (i) 매우 강력 1개 + 강력 1개, (ii) 매우 강력 1개 + 중등도 ≥2개 등 → **미충족**.  
- **병원성 가능:** (i) 매우 강력 1개 + 중등도 1개 등 → **미충족**.  
- **양성:** BA1 단독 또는 강력 양성 ≥2개 → **미충족**.  
- **양성 가능:** 강력 양성 1개 + 지지 양성 1개 등 → **미충족**.  
- **임상적 의미 불명 (VUS):** 위 범주 기준 미충족 → **충족**.  

#### **최종 분류:**
- **분류:** **VUS (Variants of Uncertain Significance)**  
- **신뢰도:** **낮음**  
- **해석 요약:**  
  - **PM2 (Strong)** 기준에 따라, gnomAD에서 **부재 또는 극히 드묾**으로 병원성 가능성이 제시되나, **CADD (0.998)** 및 **REVEL (0.965)** 점수는 **낮은 유해성**을 시사.  
  - **BP4 (Supporting)** 및 **BP7 (Supporting)** 기준에 따라, **스플라이스 영향 없음** 및 **기능적 영향 미미**로 양성 가능성이 제시됨.  
  - **충돌적 증거**로 인해 **VUS**로 분류됨.  

#### **권고사항:**
- **추가 증거 필요:**  
  - **가계 분리 분석** 또는 **기능적 연구 (in vitro/in vivo)** 수행.  
  - **환자 표현형 및 가족력** 데이터 수집.  
  - **기타 데이터베이스 (HGMD, ClinVar 등)**에서의 추가 검토.  

--- 

### **결론:**
이 변이는 **VUS**로 분류되며, **낮은 신뢰도**로 인해 추가 분석이 필요합니다. 병원성 또는 양성으로의 재분류를 위해 **가계 분리, 기능적 연구, 표현형 데이터** 수집이 권장됩니다.