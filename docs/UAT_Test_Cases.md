# User Acceptance Testing (UAT)

## Project: Hospital Appointment Management System

Prepared By: Apurva Tukaram Salunke

Version: 1.0

---

# Purpose

The purpose of User Acceptance Testing (UAT) is to verify that the Hospital Appointment Management System meets business requirements and is ready for deployment.

---

# Test Cases

| Test Case ID | Test Scenario | Test Steps | Expected Result | Status |
|---------------|---------------|------------|-----------------|--------|
| UAT-001 | Patient Registration | Enter valid patient details and click Register | Patient account is created successfully | Pass |
| UAT-002 | Patient Login | Enter valid email and password | Patient dashboard is displayed | Pass |
| UAT-003 | Search Doctor | Search by specialty | Matching doctors are displayed | Pass |
| UAT-004 | Book Appointment | Select doctor, date, and time, then confirm | Appointment is booked successfully | Pass |
| UAT-005 | Cancel Appointment | Cancel an existing appointment | Appointment status changes to Cancelled | Pass |
| UAT-006 | Reschedule Appointment | Select a new date and time | Appointment is updated successfully | Pass |
| UAT-007 | Doctor Login | Log in with valid credentials | Doctor dashboard is displayed | Pass |
| UAT-008 | Update Doctor Availability | Change available time slots | Updated schedule is saved | Pass |
| UAT-009 | View Daily Schedule | Open Today's Appointments | Daily appointment list is displayed | Pass |
| UAT-010 | Generate Reports | Open Reports page | Reports are generated successfully | Pass |

---

# UAT Entry Criteria

- Functional testing completed successfully.
- Critical defects resolved.
- Test environment is available.
- Business stakeholders are available for testing.

---

# UAT Exit Criteria

- All critical test cases have passed.
- No high-severity defects remain open.
- Business stakeholders approve the system.
- Project Sponsor signs off on deployment.

---

# UAT Sign-off

| Role | Name | Status |
|------|------|--------|
| Business Analyst | Apurva Tukaram Salunke | Approved |
| Project Manager | __________ | Approved |
| Hospital Administrator | __________ | Approved |
