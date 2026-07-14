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
