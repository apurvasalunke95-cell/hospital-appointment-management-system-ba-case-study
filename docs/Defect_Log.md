# Defect Log

## Project: Hospital Appointment Management System

Prepared By: Apurva Tukaram Salunke

Version: 1.0

---

# Purpose

The Defect Log is used to record, track, prioritize, and monitor software defects identified during testing. It helps ensure issues are resolved before the system is released.

---

# Defect Summary

| Defect ID | Module | Defect Description | Severity | Priority | Status | Assigned To |
|------------|--------|--------------------|----------|----------|--------|-------------|
| BUG-001 | Patient Registration | Email validation accepts invalid format | Medium | High | Closed | Developer |
| BUG-002 | Login | Incorrect error message for invalid password | Low | Medium | Closed | Developer |
| BUG-003 | Appointment Booking | Double booking allowed for same time slot | Critical | High | Closed | Developer |
| BUG-004 | Doctor Dashboard | Appointment list not sorted by time | Medium | Medium | In Progress | Developer |
| BUG-005 | Reports | Monthly report missing cancelled appointments | High | High | Open | Developer |

---

# Defect Lifecycle

New → Assigned → In Progress → Fixed → Retest → Closed

---

# Severity Levels

| Severity | Description |
|----------|-------------|
| Critical | System cannot function correctly |
| High | Major functionality is affected |
| Medium | Functionality works but with issues |
| Low | Minor issue with little business impact |

---

# Priority Levels

| Priority | Description |
|----------|-------------|
| High | Fix immediately |
| Medium | Fix in the current sprint |
| Low | Fix in a future release |

---

# Example Defect Report

**Defect ID:** BUG-003

**Module:** Appointment Booking

**Title:** Double booking allowed for the same doctor and time slot

**Steps to Reproduce:**
1. Log in as a patient.
2. Book an appointment with Dr. Smith at 10:00 AM.
3. Log in as another patient.
4. Book the same doctor and time slot.

**Expected Result:**
The system should prevent the second booking and display a message indicating the slot is unavailable.

**Actual Result:**
The system allows both appointments to be booked.

**Severity:** Critical

**Priority:** High

**Status:** Closed
