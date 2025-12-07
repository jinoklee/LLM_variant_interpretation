# Variant Analysis Report #10

**Gene:** HNF4A

**Variant:** NM_175914.5:c.1063G>A

---

<think>
Okay, let's tackle this variant interpretation for HNF4A c.1063G>A (p.Gly355Arg). First, I need to recall the ACMG/AMP 2015 guidelines and the ClinGen SVI recommendations. The user provided all the necessary data, so I should go through each criterion step by step.

Starting with PVS1 (Probably Pathogenic Variant in a Splice Site). The variant is a missense, not a splice site, so PVS1 doesn't apply here. Next, PS1-4 (Population Frequency). The gnomAD data is all "None," which might mean it's not present in the database. But I need to check if that's because it's a rare variant or if there's no data. If it's not in gnomAD, that could support a pathogenic classification, but I should note that absence of data might not be conclusive.

For PS3 (Population Frequency in Affected vs. Unaffected), there's no data here, so PS3 isn't applicable. Moving to PM1 (Location in a Region of Interest). The variant is in HNF4A, which is associated with maturity-onset diabetes of the young (MODY). The position is p.Gly355Arg. I need to check if this residue is in a conserved domain. The user mentioned phyloP is N/A, so maybe there's no conservation data. However, HNF4A is a transcription factor, and certain residues might be critical. If this is a conserved residue, that would support PM1, but without phyloP, I can't confirm. Maybe I should mention that the lack of conservation data is a limitation.

PM2 (Missense in a Critical and Well-Conserved Residue). Again, without phyloP, I can't assess conservation. But if the residue is in a functional domain, that might be PM2. However, without evidence, this is uncertain. PM3 (Functional Studies) – no in vitro or in vivo data, so PM3 doesn't apply. PM4 (Predicted to Affect Protein Function) – CADD is 0.997, which is very low, and REVEL is 0.565, which is below the threshold for pathogenicity (usually >0.7). So these predictions suggest the variant is not damaging. That would go against PM4.

PP1 (De Novo in Affected Individual) – no de novo data. PP2 (Missense in Gene with Known Pathogenic Variants) – HNF4A has known pathogenic variants, but this is a missense. However, the prediction scores are low, which might suggest it's not pathogenic. PP3 (Functional Studies) – no data. PP4 (Recessive Disease with Two Variants) – not applicable here. PP5 (Multiple Independent Lines of Evidence) – not applicable.

BA1 (Allele Frequency in Controls) – gnomAD AF is None, which might be considered as very low frequency, but without specific numbers, it's hard to say. BS1 (Allele Frequency in Controls) – same as BA1. BS2 (Not Observed in Exome/Genome Sequencing of Controls) – if the variant isn't in gnomAD, that could be BS2. But again, the absence of data is tricky. BS3 (Population Frequency in Controls) – similar to BS2. BP1 (Not in a Known Disease Gene) – HNF4A is a known disease gene, so BP1 doesn't apply. BP2 (Missense in a Non-Critical Residue) – if the residue isn't critical, but without conservation data, this is uncertain. BP3 (Predicted to Be Benign) – CADD and REVEL suggest benign, so BP3 applies. BP4 (Not in a Functional Domain) – if the residue isn't in a functional domain, but again, without data, this is unclear. BP5 (Not in a Region of Interest) – same as BP4.

Now, applying ClinGen SVI for PS3/BS3. Since there's no population data, PS3 isn't applicable. For BS3, if the variant is not in controls, but the absence of data is ambiguous. However, the low CADD and REVEL scores support benign.

Putting it all together: The variant is a missense in HNF4A, but the computational predictions are not pathogenic. No population data, but absence might be considered. However, the lack of conservation data and functional studies makes it hard to confirm. The most applicable criteria are BP3 (predicted benign) and possibly BS2 (not in controls). But since the absence of data is uncertain, the classification might be VUS. However, the low CADD and REVEL scores might lean towards benign. But without strong evidence, it's uncertain. So the final classification is likely VUS with low confidence.
</think>

### ACMG/AMP 2015 기준 및 ClinGen SVI 권고안에 따른 변이 해석

---

#### **1. 변이 정보 요약**
- **유전자**: `HNF4A` (MODY 유발 유전자, 전사 인자)
- **변이**: `NM_175914.5:c.1063G>A` (p.Gly355Arg)
- **유형**: Missense
- **기능 영역**: Glycine (Gly) → Arginine (Arg) 변이 (355번 아미노산)

---

#### **2. ACMG/AMP 2015 기준 평가**

| **기준** | **충족 여부** | **근거** |
|----------|----------------|----------|
| **PVS1** | ❌ | Splice site 변이가 아님. |
| **PS1** | ❌ | gnomAD AF (전체) 및 popmax 데이터 없음 (결여 데이터로 판단 불가). |
| **PS2** | ❌ | 특정 인종/인구집단에서의 높은 빈도 데이터 없음. |
| **PS3** | ❌ | 환자군 vs. 대조군의 빈도 비교 데이터 없음. |
| **PS4** | ❌ | 특정 인구집단에서의 높은 빈도 데이터 없음. |
| **PM1** | ❌ | 보존성 데이터 (phyloP) 없음. Gly355의 보존성 확인 불가. |
| **PM2** | ❌ | 기능적 영역 (예: DNA 결합 영역) 위치 확인 불가. |
| **PM3** | ❌ | 기능 연구 (in vitro/in vivo) 데이터 없음. |
| **PM4** | ❌ | CADD (0.997) 및 REVEL (0.565) 예측이 **비병원성**을 지지 (CADD < 10, REVEL < 0.7). |
| **PP1** | ❌ | de novo 데이터 없음. |
| **PP2** | ❌ | HNF4A는 MODY 유발 유전자이지만, missense 변이의 병리성 확정 불가. |
| **PP3** | ❌ | 기능 연구 데이터 없음. |
| **PP4** | ❌ | 열성 질환 관련 데이터 없음. |
| **PP5** | ❌ | 다중 증거 없음. |
| **BA1** | ❌ | gnomAD AF 데이터 결여로 판단 불가. |
| **BS1** | ❌ | gnomAD AF 데이터 결여로 판단 불가. |
| **BS2** | ✅ | gnomAD에 등록되지 않음 (결여 데이터로 병리성 가능성이 낮음). |
| **BS3** | ❌ | 인구집단 빈도 데이터 없음. |
| **BP1** | ❌ | HNF4A는 MODY 유발 유전자이므로 적용 불가. |
| **BP2** | ❌ | Gly355의 기능적 중요성 확인 불가. |
| **BP3** | ✅ | CADD (0.997) 및 REVEL (0.565) 예측이 **비병원성**을 지지. |
| **BP4** | ❌ | 기능적 영역 위치 확인 불가. |
| **BP5** | ❌ | 기능적 영역 위치 확인 불가. |

---

#### **3. ClinGen SVI 권고안 적용**
- **PS3/BS3 강도 조절**:  
  - **PS3** (환자군 vs. 대조군 빈도 비교): 데이터 없음 → 적용 불가.  
  - **BS3** (인구집단 빈도): gnomAD에 등록되지 않음 → **BS2** (결여 데이터)로 대체.  
  - **PVS1 강도 조절**: missense 변이이므로 PVS1 적용 불가.

---

#### **4. 최종 분류 및 신뢰도**
- **분류**: **VUS (Variants of Uncertain Significance)**  
- **신뢰도**: **낮음**  
- **임상적 해석**:  
  - **비병원성 예측**: CADD (0.997) 및 REVEL (0.565)이 병리성 가능성을 낮게 평가.  
  - **결여 데이터**: gnomAD에 등록되지 않음 (BS2)으로 병리성 가능성이 낮으나, 보존성 및 기능적 영역 데이터 부족으로 확정 불가.  
  - **HNF4A의 기능적 중요성**: Gly355의 보존성 및 기능적 영역 확인 불가.  
  - **결론**: 현재 증거로는 병리성 또는 무해성 확정 불가 → **VUS** 분류.

---

#### **5. 추가 검토 필요 사항**
- **보존성 분석**: phyloP 또는 다른 보존성 도구로 Gly355의 보존성 확인 필요.  
- **기능적 연구**: in vitro/in vivo 실험으로 변이의 기능적 영향 평가 필요.  
- **가계 분석**: 가족 내 유전자 분리 및 임상 증상 연관성 확인 필요.  

--- 

**참고**: ClinGen SVI 권고안에 따라, 결여 데이터는 **BS2**로 처리되며, 예측 도구의 결과는 **BP3**으로 적용. 그러나 보존성 및 기능적 데이터 부족으로 인해 최종 분류는 **VUS**로 유지.