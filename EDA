# HEALTHEDA
Health Data EDA


Step 1:** Understand the Data**
1.1 Get the Number of Records in Each Table
-- Number of patients

SELECT COUNT(*) AS num_patients FROM patients;
Result: 100

-- Number of appointments
SELECT COUNT(*) AS num_appointments FROM appointments;
Result: 200

-- Number of diagnoses
SELECT COUNT(*) AS num_diagnoses FROM diagnoses;
Result: 150

-- Number of prescriptions
SELECT COUNT(*) AS num_prescriptions FROM prescriptions;
Result: 120

Get an Overview of Patients
SELECT * FROM patients LIMIT 10;

 Get an Overview of Appointments
SELECT * FROM appointments LIMIT 10;

2.1 Distribution of Patients by Gender

SELECT gender, COUNT(*) AS num_patients
FROM patients
GROUP BY gender;

gender	num_patients
Male	  51
Female	49

Distribution of Appointments by Status

SELECT status, COUNT(*) AS num_appointments
FROM appointments
GROUP BY status;

status	  num_appointments
Completed	68
Cancelled	67
Scheduled	65

Time Series Analysis
3.1 Number of Appointments Over Time
SELECT appointment_date, COUNT(*) AS num_appointments
FROM appointments
GROUP BY appointment_date
ORDER BY appointment_date;

Diagnoses Over Time
SELECT diagnosis_date, COUNT(*) AS num_diagnoses
FROM diagnoses
GROUP BY diagnosis_date
ORDER BY diagnosis_date;


Most Common Diagnoses

SELECT diagnosis_code, description, COUNT(*) AS num_occurrences
FROM diagnoses
GROUP BY diagnosis_code, description
ORDER BY num_occurrences DESC
LIMIT 10;

diagnosis_code	description	num_occurrences
D005	Hypertension	32
D001	Cold	31
D004	Diabetes	28
D003	Flu	30
D002	Cancer	29

Medications Prescribed by Doctor

SELECT doctor_id, medication, COUNT(*) AS num_prescriptions
FROM prescriptions
GROUP BY doctor_id, medication
ORDER BY num_prescriptions DESC
LIMIT 10;

doctor_id	medication	num_prescriptions
17	MedB	5
9	MedA	4
19	MedE	4
4	MedE	3
7	MedA	3

Join Patients and Appointments

SELECT p.patient_id, p.first_name, p.last_name, a.appointment_date, a.specialty, a.status
FROM patients p
JOIN appointments a ON p.patient_id = a.patient_id
LIMIT 3;

patient_id	first_name	last_name	appointment_date	specialty	status
1	Tom	Doe	2023-01-02	Orthopedics	Completed
4	Tom	Doe	2023-01-04	Pediatrics	Completed
96	Lucy	Smith	2023-01-01	Cardiology	Scheduled

Patients with Most Appointments

SELECT p.patient_id, p.first_name, p.last_name, COUNT(a.appointment_id) AS num_appointments
FROM patients p
JOIN appointments a ON p.patient_id = a.patient_id
GROUP BY p.patient_id, p.first_name, p.last_name
ORDER BY num_appointments DESC
LIMIT 3;

patient_id	first_name	last_name	num_appointments
1	Tom	Doe	4
4	Tom	Doe	4
96	Lucy	Smith	4



