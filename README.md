CODE:KENTUCKY CAPSTONE PROJECT

# INTRO
Korean Medical Records/History from 2013 & 2023
The primary goal of the project is to look for differences between 2013 and 2023 in relation to utlization of mental health services.

# Project Setup Instructions
 - Clone the repository
 - Navigate to the cloned directory
 - Set up a virtual environment and activate it
 - To ensure you have all the necessary packages, run
     'pip install -r requirements.txt'
 - Run "Capstone.ipynb"

# Data Dictionary

## MEDICAL RECORDS (MAIN DATSET FROM 2013 & 2023)
| Original Columns     | Description/Translation             | Renamed Columns                     | MedicalRecords_2013 | MedicalRecords_2023 | Notes                                          |
| :------------------- | :---------------------------------- | :---------------------------------- | :------------------ | :------------------ | :--------------------------------------------- |
| 기준년도             | Reference Year                      | Reference_Year                      | X                   | X                   |                                                |
| 가입자일련번호       | Subscriber Serial Number            | Subscriber_ID                       | X                   | X                   |                                                |
| 진료내역일련번호     | Claim Serial Number                 | Claim_ID                            | X                   | X                   |                                                |
| 성별코드             | Sex Code                            | Sex                                 | X                   | X                   |                                                |
| 연령대코드           | Age Group Code                      | Age                                 | X                   | X                   |                                                |
| 시도코드             | City Code                           | City_Area                           | X                   | X                   |                                                |
| 요양개시일자         | Date of Medical Care                | date_of_care                        | X                   | X                   |                                                |
| 서식코드             | Form Code                           | form                                | X                   | X                   | Dropped                                        |
| 진료과목코드         | Medical Department Code             | medical_dept                        | X                   | X                   |                                                |
| 주상병코드           | Primary Diagnosis Code              | primary_Diagnosis                   | X                   | X                   |                                                |
| 부상병코드           | Secondary Diagnosis Code            | secondary_diagnosis                 | X                   | X                   |                                                |
| 요양일수             | Number of Medical Care Days         | Total_Care_Days                     | X                   | X                   |                                                |
| 입내원일수           | Number of inpatient care days       | Inpatient_care_days                 | X                   | X                   |                                                |
| 심결가산율           | adjudicated adjustment rate         | adjudicated_adjustment_rate         | X                   | X                   |                                                |
| 심결요양급여비용총액 | adjudicated total medical care cost | adjudicated_total_medical_care_cost | X                   | X                   |                                                |
| 심결본인부담금       | adjudicated patient payment amount  | adjudicated_patient_payment_amount  | X                   | X                   |                                                |
| 심결보험자부담금     | adjusted insurer payment            | adjudicated_insurer_payment         | X                   | X                   |                                                |
| 총처방일수           | Total prescription days             | total_prescription_days             | X                   | X                   |                                                |
| 데이터 기준일자      |                                     |                                     | X                   | N/A                 | Deleted from 2013 dataset during data cleaning |
## GENDER CODING

| CODE  | SEX |
|:-----|:----- |
| 1 | MALE |
| 2 | FEMALE |

## AGE GROUPING
| Age group | Age     |
| :-------- | :------ |
| 1         | 0 - 4   |
| 2         | 5 - 9   |
| 3         | 10 - 14 |
| 4         | 15 - 19 |
| 5         | 20 - 24 |
| 6         | 25 - 29 |
| 7         | 30 - 34 |
| 8         | 35 - 39 |
| 9         | 40 - 44 |
| 10        | 45 - 49 |
| 11        | 50 - 54 |
| 12        | 55 - 59 |
| 13        | 60 - 64 |
| 14        | 65 - 69 |
| 15        | 70 - 74 |
| 16        | 75 - 79 |
| 17        | 80 - 84 |
| 18        | 85 +    |

## AREA/CITY GROUPING
| Area Codes | Area_KR | Area_EN   |
| :--------- | :------ | :-------- |
| 11         | 서울    | Seoul     |
| 26         | 부산    | Busan     |
| 28         | 인천    | Incheon   |
| 27         | 대구    | Daegu     |
| 29         | 광주    | Gwangju   |
| 30         | 대전    | Daejeon   |
| 31         | 울산    | Ulsan     |
| 41         | 경기    | Gyeonggi  |
| 42         | 강원    | Gangwon   |
| 43         | 충북    | Chungbuk  |
| 44         | 충남    | Chungnam  |
| 45         | 전북    | Jeonbuk   |
| 46         | 전남    | Jeonnam   |
| 47         | 경북    | Gyeongbuk |
| 48         | 경남    | Gyeongnam |
| 49         | 제주    | Jeju      |
| 41         | 세종    | Sejong    |

## FORM CODES
| Form CODES | Description_KR          | Description_EN           |
| :--------- | :---------------------- | :----------------------- |
| 2          | 의과 입원               | Medical Inpatient        |
| 3          | 의과 외래               | Medical Outpatient       |
| 6          | 조산원 입원             | Midwifery Inpatient      |
| 7          | 보건기관 입원           | Institutional Inpatient  |
| 8          | 보건기관 외래           | Institutional Outpatient |
| 9          | 정신과 낮병동           | Psychiatric Dayward      |
| 10         | 정신과 입원             | Psychiatric Inpatient    |
| 11         | 정신과 외래             | Psychiatric Outpatient   |
| ZZ         | 결측                    | Missing                  |
| -          | 정상 또는 해당사항 없음 | Not Applicable           |

## MEDICAL DEPARTMENT CODES
| Med_Dept_Code | Med_Dept_Code_KR        | Med_Dept_Code_EN                          |
| :------------ | :---------------------- | :---------------------------------------- |
| 0             | 일반의                  | General medicine                          |
| 1             | 내과                    | Internal medicine                         |
| 2             | 신경과                  | Neurology                                 |
| 3             | 정신건강의학과          | Psychiatry                                |
| 4             | 외과                    | Surgery                                   |
| 5             | 정형외과                | Orthopedics                               |
| 6             | 신경외과                | Neurosurgery                              |
| 7             | 흉부외과                | Thoracic Surgery                          |
| 8             | 성형외과                | Plastic surgery                           |
| 9             | 마취통증의학과          | Anesthesiology and pain medicine          |
| 10            | 산부인과                | Obstetrics and gynecology                 |
| 11            | 소아청소년과            | Pediatrics                                |
| 12            | 안과                    | Ophthalmology                             |
| 13            | 이비인후과              | ENT                                       |
| 14            | 피부과                  | Dermatology                               |
| 15            | 비뇨의학과              | Urology                                   |
| 16            | 영상의학과              | Radiology                                 |
| 17            | 방사선종양학과          | Radiation oncology                        |
| 18            | 병리과                  | Pathology                                 |
| 19            | 진단검사의학과          | Laboratory medicine                       |
| 20            | 결핵과                  | Tuberculosis                              |
| 21            | 재활의학과              | Rehabilitation Medicine                   |
| 22            | 핵의학과                | Nuclear Medicine                          |
| 23            | 가정의학과              | Family Medicine                           |
| 24            | 응급의학과              | Emergency Medicine                        |
| 25            | 산업의학과              | Occupational and Environmental Medicine   |
| 26            | 예방의학과              | Preventive Medicine                       |
| 50            | 구강악안면외과          | Oral and Maxillofacial Surgery            |
| 51            | 치과보철과              | Prosthodontics                            |
| 52            | 치과교정과              | Orthodontics                              |
| 53            | 소아치과                | Pediatric Dentistry                       |
| 54            | 치주과                  | Periodontics                              |
| 55            | 치과보존과              | Conservative Dentistry                    |
| 56            | 구강내과                | Oral Medicine                             |
| 57            | 영상치의학과            | Radiology                                 |
| 58            | 구강병리과              | Oral Pathology                            |
| 59            | 예방치과                | Preventive Dentistry                      |
| 80            | 한방내과                | Oriental Medicine Internal Medicine       |
| 81            | 한방부인과              | Oriental Medicine Gynecology              |
| 82            | 한방소아과              | Oriental Medicine Pediatrics              |
| 83            | 한방안·이비인후·피부과  | Oriental Medicine Ophthalmology & ENT     |
| 84            | 한방신경정신과          | Oriental Medicine Neuropsychiatry         |
| 85            | 침구과                  | Acupuncture and Moxibustion               |
| 86            | 한방재활의학과          | Oriental Medicine Rehabilitation Medicine |
| 87            | 사상체질과              | Constitutional Medicine                   |
| 88            | 한방응급                | Oriental Medicine Emergency               |
| ZZ            | 결측                    | Missing                                   |
| -             | 정상 또는 해당사항 없음 | Not Applicable                            |
# Data Summary

# Data Source





