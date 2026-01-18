# MIMIC-IV_Data_Analysis

MIMIC-IV Clinical Database Demo를 활용한 데이터 분석 프로젝트입니다.


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
   - `MIMIC_IV_Tutorial.ipynb`
4. 업로드가 완료되면 노트북이 열리며 Colab에서 바로 실행할 수 있습니다.

> **참고**: 노트북을 실행하면 자동으로 GitHub에서 데이터 파일을 다운로드하여 Google Drive에 저장합니다. 별도의 데이터 업로드가 필요하지 않습니다.

## 📊 데이터 설명

본 프로젝트에서 사용하는 데이터는 [MIMIC-IV Clinical Database Demo v2.2](https://physionet.org/content/mimic-iv-demo/2.2/hosp/#files-panel)에서 가져온 것입니다.

MIMIC-IV는 Beth Israel Deaconess Medical Center의 중환자실(ICU)에 입원한 환자들의 비식별화된 건강 관련 데이터를 포함하는 대규모 공개 데이터베이스입니다. 
Demo 버전은 전체 데이터베이스의 구조와 내용을 검토할 수 있도록 100명의 환자 데이터로 구성된 오픈 소스 데이터셋입니다.

### 데이터 파일 설명

| 파일명 | 설명 | 주요 컬럼 |
|--------|------|----------|
| `patients.csv` | 환자 기본 정보 (인구통계학적 데이터) | `subject_id`, `gender`, `anchor_age`, `dod` |
| `patient_admissions.csv` | 입원 기록 정보 | `patient_id`, `admission_id`, `admission_timestamp`, `urgency_level`, `primary_diagnosis_code` |
| `patient_discharges.csv` | 퇴원 정보 | `patient_id`, `admission_id`, `admission_timestamp`, `discharge_timestamp`, `discharge_status` |
| `patient_transfers.csv` | 환자 전원 기록 (병동 간 이동) | `patient_id`, `admission_id`, `department`, `transfer_in_timestamp`, `transfer_out_timestamp` |
| `d_icd_diagnoses.csv` | ICD-9 진단 코드 사전 | `icd9_code`, `icd_version`, `long_title` |

### 인용 방법

본 데이터를 사용할 경우 다음 논문을 인용해주세요:

```
Johnson, A.E.W., Bulgarelli, L., Shen, L. et al. MIMIC-IV, a freely accessible electronic health record dataset.
Sci Data 10, 1 (2023). https://doi.org/10.1038/s41597-022-01899-x
```

## 📚 참고 자료

- [MIMIC-IV 공식 웹사이트](https://mimic.mit.edu)
- [PhysioNet MIMIC-IV Demo 페이지](https://physionet.org/content/mimic-iv-demo/2.2/hosp/#files-panel)
- [MIMIC-IV 논문](https://www.nature.com/articles/s41597-022-01899-x)

## ⚠️ 주의사항

- 본 데이터는 비식별화되었지만 실제 환자 데이터를 기반으로 하므로, 데이터 사용 시 관련 규정 및 윤리 가이드라인을 준수해야 합니다.
- Demo 버전은 전체 데이터베이스의 일부 샘플이며, 전체 MIMIC-IV 데이터 사용 시 결과와 다를 수 있다.
- 전체 MIMIC-IV 데이터 접근을 위해서는 PhysioNet에서 자격 인증이 필요합니다.
