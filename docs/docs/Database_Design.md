# Database Design

## Purpose

The Hospital Appointment Management System stores information about patients, doctors, appointments, and users. The database is designed to ensure data consistency and support efficient appointment scheduling.

---

# Entity Relationship Overview

The system consists of four main entities:

- Patient
- Doctor
- Appointment
- User

Relationships:

- One Patient can have many Appointments.
- One Doctor can have many Appointments.
- One Appointment belongs to one Patient and one Doctor.

---

# Patient Table

| Column | Data Type | Description |
|---------|-----------|-------------|
| PatientID | INT (PK) | Unique patient ID |
| FirstName | VARCHAR(50) | Patient first name |
| LastName | VARCHAR(50) | Patient last name |
| DOB | DATE | Date of birth |
| Gender | VARCHAR(10) | Gender |
| Phone | VARCHAR(15) | Contact number |
| Email | VARCHAR(100) | Email address |

---

# Doctor Table

| Column | Data Type | Description |
|---------|-----------|-------------|
| DoctorID | INT (PK) | Unique doctor ID |
| FirstName | VARCHAR(50) | First name |
| LastName | VARCHAR(50) | Last name |
| Department | VARCHAR(50) | Department |
| Specialty | VARCHAR(100) | Medical specialty |
| Email | VARCHAR(100) | Email |
| Phone | VARCHAR(15) | Contact number |

---

# Appointment Table

| Column | Data Type | Description |
|---------|-----------|-------------|
| AppointmentID | INT (PK) | Appointment ID |
| PatientID | INT (FK) | Patient reference |
| DoctorID | INT (FK) | Doctor reference |
| AppointmentDate | DATE | Appointment date |
| AppointmentTime | TIME | Appointment time |
| Status | VARCHAR(20) | Booked, Cancelled, Completed |

---

# User Table

| Column | Data Type | Description |
|---------|-----------|-------------|
| UserID | INT (PK) | User ID |
| Username | VARCHAR(50) | Login username |
| Password | VARCHAR(255) | Encrypted password |
| Role | VARCHAR(20) | Patient, Doctor, Receptionist, Admin |
