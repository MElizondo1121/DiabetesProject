# Collaborative Research: SCH: Improving Diagnostic Efficiency and Patient Care

November 11, 2023
Diabetes can be classified into four categories (Diabetes - Type 1, Type 2, Mellitus, Mellitus with Complications)

# Diabetic Patients' Re-Admission (Kaggle)
## Attribute Descriptions :
| Feature name               | Type    | Description                                                                                                   | % missing |
|----------------------------|---------|---------------------------------------------------------------------------------------------------------------|-----------|
| Encounter ID               | Numeric | Unique identifier of an encounter                                                                              | 0%        |
| Patient number             | Numeric | Unique identifier of a patient                                                                                 | 0%        |
| Race                       | Nominal | Values: Caucasian, Asian, African American, Hispanic, and other                                              | 2%        |
| Gender                     | Nominal | Values: male, female, and unknown/invalid                                                                     | 0%        |
| Age                        | Nominal | Grouped in 10-year intervals: [0, 10), [10, 20), ..., [90, 100)                                                | 0%        |
| Weight                     | Numeric | Weight in pounds.                                                                                              | 97%       |
| Admission type             | Nominal | Integer identifier corresponding to 9 distinct values, e.g., emergency, urgent, elective, newborn, and not available | 0%        |
| Discharge disposition      | Nominal | Integer identifier corresponding to 29 distinct values, e.g., discharged to home, expired, and not available    | 0%        |
| Admission source           | Nominal | Integer identifier corresponding to 21 distinct values, e.g., physician referral, emergency room, and transfer from a hospital | 0%        |
| Time in hospital           | Numeric | Number of days between admission and discharge                                                                 | 0%        |
| Payer code                 | Numeric | Identifier corresponding to 23 distinct values, e.g., Blue Cross Blue Shield, Medicare, and self-pay           | 52%       |
| Medical specialty          | Nominal | Identifier of a specialty of the admitting physician, corresponding to 84 distinct values, e.g., cardiology, internal medicine, family/general practice, and surgeon | 53%       |
| Number of lab procedures   | Numeric | Number of lab tests performed during the encounter                                                              | 0%        |
| Number of procedures       | Numeric | Number of procedures (other than lab tests) performed during the encounter                                     | 0%        |
| Number of medications      | Numeric | Number of distinct generic names administered during the encounter                                             | 0%        |
| Number of outpatient visits| Numeric | Number of outpatient visits of the patient in the year preceding the encounter                                  | 0%        |
| Number of emergency visits | Numeric | Number of emergency visits of the patient in the year preceding the encounter                                  | 0%        |
| Number of inpatient visits | Numeric | Number of inpatient visits of the patient in the year preceding the encounter                                  | 0%        |
| Diagnosis 1                | Numeric | The primary diagnosis (coded as first three digits of ICD9); 848 distinct values                               | 0%        |
| Diagnosis 2                | Numeric | Secondary diagnosis (coded as first three digits of ICD9); 923 distinct values                                 | 0%        |
| Diagnosis 3                | Numeric | Additional secondary diagnosis (coded as first three digits of ICD9); 954 distinct values                        | 1%        |
| Number of diagnoses        | Numeric | Number of diagnoses entered to the system                                                                     | 0%        |
| Glucose serum test result  | Nominal | Indicates the range of the result or if the test was not taken. Values: ">200," ">300," "normal," and "none" if not measured | 0%        |
| A1Cresult                  | Nominal | Indicates the range of the result or if the test was not taken. Values: ">8," ">7," "normal," and "none" if not measured | 0%        |
| 24 features for medications| Nominal | Indicates if there was a change in diabetic medications. Values: "change" and "no change"                        | 0%        |
| Change of medications      | Nominal | Indicates if there was any diabetic medication prescribed. Values: "yes" and "no"                              | 0%        |
| Diabetes medications       | Nominal | Indicates whether specific drugs were prescribed or had dosage changes. Values: "up," "down," "steady," and "no" | 0%        |
| Readmitted                 | Nominal | Days to inpatient readmission. Values: "<30," ">30," and "No" for no record of readmission                    | 0%        |
