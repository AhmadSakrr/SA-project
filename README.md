# SA-project
## Clinic Management System - System Analysis Report

### 1. Introduction
This report presents the analysis and design of a **Clinic Management System**[cite: 1]. The system aims to improve clinic operations by integrating patient registration, appointment scheduling, consultation management, and billing into a single platform[cite: 1].

### 2. Problem Statement
Many clinics rely on manual or partially digital systems, leading to scheduling conflicts, long waiting times, and difficulty accessing patient information[cite: 1]. A centralized system is needed to improve efficiency and accuracy[cite: 1].

### 3. System Scope
*   **In Scope:** Patient registration, appointment scheduling, consultation recording, and billing[cite: 1].
*   **Out of Scope:** Laboratory systems, pharmacy systems, and inpatient services[cite: 1].

### 4. Stakeholders
*   Clinic Owner (Project Sponsor)[cite: 1]
*   Patients[cite: 1]
*   Doctors[cite: 1]
*   Receptionists[cite: 1]
*   IT Support Staff[cite: 1]

### 5. Actors
*   **Primary Actors:** Patient, Receptionist, Doctor[cite: 1].
*   **Supporting Actors:** System Administrator, Payment System[cite: 1].

### 6. Requirements Definition
| Category | Requirements |
| :--- | :--- |
| **Functional** | Register patients, schedule/manage appointments, record consultations, process payments, and handle cancellations/refunds[cite: 1]. |
| **Non-Functional** | Reliability, security, usability, performance, and availability[cite: 1]. |

### 7. Requirements Elicitation Technique
The primary technique used is **Interviews** with clinic staff, supplemented by **Observation** of real-life operations[cite: 1].

### 8. Methodology Selection
The **V-Model** is selected to ensure reliability and quality by matching each development phase with a specific testing phase[cite: 1].

### 9. System Design Overview
The system is divided into three main modules to improve maintainability[cite: 1]:
*   Patient Records System[cite: 1]
*   Appointment Management System[cite: 1]
*   Billing & Payment System[cite: 1]

---

### 10. Event-Response Table

| Event | Trigger | Source | Use Case | Response | Destination |
| :--- | :--- | :--- | :--- | :--- | :--- |
| Patient registers | Enter personal data | Patient / Receptionist | Register Patient | Patient record created | Patient Records System[cite: 2] |
| Patient books appointment | Select time slot | Patient / Receptionist | Schedule Appointment | Appointment scheduled OR rejected if no slots | Appointment Management System[cite: 2] |
| No available slots | No free time slots | Appointment Management System | Notify Unavailability | Inform patient no appointments available | Patient / Receptionist[cite: 2] |
| Online payment made | Pay during booking | Patient | Process Online Payment | Payment confirmed | Billing & Payment System[cite: 2] |
| Patient arrives | Arrives at clinic | Patient | Check-in Patient | Patient marked as arrived | Appointment Management System[cite: 2] |
| Payment required | No prior payment | Appointment Management System | Request Payment | Payment request generated | Receptionist[cite: 2] |
| On-site payment made | Pay at reception | Patient | Process Payment | Payment recorded | Billing & Payment System[cite: 2] |
| Payment verified | Payment completed | Billing & Payment System | Validate Payment | Consultation access granted | Doctor[cite: 2] |
| Doctor starts consultation | Patient ready & paid | Doctor | Start Consultation | Patient record displayed | Patient Records System[cite: 2] |
| Doctor records diagnosis | During consultation | Doctor | Record Diagnosis | Medical notes saved | Patient Records System[cite: 2] |
| Doctor ends consultation | Consultation finished | Doctor | End Consultation | Visit status updated | Appointment Management System[cite: 2] |
| Appointment canceled | Cancel request | Patient / Receptionist | Cancel Appointment | Appointment removed | Appointment Management System[cite: 2] |
| Refund requested | Cancel after online payment | System | Process Refund | Refund initiated | Billing & Payment System[cite: 2] |
| Refund completed | Refund processed | Billing & Payment System | Confirm Refund | Patient notified of refund | Patient[cite: 2] |

---

### 11. Conclusion
The proposed Clinic Management System provides an efficient solution to manage clinic operations, enhancing workflow and reducing errors through automation[cite: 2].
## Tasks
- [x] Event table [Ahmed Sakr]
- [x] Use case diagram [Ahmed Sakr]
- [ ] Use case description for some use cases
- [ ] Activity diagram
- [ ] State diagram for some objects
- [ ] DFD
- [ ] Project Management
