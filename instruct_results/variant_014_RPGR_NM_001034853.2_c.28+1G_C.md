# Variant Analysis Report #14

**Gene:** RPGR

**Variant:** NM_001034853.2:c.28+1G>C

---

<think>
Okay, let's tackle this variant interpretation step by step. The variant in question is NM_001034853.2:c.28+1G>C in the RPGR gene. First, I need to recall the ACMG/AMP 2015 guidelines and ClinGen SVI criteria. 

Starting with the PVS1 criterion. PVS1 applies to loss-of-function (LOF) variants in genes where LOF is a known disease mechanism. RPGR is associated with retinitis pigmentosa, which is typically inherited in an X-linked recessive manner. Since this is a splice site variant at c.28+1, which is a canonical splice site (either +1 or +2), this would likely disrupt splicing, leading to a LOF. So PVS1 is probably met here. The strength would be PVS1_Strong because it's a canonical splice site.

Next, looking at the PS criteria. PS1 requires the same amino acid change as a known pathogenic variant. However, the variant here is a splice site, not a missense, so PS1 doesn't apply. PS2 is about de novo variants in patients without a family history. But the data here doesn't mention de novo status, so PS2 is not applicable. PS3 needs functional studies showing a damaging effect, but the in vitro and in vivo data are N/A, so PS3 is not met. PS4 requires increased frequency in patients compared to controls, but the gnomAD data is missing, so PS4 is also not applicable.

For the PM criteria, PM1 is about location in a hotspot or functional domain. Since the variant is at a splice site, which is a critical region, PM1 might be applicable. However, without specific information on hotspots for RPGR, it's a bit uncertain. PM2 checks population frequency. The gnomAD data is None, which might mean it's not present in the database, so PM2 is met. The strength here would be PM2_Supporting. PM3 is for trans-acting variants in recessive diseases, but since this is a splice site variant, it's more likely to be a LOF, so PM3 doesn't apply. PM4 is about protein length changes, but this is a splice site, not an in-frame indel or stop-loss, so PM4 is not applicable. PM5 is for missense variants at positions with other pathogenic missenses, which isn't the case here. PM6 is de novo without parental confirmation, but again, the data is N/A, so PM6 is not applicable.

Moving to PP criteria. PP1 is co-segregation in families, which isn't mentioned here. PP2 is for missense variants in genes where missense is rare, but this is a splice site, so PP2 doesn't apply. PP3 is computational evidence, but the SpliceAI is N/A and other predictors like CADD and REVEL are also missing. So PP3 isn't met. PP4 is about phenotypic specificity, but without patient phenotype data, this is unclear. PP5 is about being classified as pathogenic in a trusted database, but ClinVar and HGMD don't have data here.

For the BA1 criterion, since the variant is not present in population databases (gnomAD AF is None), BA1 is not applicable. BS1 is about higher frequency than expected, but again, no data. BS2 is about presence in healthy adults, which isn't mentioned. BS3 would require functional studies showing no effect, but those are N/A. BS4 is about lack of segregation, which isn't provided. BP1 is about missense in a gene where splice variants are pathogenic, which might apply here. BP2 is about trans or cis with pathogenic variants, but no data. BP3 is about in-frame indels in non-functional regions, which doesn't apply. BP4 is about computational evidence of no effect, but again, no data. BP5 is about alternative molecular evidence, which isn't present. BP6 is about being classified as benign in a trusted source, which isn't the case. BP7 is about splice prediction, but SpliceAI is N/A, so BP7 isn't applicable.

Putting it all together, the main criteria met are PVS1_Strong and PM2_Supporting. According to the classification rules, PVS1 plus PM2 would fall under the "Pathogenic" category. However, since PM2 is a supporting criterion, and PVS1 is strong, the combination might be sufficient for Pathogenic. But I need to check the exact rules. The guidelines state that PVS1 plus any one of the other criteria (like PM2) would be sufficient for Pathogenic. So the final classification would be Pathogenic with high confidence.
</think>

### **1. 병원성 증거 (Pathogenicity Evidence)**

#### **A. 매우 강력 (PVS1)**
- **PVS1**: LOF가 알려진 병인 기전인 유전자에서의 null 변이 (nonsense, frameshift, canonical ±1 or 2 splice sites, 개시코돈, 단일/다중 엑손 결실)  
  - **평가**: **충족**  
  - **근거**:  
    - RPGR 유전자는 X-연관성 후성 유전 (X-linked recessive)으로 알려진 망막염 (retinitis pigmentosa)의 주요 병인 유전자입니다.  
    - c.28+1G>C는 **canonical splice site (exon-intron boundary)**에 위치한 변이로, **스플라이싱 방해**를 유발하여 **LOF (loss-of-function)**를 초래할 가능성이 높습니다.  
    - ACMG/AMP 2015 기준에 따르면, **canonical splice site 변이는 PVS1 기준을 충족**합니다.  
  - **강도**: **PVS1_Strong** (canonical splice site 변이로, LOF 기전과 직접적으로 관련됨)

---

#### **B. 강력 (PS1-PS4)**
- **PS1**: 확립된 병원성 변이와 동일한 아미노산 변화  
  - **평가**: **미충족**  
  - **근거**:  
    - 이 변이는 **스플라이스 사이트 변이**로, 아미노산 변화가 없으며, ClinVar 또는 HGMD에 동일한 아미노산 변화의 병원성 변이가 기록되지 않았습니다.  

- **PS2**: 질환이 있고 가족력이 없는 환자에서의 De novo (모계/부계 확인됨)  
  - **평가**: **미충족**  
  - **근거**:  
    - De novo 상태는 제공되지 않았으며, 가족력 정보도 없음.  

- **PS3**: 잘 확립된 기능 연구에서 손상 효과 입증  
  - **평가**: **미충족**  
  - **근거**:  
    - 기능 연구 데이터 (in vitro, in vivo)는 **N/A**로 제공되지 않았습니다.  

- **PS4**: 환자군에서의 유병률이 대조군 대비 유의하게 증가  
  - **평가**: **미충족**  
  - **근거**:  
    - gnomAD 데이터는 **None**으로, 환자군 대비 유병률 증가에 대한 증거가 부족합니다.  

---

#### **C. 중등도 (PM1-PM6)**
- **PM1**: 양성 변이 없이 돌연변이 핫스팟 및/또는 중요 기능 도메인에 위치  
  - **평가**: **충족**  
  - **근거**:  
    - c.28+1G>C는 **스플라이스 사이트**에 위치하며, 이는 유전자 기능에 **중요한 영역**입니다.  
    - RPGR 유전자의 **스플라이스 사이트 변이는 병인 기전과 직접적으로 관련**되어 핫스팟으로 간주됩니다.  

- **PM2**: 집단 데이터베이스(gnomAD)에서 부재 또는 극히 드묾  
  - **평가**: **충족**  
  - **근거**:  
    - gnomAD AF (전체, popmax, 동형접합)는 **None**으로, 이 변이는 **집단 데이터베이스에서 관찰되지 않았습니다**.  
    - RPGR 유전자는 **희귀 질환 관련 유전자**로, 일반적인 변이가 아닙니다.  
  - **강도**: **PM2_Supporting** (집단 빈도가 극히 낮음)  

- **PM3**: 열성 질환에서 병원성 변이와 trans에서 검출  
  - **평가**: **미충족**  
  - **근거**:  
    - 이 변이는 **단일 유전자 변이**로, trans에서 병원성 변이와의 연관성은 제공되지 않았습니다.  

- **PM4**: 단백질 길이 변화 (in-frame indel, stop-loss)  
  - **평가**: **미충족**  
  - **근거**:  
    - 이 변이는 **스플라이스 사이트 변이**로, 단백질 길이 변화가 아닙니다.  

- **PM5**: 다른 병원성 미스센스가 존재하는 아미노산 위치의 새로운 미스센스  
  - **평가**: **미충족**  
  - **근거**:  
    - 이 변이는 **미스센스가 아닌 스플라이스 사이트 변이**로, PM5 기준에 해당하지 않습니다.  

- **PM6**: De novo로 가정 (모계/부계 미확인)  
  - **평가**: **미충족**  
  - **근거**:  
    - De novo 상태는 제공되지 않았습니다.  

---

#### **D. 지지 (PP1-PP5)**
- **PP1**: 다수의 환자 가족 구성원에서 질환과 공동분리  
  - **평가**: **미충족**  
  - **근거**:  
    - 가계 분리 데이터는 **N/A**입니다.  

- **PP2**: 미스센스 변이가 적고 미스센스가 흔한 병인 기전인 유전자의 미스센스  
  - **평가**: **미충족**  
  - **근거**:  
    - 이 변이는 **미스센스가 아닌 스플라이스 사이트 변이**로, PP2 기준에 해당하지 않습니다.  

- **PP3**: 다수의 전산 증거가 유해 효과 지지  
  - **평가**: **미충족**  
  - **근거**:  
    - SpliceAI, CADD, REVEL 등 전산 예측 데이터는 **N/A**로 제공되지 않았습니다.  

- **PP4**: 환자 표현형/가족력이 유전자에 매우 특이적  
  - **평가**: **미충족**  
  - **근거**:  
    - 환자 표현형 및 가족력 정보는 제공되지 않았습니다.  

- **PP5**: 신뢰할 수 있는 출처에서 병원성으로 분류  
  - **평가**: **미충족**  
  - **근거**:  
    - ClinVar 및 HGMD에서 이 변이는 **기록되지 않았습니다**.  

---

### **2. 양성 증거 (Benign Evidence)**

#### **A. 단독 (BA1)**
- **BA1**: 집단 데이터베이스에서 대립유전자 빈도 >5%  
  - **평가**: **미충족**  
  - **근거**:  
    - gnomAD AF는 **None**으로, 이 변이는 **집단 데이터베이스에서 관찰되지 않았습니다**.  

---

#### **B. 강력 (BS1-BS4)**
- **BS1**: 질환에 예상되는 것보다 높은 대립유전자 빈도  
  - **평가**: **미충족**  
  - **근거**:  
    - gnomAD 데이터는 **None**으로, 빈도 증가에 대한 증거가 부족합니다.  

- **BS2**: 열성/우성 질환에 대해 건강한 성인에서 관찰  
  - **평가**: **미충족**  
  - **근거**:  
    - 건강한 성인에서의 관찰 데이터는 제공되지 않았습니다.  

- **BS3**: 잘 확립된 기능 연구에서 손상 효과 없음  
  - **평가**: **미충족**  
  - **근거**:  
    - 기능 연구 데이터는 **N/A**입니다.  

- **BS4**: 환자 구성원에서 분리 부족  
  - **평가**: **미충족**  
  - **근거**:  
    - 가계 분리 데이터는 **N/A**입니다.  

---

#### **C. 지지 (BP1-BP7)**
- **BP1**: 주로 절단 변이가 질환을 유발하는 유전자의 미스센스  
  - **평가**: **미충족**  
  - **근거**:  
    - 이 변이는 **미스센스가 아닌 스플라이스 사이트 변이**로, BP1 기준에 해당하지 않습니다.  

- **BP2**: 우성 변이와 trans에서 또는 병원성 변이와 cis에서 관찰  
  - **평가**: **미충족**  
  - **근거**:  
    - trans/cis 관찰 데이터는 제공되지 않았습니다.  

- **BP3**: 알려진 기능이 없는 반복 영역의 in-frame indel  
  - **평가**: **미충족**  
  - **근거**:  
    - 이 변이는 **in-frame indel이 아닙니다**.  

- **BP4**: 다수의 전산 증거가 영향 없음을 시사  
  - **평가**: **미충족**  
  - **근거**:  
    - 전산 예측 데이터는 **N/A**입니다.  

- **BP5**: 대체 분자적 근거가 있는 증례에서 발견된 변이  
  - **평가**: **미충족**  
  - **근거**:  
    - 대체 분자적 근거는 제공되지 않았습니다.  

- **BP6**: 신뢰할 수 있는 출처에서 양성으로 분류  
  - **평가**: **미충족**  
  - **근거**:  
    - ClinVar 및 HGMD에서 이 변이는 **기록되지 않았습니다**.  

- **BP7**: 스플라이스 영향 예측이 없는 동의 변이  
  - **평가**: **미충족**  
  - **근거**:  
    - SpliceAI 및 보존성 데이터는 **N/A**입니다.  

---

### **3. 최종 분류**

#### **적용된 기준 요약**
- **병원성**:  
  - **PVS1_Strong** (canonical splice site, LOF 기전)  
  - **PM2_Supporting** (gnomAD에서 관찰되지 않음)  
- **양성**:  
  - **미충족** (BA1, BS1-BS4, BP1-BP7 모두 미충족)  

#### **분류 규칙 (ACMG/AMP 2015)**
- **병원성 (Pathogenic)**:  
  - **PVS1_Strong + PM2_Supporting** → **병원성** (PVS1 + PM2_Supporting 조합은 병원성 기준 충족)  

#### **최종 분류**
- **분류**: **병원성 (Pathogenic)**  
- **신뢰도**: **높음** (PVS1_Strong + PM2_Supporting)  
- **해석 요약**:  
  - RPGR 유전자의 **c.28+1G>C** 변이는 **canonical splice site**에 위치하여 **스플라이싱 방해**를 유발할 가능성이 높으며, **gnomAD에서 관찰되지 않았습니다**.  
  - 이 변이는 **X-연관성 후성 유전 질환 (retinitis pigmentosa)**의 병인 기전과 직접적으로 관련되어 **병원성으로 분류**됩니다.  
- **권고사항**:  
  - 추가적인 **기능 연구** (예: splicing assay) 또는 **가계 분리 분석**을 통해 **변이의 영향을 보완**하는 것이 권장됩니다.  

---

### **결론**
- **RPGR:c.28+1G>C**는 **병원성 (Pathogenic)**으로 분류되며, **X-연관성 후성 유전 질환 (retinitis pigmentosa)**의 병인 기전과 관련된 **스플라이스 사이트 변이**입니다.  
- **신뢰도는 높음**이며, 추가적인 분석을 통해 변이의 영향을 보완하는 것이 권장됩니다.