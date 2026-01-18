# MIMIC-III_Data_Analysis

MIMIC-III Clinical Database Demo를 활용한 데이터 분석 프로젝트입니다.

## 📋 목차

- [시작하기](#시작하기)
- [데이터 설명](#데이터-설명)
- [프로젝트 구조](#프로젝트-구조)

## 🚀 시작하기

### How to Start: Download and Open in Colab

튜토리얼 노트북을 실행하려면 다음 단계를 따르세요:

#### [Step 1: GitHub 저장소 다운로드]

1. GitHub 저장소 페이지에서 초록색 **Code** 버튼(우측 상단)을 클릭합니다.
2. **Download ZIP**을 선택합니다.
3. 다운로드한 ZIP 파일을 로컬 컴퓨터에서 압축 해제합니다.

#### [Step 2: Colab에서 노트북 열기]

1. [Google Colab](https://colab.research.google.com/)에 접속합니다.
2. 우측 상단의 **Open Colab** 버튼을 클릭합니다.
3. **Upload** 탭을 선택하고 압축 해제한 폴더에서 튜토리얼 노트북 파일을 업로드합니다.
   - `MIMIC_III_Tutorial.ipynb`
4. 업로드가 완료되면 노트북이 열리며 Colab에서 바로 실행할 수 있습니다.

## 📊 데이터 설명

본 프로젝트에서 사용하는 데이터는 [MIMIC-III Clinical Database Demo v1.4](https://physionet.org/content/mimiciii-demo/1.4/)에서 가져온 것입니다.

MIMIC-III는 2001년부터 2012년까지 Beth Israel Deaconess Medical Center의 중환자실(ICU)에 입원한 40,000명 이상의 환자와 관련된 비식별화된 건강 관련 데이터를 포함하는 대규모 공개 데이터베이스입니다. Demo 버전은 전체 데이터베이스의 구조와 내용을 검토할 수 있도록 100명의 환자 데이터로 구성된 샘플 데이터셋입니다.

### 데이터 파일 설명

| 파일명 | 설명 | 크기 (예시) |
|--------|------|------------|
| `patients.csv` | 환자 기본 정보 (인구통계학적 데이터, 생년월일, 사망일 등) | ~8.4 KB |
| `patient_admissions.csv` | 입원 기록 정보 (입원일, 퇴원일, 입원 유형, 진단 등) | ~26.2 KB |
| `patient_discharges.csv` | 퇴원 정보 (퇴원 상태, 퇴원 후 처방 등) | 포함됨 |
| `patient_transfers.csv` | 환자 전원 기록 (병동 간 이동, ICU 입실/퇴실 등) | ~46.1 KB |

### 데이터 출처

- **원본 데이터베이스**: MIMIC-III Clinical Database Demo v1.4
- **제공 기관**: PhysioNet
- **DOI**: [10.13026/C2HM2Q](https://doi.org/10.13026/C2HM2Q)
- **라이선스**: Open Data Commons Open Database License v1.0

### 인용 방법

본 데이터를 사용할 경우 다음 논문을 인용해주세요:

```
Johnson, A. E. W., Pollard, T. J., Shen, L., Lehman, L. H., Feng, M., Ghassemi, M., 
Moody, B., Szolovits, P., Celi, L. A., & Mark, R. G. (2016). 
MIMIC-III, a freely accessible critical care database. 
Scientific Data, 3, 160035.
```

## 📚 참고 자료

- [MIMIC-III 공식 웹사이트](https://mimic.physionet.org)
- [PhysioNet MIMIC-III Demo 페이지](https://physionet.org/content/mimiciii-demo/1.4/)
- [MIMIC-III 논문](https://www.nature.com/articles/sdata201635)

## ⚠️ 주의사항

- 본 데이터는 비식별화되었지만 실제 환자 데이터를 기반으로 하므로, 데이터 사용 시 관련 규정 및 윤리 가이드라인을 준수해야 합니다.
- Demo 버전은 전체 데이터베이스의 일부 샘플이므로, 연구 목적에 따라 전체 데이터베이스 접근이 필요할 수 있습니다.
- 전체 MIMIC-III 데이터베이스 접근을 위해서는 PhysioNet에서 자격 인증이 필요합니다.
