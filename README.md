# Heart Attack Risk Database

This project involves the segmentation of a dataset into multiple tables, which are then imported into an SQL database, with primary and foreign keys set up for relational integrity. The dataset was sourced from Kaggle and is structured to facilitate efficient data analysis.

## Table Structure

### 1. HealthMetrics
- **Columns:**
  - `PatientID` (VARCHAR, Primary Key, Foreign Key)
  - `Cholesterol` (INT)
  - `BloodPressure` (VARCHAR)
  - `HeartRate` (INT)
  - `Triglycerides` (INT)
  - `BMI` (DOUBLE)

### 2. Lifestyle
- **Columns:**
  - `PatientID` (VARCHAR, Primary Key, Foreign Key)
  - `Smoking` (BOOLEAN)
  - `Obesity` (BOOLEAN)
  - `AlcoholConsumption` (BOOLEAN)
  - `Diet` (VARCHAR)
  - `PhysicalActivityDaysPerWeek` (INT)
  - `SleepHoursPerDay` (DOUBLE)
  - `SedentaryHoursPerDay` (DOUBLE)
  - `ExerciseHoursPerWeek` (DOUBLE)

### 3. MedicalHistory
- **Columns:**
  - `PatientID` (VARCHAR, Primary Key, Foreign Key)
  - `Diabetes` (BOOLEAN)
  - `PreviousHeartProblems` (BOOLEAN)
  - `MedicationUse` (BOOLEAN)
  - `StressLevel` (INT)

### 4. Patients
- **Columns:**
  - `PatientID` (VARCHAR, Primary Key)
  - `Age` (INT)
  - `Sex` (VARCHAR)
  - `FamilyHistory` (BOOLEAN)
  - `Country` (VARCHAR)
  - `Continent` (VARCHAR)
  - `Hemisphere` (VARCHAR)

### 5. RiskAssessment
- **Columns:**
  - `PatientID` (VARCHAR, Primary Key, Foreign Key)
  - `HeartAttackRisk` (BOOLEAN)

### 6. SocioeconomicStatus
- **Columns:**
  - `PatientID` (VARCHAR, Primary Key, Foreign Key)
  - `Income` (INT)

## Relationships

- **Primary Keys:**
  - Each table has a `PatientID` as the primary key, ensuring that each record is uniquely identifiable.

- **Foreign Keys:**
  - The `PatientID` in `HealthMetrics`, `Lifestyle`, `MedicalHistory`, `RiskAssessment`, and `SocioeconomicStatus` tables serves as a foreign key that references the `PatientID` in the `Patients` table. This enforces referential integrity across the database.

## Dataset Source

The dataset used in this project was sourced from Kaggle. It was split into several tables to normalize the data structure, improve query performance, and make the data easier to manage.

- [Heart Attack Risk Dataset on Kaggle](https://www.kaggle.com/datasets/muhammadehsan000/heart-attack-risk-dataset)

## Database Modifications

- The data types were adjusted to match the intended use case (e.g., converting certain integer columns to BOOLEAN where applicable).
- Primary keys and foreign keys were established to maintain data integrity and relationships between tables.

## How to Use

1. Import the SQL files into your database management system.
2. The database is ready for use with any SQL-based queries for analysis, reporting, or application development.

----------------------------
![1](/HeartAttackRisk/1.png)
![2](/HeartAttackRisk/2.png)
![3](/HeartAttackRisk/3.png)
![4](/HeartAttackRisk/4.png)
![5](/HeartAttackRisk/5.png)
![6](/HeartAttackRisk/6.png)
![7](/HeartAttackRisk/7.png)
![8](/HeartAttackRisk/8.png)
![9](/HeartAttackRisk/9.png)
![10](/HeartAttackRisk/10.png)
![11](/HeartAttackRisk/11.png)
![12](/HeartAttackRisk/12.png)
![13](/HeartAttackRisk/13.png)
![14](/HeartAttackRisk/14.png)
![15](/HeartAttackRisk/15.png)
![16](/HeartAttackRisk/16.png)
![17](/HeartAttackRisk/17.png)
![18](/HeartAttackRisk/18.png)