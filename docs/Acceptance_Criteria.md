# Acceptance Criteria

## Project: Hospital Appointment Management System

Prepared By: Apurva Tukaram Salunke

---

# AC-001: Patient Registration

**Related User Story:** US-001

### Given
The patient is on the registration page.

### When
The patient enters all mandatory details correctly and clicks **Register**.

### Then
- A new patient account is created.
- A success message is displayed.
- The patient is redirected to the login page.

---

# AC-002: Patient Login

**Related User Story:** US-002

### Given
The patient has a registered account.

### When
The patient enters a valid email and password.

### Then
- The patient is logged in successfully.
- The dashboard is displayed.

---

# AC-003: Search Doctor

**Related User Story:** US-003

### Given
The patient is logged in.

### When
The patient searches using a specialty or doctor's name.

### Then
- A list of matching doctors is displayed.
- Available appointment slots are shown.

---

# AC-004: Book Appointment

**Related User Story:** US-004

### Given
The patient has selected a doctor and an available time slot.

### When
The patient clicks **Confirm Appointment**.

### Then
- The appointment is created.
- The selected time slot becomes unavailable.
- A confirmation message is displayed.
- A confirmation email/SMS is sent.

---

# AC-005: Cancel Appointment

**Related User Story:** US-005

### Given
The patient has an upcoming appointment.

### When
The patient clicks **Cancel Appointment**.

### Then
- The appointment status changes to **Cancelled**.
- The time slot becomes available again.
- The patient receives a cancellation confirmation.

---

# AC-006: Reschedule Appointment

**Related User Story:** US-006

### Given
The patient has an existing appointment.

### When
The patient selects a new available date and time.

### Then
- The previous appointment is updated.
- The new appointment details are saved.
- The patient receives a confirmation message.

---

# AC-007: Doctor Updates Availability

**Related User Story:** US-008

### Given
The doctor is logged in.

### When
The doctor updates available dates or time slots.

### Then
- The updated schedule is saved.
- Patients can only book available slots.

---

# AC-008: Administrator Views Reports

**Related User Story:** US-010

### Given
The administrator is logged in.

### When
The administrator opens the Reports page.

### Then
- Appointment statistics are displayed.
- Patient statistics are displayed.
- Reports can be exported.
