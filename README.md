**Healthcare Data Exploratory Data Analysis (EDA)**

This repository contains an exploratory data analysis (EDA) of a sample healthcare dataset that I conducted.
The analysis includes the examination of patient demographics, appointment details, diagnoses, and prescription data. 
The purpose of this EDA is to uncover insights and relationships within the healthcare data, providing a foundation for 
further analysis or model building.

**Dataset Description**
The dataset comprises four tables: patients, appointments, diagnoses, and prescriptions. Below is a brief description 
of each table:

**patients:** Contains information about patients, including their ID, name, birth date, gender, city, and state.
appointments: Records details of patient appointments, including appointment ID, patient ID, appointment date, doctor ID, specialty, and status.

**diagnoses:** Includes records of patient diagnoses, with diagnosis ID, patient ID, diagnosis date, diagnosis code, and description.

**Prescriptions:** Contains prescription data, including prescription ID, patient ID, doctor ID, medication, dosage, start date, and end date.

**EDA Steps**
**1. Understanding the Data**
1.1 Get the Number of Records in Each Table:
I determined the count of records in patients, appointments, diagnoses, and prescriptions tables.

1.2 Get an Overview of Patients:
I retrieved a sample of records from the patient's table to understand the structure and contents.

1.3 Get an Overview of Appointments:
I retrieved a sample of records from the appointments table to understand the structure and contents.

**2. Basic Statistics**

2.1 Distribution of Patients by Gender:
I calculated the distribution of patients based on gender.

2.2 Distribution of Appointments by Status:
I calculated the distribution of appointments based on their status (Completed, Cancelled, Scheduled).

**3. Time Series Analysis**

3.1 Number of Appointments Over Time:
I analyzed the number of appointments over time to identify trends.

3.2 Diagnoses Over Time:
I analyzed the number of diagnoses over time to identify trends.

**4. Relationships and Trends**

4.1 Most Common Diagnoses:
I identified the most common diagnoses by counting the occurrences of each diagnosis code and description.

4.2 Medications Prescribed by Doctor:
I determined the most frequently prescribed medications by each doctor.

**5. Join Tables **
5.1 Join Patients and Appointments:
I joined the patients and appointments tables to get detailed information about patient appointments.

5.2 Patients with Most Appointments:
I identified the patients with the highest number of appointments.


**Insights from the Analysis**

**Patient Demographics:**
The gender distribution of patients is nearly balanced, with a slight majority of male patients (51%).
Patients are distributed across various cities and states, with no significant concentration in any specific area.

**Appointment Statistics:**
The appointments are almost evenly distributed among the statuses: Completed, Cancelled, and Scheduled.
There are observable trends in the number of appointments over time, which may indicate seasonal or other time-based patterns.

**Diagnosis Patterns:**
The most common diagnoses are Hypertension, Cold, Flu, Cancer, and Diabetes.
There are noticeable trends in the number of diagnoses over time, which can help in identifying patterns in disease prevalence.

**Prescription Trends:**
Certain medications are prescribed more frequently by specific doctors, indicating specialization or preference in treatment approaches.
There is a correlation between specific diagnoses and the number of prescriptions, highlighting common treatment practices.

**Patient Engagement:**
Some patients have a significantly higher number of appointments, which may indicate chronic conditions or frequent healthcare needs.

**Data Relationships:**
Joining different tables provided deeper insights into patient care, such as the relationship between diagnoses and prescriptions, and the detailed view of patient appointments.


**Conclusion**


This EDA provides a comprehensive overview of a healthcare dataset, helping to uncover key insights and relationships within the data. The analysis can be further extended to include more detailed investigations or to build predictive models based on the discovered patterns.
