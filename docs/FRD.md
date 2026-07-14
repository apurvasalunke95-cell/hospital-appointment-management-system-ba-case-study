# Functional Requirements Document (FRD)

## Project Information

| Item | Details |
|------|---------|
| Project Name | Hospital Appointment Management System |
| Prepared By | Apurva Tukaram Salunke |
| Role | Business Analyst |
| Version | 1.0 |
| Date | July 2026 |

---

# 1. Purpose

This document defines the functional and non-functional requirements for the Hospital Appointment Management System. It serves as a reference for developers, testers, and stakeholders during design, development, and testing.

---

# 2. System Users

- Patient
- Doctor
- Receptionist
- Hospital Administrator

---

# 3. Functional Requirements

## FR-01: Patient Registration

**Description:**  
The system shall allow new patients to register by providing personal details.

**Input:**
- Full Name
- Date of Birth
- Gender
- Phone Number
- Email Address
- Password

**Output:**
- Patient account created successfully.

---

## FR-02: Patient Login

**Description:**  
The system shall allow registered patients to log in securely using their email and password.

---

## FR-03: Search Doctor

The patient shall be able to search doctors by:
- Department
- Specialty
- Doctor Name
- Available Date

---

## FR-04: Book Appointment

The patient shall be able to:
- Select a doctor
- Select an available date
- Select an available time slot
- Confirm the appointment

The system shall prevent double bookings.

---

## FR-05: Cancel Appointment

Patients shall be able to cancel appointments before the scheduled time.

---

## FR-06: Reschedule Appointment

Patients shall be able to select a new available date and time.
---

# 4. Doctor Module

## FR-07: Doctor Login

The system shall allow doctors to log in securely using their registered email address and password.

---

## FR-08: View Appointment Schedule

The doctor shall be able to:

- View today's appointments
- View upcoming appointments
- View patient details
- Filter appointments by date

---

## FR-09: Manage Availability

The doctor shall be able to:

- Add available dates
- Remove unavailable dates
- Block vacation days
- Update working hours

---

# 5. Receptionist Module

## FR-10: Manage Patients

The receptionist shall be able to:

- Register new patients
- Update patient details
- Search patient records

---

## FR-11: Manage Appointments

The receptionist shall be able to:

- Book appointments
- Cancel appointments
- Reschedule appointments
- Check doctor availability

---

# 6. Administrator Module

## FR-12: User Management

The administrator shall be able to:

- Create users
- Edit users
- Delete users
- Reset passwords

---

## FR-13: Reports

The administrator shall be able to generate reports such as:

- Daily appointments
- Monthly appointments
- Doctor utilization
- Appointment cancellations
- Patient registration statistics

---

## FR-14: Dashboard

The administrator dashboard shall display:

- Total appointments
- Today's appointments
- Active doctors
- Registered patients
- Cancelled appointments
- ---

# 7. Non-Functional Requirements

| ID | Requirement |
|----|-------------|
| NFR-01 | System availability shall be 99.9%. |
| NFR-02 | Login response time shall be less than 2 seconds. |
| NFR-03 | Appointment booking shall complete within 5 seconds. |
| NFR-04 | User passwords shall be encrypted. |
| NFR-05 | Only authorized users can access the system. |
| NFR-06 | System shall support Chrome, Edge, Safari and Firefox. |
| NFR-07 | Daily database backup shall be performed. |
| NFR-08 | The application shall support at least 500 concurrent users. |

---

# 8. Business Rules

- A patient cannot book two appointments at the same time.
- Doctors cannot be booked during unavailable hours.
- Cancelled appointment slots become available immediately.
- Every appointment must have one patient and one doctor.
- Only administrators can delete user accounts.
- Appointment reminders shall be sent 24 hours before the appointment.

---

# 9. Assumptions

- Internet connectivity is available.
- Users possess valid login credentials.
- Doctors update their availability regularly.

---

# 10. Dependencies

- Patient database
- Doctor database
- Email/SMS notification service
- Authentication service
