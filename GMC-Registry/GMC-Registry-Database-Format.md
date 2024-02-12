|**Column**|**Description**|**Type**|**Maximum number of characters**|**Comments**|
|----------|---------------|--------|--------------------------------|------------|
|GMC Ref No|This is the unique seven digit reference number allocated by the GMC to each registered doctor|VARCHAR2|7||
|Surname|The surname, last name or family name in mixed case|VARCHAR2|50||
|Given name|The given/first names in mixed case|VARCHAR2|50||
|Gender|Man (M) or Woman (W) or Not available (X)|VARCHAR2|1|M’an or ‘W’oman or ‘X’ not available|
|Qualification|This is the name of the doctor’s primary medical qualification|VARCHAR2|30||
|Year of Qualification|The year when primary medical qualification exams were passed|VARCHAR2|4||
|Place of Qualification|The name of the place of study for primary medical qualification|VARCHAR2|100||
|PR Date|This is the date that the doctor was first granted provisional registration|DATE|8|ddmmyyyy format|
|FR Date|This is the date that the doctor was first granted full registration|DATE|8|ddmmyyyy format|
|Specialist Register Date|This is the date that the doctor was entered into the Specialist Register|DATE|8|ddmmyyyy format|
|GP Register Date|This is the date that the doctor was entered into the GP Register|DATE|8|ddmmyyyy format|
|Registration Status1|The current status of a doctor's entry in the medical register, including the doctor’s licence status|VARCHAR2|100||
|ARF Due Date|This is the date that the doctor’s annual retention fee (ARF) is due|DATE|8|ddmmyyyy format|
|Specialty1-7|This is the specialty identified in the specialist register. Up to 7 specialties can be provided for a given doctor|VARCHAR2|100||
|Sub-Specialty1-7|This is the sub-specialty identified in the Specialist Register. Up to 7 sub-specialties can be provided for a given doctor|VARCHAR2|100||
|FtP Conditions Exist|This indicates whether the doctor has active fitness to practise conditions applied to their registration|VARCHAR2|1|‘Y’es or ‘N’o|
|FtP Undertakings Exist|This indicates whether the doctor has active fitness to practise undertakings applied to their registration|VARCHAR2|1|‘Y’es or ‘N’o|
|Other Names|The doctor’s other or “middle” names in mixed case. This field will contain all of the other names that the doctor has registered with the GMC|VARCHAR2|150||
|FtP Warnings Exist|This indicates whether the doctor has an active fitness to practise warning|VARCHAR2|1|‘Y’es or ‘N’o|
|Place of Qualification Country|The name of the country where a doctor did their primary medical qualification|VARCHAR2|100||
|Revalidation Status|The doctor’s current revalidation status|String|100||
|Designated Body|The name of the doctor’s current designated body|String|150||
|Responsible Officer|The name of the doctor’s current responsible officer|String|50||
|Doctor in Training|Indicates if the doctor was known to be on a postgraduate training programme in the most recent national training survey|String|1|‘Y’es or ‘N’o|
|Training Deanery/LETB|The deanery/LETB responsible for the doctor’s training, as declared in the most recent national training survey|String|100||
|Training Programme Speciality|The doctor’s training programme speciality, as declared in the most recent national training survey|String|100||
|GMC Approved Trainer|Indicates if the doctor is an approved trainer|String|1|‘Y’es or ‘N’o|
|Trainer Deanery/LETB 1|The deanery/LETB where the doctor is known to be a trainer|String|100||
|Trainer Programmes Speciality 1|The training programme speciality that the doctor is known to train in|String|100||
|Trainer Deanery/LETB 2|The second deanery/LETB where the doctor is known to be a trainer, where more than one exists|String|100||
|Trainer Programmes Speciality 2|The second training programme specialty that the doctor is known to train in, where more than one exists|String|100||
|Trainer Deanery/LETB 3|The third deanery/LETB where the doctor is known to be a trainer, where three exist|String|100||
|Trainer Programmes Speciality 3|The third training programme specialty that the doctor is known to train in, where three exist|String|100||
|ID Check Not Done|The GMC has been unable to perform an identity check for this doctor due to the COVID pandemic|String|3|'Y'es, 'N/A' or blank|
|Temporary Covid Registration|The doctor holds temporary registration as a result of the COVID pandemic|String|1|'Y'es or blank|

