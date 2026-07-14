# SQL Queries

## Project: Hospital Appointment Management System

These sample SQL queries demonstrate how data can be retrieved to support business operations and reporting.

---

# 1. View All Patients

```sql
SELECT *
FROM Patient;
```

---

# 2. View All Doctors

```sql
SELECT *
FROM Doctor;
```

---

# 3. Find Available Doctors by Department

```sql
SELECT DoctorID,
       FirstName,
       LastName,
       Department,
       Specialty
FROM Doctor
WHERE Department = 'Cardiology';
```

---

# 4. View Today's Appointments

```sql
SELECT AppointmentID,
       PatientID,
       DoctorID,
       AppointmentDate,
       AppointmentTime,
       Status
FROM Appointment
WHERE AppointmentDate = CURRENT_DATE;
```

---

# 5. Count Total Appointments

```sql
SELECT COUNT(*) AS TotalAppointments
FROM Appointment;
```

---

# 6. Count Cancelled Appointments

```sql
SELECT COUNT(*) AS CancelledAppointments
FROM Appointment
WHERE Status = 'Cancelled';
```

---

# 7. Patient Appointment History

```sql
SELECT AppointmentDate,
       AppointmentTime,
       Status
FROM Appointment
WHERE PatientID = 101
ORDER BY AppointmentDate DESC;
```

---

# 8. Doctor's Daily Schedule

```sql
SELECT AppointmentTime,
       PatientID,
       Status
FROM Appointment
WHERE DoctorID = 5
AND AppointmentDate = CURRENT_DATE
ORDER BY AppointmentTime;
```

---

# 9. Upcoming Appointments

```sql
SELECT *
FROM Appointment
WHERE AppointmentDate >= CURRENT_DATE
ORDER BY AppointmentDate,
         AppointmentTime;
```

---

# 10. Top 5 Doctors by Number of Appointments

```sql
SELECT DoctorID,
       COUNT(*) AS TotalAppointments
FROM Appointment
GROUP BY DoctorID
ORDER BY TotalAppointments DESC
LIMIT 5;
```

---

## Business Value

These queries help hospital management to:

- Monitor appointment trends
- Track doctor utilization
- Measure cancellation rates
- Review patient appointment history
- Support operational decision-making
