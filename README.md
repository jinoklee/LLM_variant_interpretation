**prompt: ACMG/AMP 기반 변이 해석 지시 유무에 따른 결과**

---

**PPT 코드 및 결과**   
- 위치: PPT/
- 코드: qwen_LLM_simple.ipynb
- 결과: variants_results.md, variant_instruct_results.md

---

**VEP annotation 파일: variants.annot.txt** 

1. 단순 해석요구 :
   - 위치: results/
   - 코드: qwen_LLM_vep_annotation_results.ipynb
   - 결과: *md
  ```
      def analyze_variant_simple(model, variant_info):
              """ACMG/AMP 2015 변이 분석 """
              prompt = f"""당신은 ACMG/AMP 2015 가이드라인과 ClinGen Sequence Variant Interpretation (SVI) 권고안에 따라 변이 해석을 수행하는 임상 유전학 전문가입니다.
      
      변이 정보:
      유전자: {variant_info.get('gene')}
      변이: {variant_info.get('variant')}
      유형: {variant_info.get('type')}
      cDNA: {variant_info.get('cdna', 'N/A')}
      단백질: {variant_info.get('protein', 'N/A')}
      
      증거 데이터:
      집단 데이터:
      - gnomAD AF (전체): {variant_info.get('gnomad_af', 'Unknown')}
      - gnomAD AF (popmax): {variant_info.get('gnomad_popmax', 'Unknown')}
      - gnomAD 동형접합: {variant_info.get('gnomad_hom', 'Unknown')}
      
      데이터베이스 증거:
      - ClinVar: {variant_info.get('clinvar', 'Not found')}
      - HGMD: {variant_info.get('hgmd', 'Not available')}
      
      전산 예측:
      - CADD: {variant_info.get('cadd', 'N/A')}
      - REVEL: {variant_info.get('revel', 'N/A')}
      - SpliceAI: {variant_info.get('spliceai', 'N/A')}
      - 보존성 (phyloP): {variant_info.get('phylop', 'N/A')}
      
      기능 연구:
      - In vitro 데이터: {variant_info.get('functional', 'N/A')}
      - In vivo 데이터: {variant_info.get('in_vivo', 'N/A')}
      
      가계 분리 및 증례 데이터:
      - 가계 분리: {variant_info.get('segregation', 'N/A')}
      - De novo: {variant_info.get('de_novo', 'N/A')}
      - 환자-대조군 연구: {variant_info.get('case_control', 'N/A')}
      
      과제: ACMG/AMP 2015 기준을 체계적으로 평가하세요. 각 기준(PVS1, PS1-4, PM1-6, PP1-5, BA1, BS1-4, BP1-7)에 대해 충족 여부를 증거와 근거와 함께 명시하세요. PS3/BS3와 PVS1 강도 조절에 대한 ClinGen SVI 권고안을 적용하세요. 최종 분류(병원성/병원성 가능/VUS/양성 가능/양성)를 신뢰도 및 임상적 해석과 함께 제공하세요."""
              
              return chat(model, prompt, max_tokens=30000, temperature=0.2)
  ```

2. 해석 지시 및 결과 구조화
   - 위치: instruct_results/
   - 코드: qwen_LLM_vep_annotation_instruct_results.ipynb
   - 결과: *.md
  ```
      def analyze_variant(model, variant_info):
              """ACMG/AMP 2015 변이 분석"""
              prompt = f"""당신은 ACMG/AMP 2015 가이드라인과 ClinGen Sequence Variant Interpretation (SVI) 권고안에 따라 변이 해석을 수행하는 임상 유전학 전문가입니다.
      
      변이 정보:
      유전자: {variant_info.get('gene')}
      변이: {variant_info.get('variant')}
      유형: {variant_info.get('type')}
      cDNA: {variant_info.get('cdna', 'N/A')}
      단백질: {variant_info.get('protein', 'N/A')}
      
      증거 데이터:
      집단 데이터:
      - gnomAD AF (전체): {variant_info.get('gnomad_af', 'Unknown')}
      - gnomAD AF (popmax): {variant_info.get('gnomad_popmax', 'Unknown')}
      - gnomAD 동형접합: {variant_info.get('gnomad_hom', 'Unknown')}
      
      데이터베이스 증거:
      - ClinVar: {variant_info.get('clinvar', 'Not found')}
      - HGMD: {variant_info.get('hgmd', 'Not available')}
      
      전산 예측:
      - CADD: {variant_info.get('cadd', 'N/A')}
      - REVEL: {variant_info.get('revel', 'N/A')}
      - SpliceAI: {variant_info.get('spliceai', 'N/A')}
      - 보존성 (phyloP): {variant_info.get('phylop', 'N/A')}
      
      기능 연구:
      - In vitro 데이터: {variant_info.get('functional', 'N/A')}
      - In vivo 데이터: {variant_info.get('in_vivo', 'N/A')}
      
      가계 분리 및 증례 데이터:
      - 가계 분리: {variant_info.get('segregation', 'N/A')}
      - De novo: {variant_info.get('de_novo', 'N/A')}
      - 환자-대조군 연구: {variant_info.get('case_control', 'N/A')}
      
      과제: ACMG/AMP 2015 기준 체계적 평가
      
      1. 병원성 증거:
      
         A. 매우 강력 (PVS1):
            - PVS1: LOF가 알려진 병인 기전인 유전자에서의 null 변이 (nonsense, frameshift, canonical ±1 or 2 splice sites, 개시코돈, 단일/다중 엑손 결실)
            → 평가: [충족/미충족]
            → 근거: [상세한 근거]
            → 강도: [PVS1, PVS1_Strong, PVS1_Moderate, PVS1_Supporting, 또는 미충족]
      
         B. 강력 (PS1-PS4):
            - PS1: 확립된 병원성 변이와 동일한 아미노산 변화
            → 평가: [충족/미충족]
            → 근거:
            
            - PS2: 질환이 있고 가족력이 없는 환자에서의 De novo (모계/부계 확인됨)
            → 평가: [충족/미충족]
            → 근거:
            
            - PS3: 잘 확립된 기능 연구에서 손상 효과 입증 (ClinGen SVI 기준)
            → 평가: [충족/미충족]
            → 근거: [고려사항: 검증된 분석법, 재현성, 기능적 효과 입증]
            → 강도: [PS3, PS3_Moderate, PS3_Supporting, 또는 미충족]
            
            - PS4: 환자군에서의 유병률이 대조군 대비 유의하게 증가
            → 평가: [충족/미충족]
            → 근거:
      
         C. 중등도 (PM1-PM6):
            - PM1: 양성 변이 없이 돌연변이 핫스팟 및/또는 중요 기능 도메인에 위치
            → 평가: [충족/미충족]
            → 근거:
            
            - PM2: 집단 데이터베이스(gnomAD)에서 부재 또는 극히 드묾
            → 평가: [충족/미충족]
            → 근거: [질환 유병률 및 발현율 고려]
            → 강도: [PM2, PM2_Supporting, 또는 미충족]
            
            - PM3: 열성 질환에서 병원성 변이와 trans에서 검출
            → 평가: [충족/미충족]
            → 근거:
            
            - PM4: 단백질 길이 변화 (in-frame indel, stop-loss)
            → 평가: [충족/미충족]
            → 근거:
            
            - PM5: 다른 병원성 미스센스가 존재하는 아미노산 위치의 새로운 미스센스
            → 평가: [충족/미충족]
            → 근거:
            
            - PM6: De novo로 가정 (모계/부계 미확인)
            → 평가: [충족/미충족]
            → 근거:
      
         D. 지지 (PP1-PP5):
            - PP1: 다수의 환자 가족 구성원에서 질환과 공동분리
            → 평가: [충족/미충족]
            → 근거:
            
            - PP2: 미스센스 변이가 적고 미스센스가 흔한 병인 기전인 유전자의 미스센스
            → 평가: [충족/미충족]
            → 근거:
            
            - PP3: 다수의 전산 증거가 유해 효과 지지
            → 평가: [충족/미충족]
            → 근거: [REVEL, BayesDel 같은 메타 예측자 고려]
            
            - PP4: 환자 표현형/가족력이 유전자에 매우 특이적
            → 평가: [충족/미충족]
            → 근거:
            
            - PP5: 신뢰할 수 있는 출처에서 병원성으로 분류
            → 평가: [충족/미충족]
            → 근거:
      
      2. 양성 증거:
      
         A. 단독 (BA1):
            - BA1: 집단 데이터베이스에서 대립유전자 빈도 >5%
            → 평가: [충족/미충족]
            → 근거:
      
         B. 강력 (BS1-BS4):
            - BS1: 질환에 예상되는 것보다 높은 대립유전자 빈도
            → 평가: [충족/미충족]
            → 근거: [질환 유병률, 발현율, 유전적 이질성 고려]
            
            - BS2: 열성/우성 질환에 대해 건강한 성인에서 관찰
            → 평가: [충족/미충족]
            → 근거:
            
            - BS3: 잘 확립된 기능 연구에서 손상 효과 없음 (ClinGen SVI 기준)
            → 평가: [충족/미충족]
            → 근거: [고려사항: 검증된 분석법, 재현성, 기능적 효과 없음]
            → 강도: [BS3, BS3_Moderate, BS3_Supporting, 또는 미충족]
            
            - BS4: 환자 구성원에서 분리 부족
            → 평가: [충족/미충족]
            → 근거:
      
         C. 지지 (BP1-BP7):
            - BP1: 주로 절단 변이가 질환을 유발하는 유전자의 미스센스
            → 평가: [충족/미충족]
            → 근거:
            
            - BP2: 우성 변이와 trans에서 또는 병원성 변이와 cis에서 관찰
            → 평가: [충족/미충족]
            → 근거:
            
            - BP3: 알려진 기능이 없는 반복 영역의 in-frame indel
            → 평가: [충족/미충족]
            → 근거:
            
            - BP4: 다수의 전산 증거가 영향 없음을 시사
            → 평가: [충족/미충족]
            → 근거:
            
            - BP5: 대체 분자적 근거가 있는 증례에서 발견된 변이
            → 평가: [충족/미충족]
            → 근거:
            
            - BP6: 신뢰할 수 있는 출처에서 양성으로 분류
            → 평가: [충족/미충족]
            → 근거:
            
            - BP7: 스플라이스 영향 예측이 없는 동의 변이
            → 평가: [충족/미충족]
            → 근거: [SpliceAI, 보존성 고려]
      
      3. 최종 분류:
      
         적용된 기준 요약:
         - 병원성: [충족된 모든 병원성 기준과 강도 나열]
         - 양성: [충족된 모든 양성 기준과 강도 나열]
      
         분류 규칙 (ACMG/AMP 2015):
         - 병원성 (Pathogenic): (i) 매우 강력 1개 + 강력 1개, 또는 (ii) 매우 강력 1개 + 중등도 ≥2개, 또는 (iii) 매우 강력 1개 + 중등도 1개 + 지지 1개, 또는 (iv) 강력 2개, 또는 (v) 강력 1개 + 중등도 ≥3개, 또는 (vi) 강력 1개 + 중등도 2개 + 지지 ≥2개
         - 병원성 가능 (Likely Pathogenic): (i) 매우 강력 1개 + 중등도 1개, 또는 (ii) 강력 1개 + 중등도 1-2개, 또는 (iii) 강력 1개 + 지지 ≥2개, 또는 (iv) 중등도 ≥3개, 또는 (v) 중등도 2개 + 지지 ≥2개, 또는 (vi) 중등도 1개 + 지지 ≥4개
         - 양성 (Benign): BA1 단독 또는 강력 양성 ≥2개
         - 양성 가능 (Likely Benign): 강력 양성 1개 + 지지 양성 1개 또는 지지 양성 ≥2개
         - 임상적 의미 불명 (VUS): 위 범주 기준 미충족
      
         최종 분류: [병원성/병원성 가능/VUS/양성 가능/양성]
         
         신뢰도: [높음/중등도/낮음]
         
         해석 요약: [간략한 임상적 해석]
         
         권고사항: [VUS인 경우 추가 증거 또는 검사 제안]
      
      체계적 분석을 시작하세요:"""
              
              return chat(model, prompt, max_tokens=30000, temperature=0.2)
  
  ```
