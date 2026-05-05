# SA-project
## Clinic Management System - System Analysis Report

### 1. Introduction
This report presents the analysis and design of a **Clinic Management System**. The system aims to improve clinic operations by integrating patient registration, appointment scheduling, consultation management, and billing into a single platform.

### 2. Problem Statement
Many clinics rely on manual or partially digital systems, leading to scheduling conflicts, long waiting times, and difficulty accessing patient information. A centralized system is needed to improve efficiency and accuracy.

### 3. System Scope
*   **In Scope:** Patient registration, appointment scheduling, consultation recording, and billing.
*   **Out of Scope:** Laboratory systems, pharmacy systems, and inpatient services.

### 4. Stakeholders
*   Clinic Owner (Project Sponsor)
*   Patients
*   Doctors
*   Receptionists
*   IT Support Staff

### 5. Actors
*   **Primary Actors:** Patient, Receptionist, Doctor.
*   **Supporting Actors:** System Administrator, Payment System.

### 6. Requirements Definition
| Category | Requirements |
| :--- | :--- |
| **Functional** | Register patients, schedule/manage appointments, record consultations, process payments, and handle cancellations/refunds. |
| **Non-Functional** | Reliability, security, usability, performance, and availability. |

### 7. Requirements Elicitation Technique
The primary technique used is **Interviews** with clinic staff, supplemented by **Observation** of real-life operations.

### 8. Methodology Selection
The **V-Model** is selected to ensure reliability and quality by matching each development phase with a specific testing phase.

### 9. System Design Overview
The system is divided into three main modules to improve maintainability:
*   Patient Records System
*   Appointment Management System
*   Billing & Payment System

---

### 10. Event-Response Table

| Event | Trigger | Source | Use Case | Response | Destination |
| :--- | :--- | :--- | :--- | :--- | :--- |
| Patient registers | Enter personal data | Patient / Receptionist | Register Patient | Patient record created | Patient Records System |
| Patient books appointment | Select time slot | Patient / Receptionist | Schedule Appointment | Appointment scheduled OR rejected if no slots | Appointment Management System |
| No available slots | No free time slots | Appointment Management System | Notify Unavailability | Inform patient no appointments available | Patient / Receptionist |
| Online payment made | Pay during booking | Patient | Process Online Payment | Payment confirmed | Billing & Payment System |
| Patient arrives | Arrives at clinic | Patient | Check-in Patient | Patient marked as arrived | Appointment Management System |
| Payment required | No prior payment | Appointment Management System | Request Payment | Payment request generated | Receptionist |
| On-site payment made | Pay at reception | Patient | Process Payment | Payment recorded | Billing & Payment System |
| Payment verified | Payment completed | Billing & Payment System | Validate Payment | Consultation access granted | Doctor |
| Doctor starts consultation | Patient ready & paid | Doctor | Start Consultation | Patient record displayed | Patient Records System |
| Doctor records diagnosis | During consultation | Doctor | Record Diagnosis | Medical notes saved | Patient Records System |
| Doctor ends consultation | Consultation finished | Doctor | End Consultation | Visit status updated | Appointment Management System |
| Appointment canceled | Cancel request | Patient / Receptionist | Cancel Appointment | Appointment removed | Appointment Management System |
| Refund requested | Cancel after online payment | System | Process Refund | Refund initiated | Billing & Payment System |
| Refund completed | Refund processed | Billing & Payment System | Confirm Refund | Patient notified of refund | Patient |

---

### 11. Conclusion
The proposed Clinic Management System provides an efficient solution to manage clinic operations, enhancing workflow and reducing errors through automation.
## Tasks
- [x] Event table [Ahmed Sakr]
- [x] Use case diagram [Ahmed Sakr]
- [x] [Use case description for some use cases](Use_Case_Descriptions.md) [Ahmed Sakr]
- [ ] Activity diagram
- [ ] State diagram for some objects
- [ ] DFD
- [ ] Project Management
