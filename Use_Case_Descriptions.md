# Use Case Descriptions

This document provides detailed descriptions for some of the primary use cases in the Clinic Management System, formatted using standard Use Case Description templates.

## 1. Register Patient

| | | |
| :--- | :--- | :--- |
| **Use Case Name:** | Register Patient | |
| **Actors:** | Patient / Receptionist | |
| **Preconditions:** | The patient does not already exist in the Patient Records System. | |
| **Postconditions:** | A new patient record is created and stored in the Patient Records System. | |
| **Flow of Activities:** | **Actor** | **System** |
| | 1. Actor selects the "Register Patient" option.<br>2. Actor enters the required information and submits. | 1.1 System prompts for patient details (Name, DOB, Contact Info, Medical History).<br>2.1 System validates the input data.<br>2.2 System creates a new patient record in the database.<br>2.3 System displays a success message with the new Patient ID. |
| **Exception Conditions:** | 2.1 If invalid data, system highlights errors and asks the actor to re-enter the data.<br>2.1 If patient already exists, system detects duplicate information and offers to retrieve the existing record. | |

## 2. Schedule Appointment

| | | |
| :--- | :--- | :--- |
| **Use Case Name:** | Schedule Appointment | |
| **Actors:** | Patient / Receptionist | |
| **Preconditions:** | The patient must be registered in the system. | |
| **Postconditions:** | An appointment is confirmed and added to the Appointment Management System. | |
| **Flow of Activities:** | **Actor** | **System** |
| | 1. Actor accesses the appointment scheduling interface.<br>2. Actor selects a specific doctor and date.<br>3. Actor selects an available time slot.<br>4. Actor confirms the booking (and optionally pays online). | 1.1 System displays the scheduling interface.<br>2.1 System retrieves and displays available time slots.<br>3.1 System temporarily holds the slot and prompts for confirmation.<br>4.1 System saves the appointment details.<br>4.2 System sends a confirmation notification to the patient. |
| **Exception Conditions:** | 2.1 If no time slots are available, system notifies the actor and prompts to select another date or doctor.<br>3.1 If the actor takes too long to confirm, the held slot is released. | |

## 3. Process Payment

| | | |
| :--- | :--- | :--- |
| **Use Case Name:** | Process Payment | |
| **Actors:** | Patient, Receptionist | |
| **Preconditions:** | An appointment must be scheduled, and payment must be pending. | |
| **Postconditions:** | Payment is recorded, and the appointment status is updated to allow consultation. | |
| **Flow of Activities:** | **Actor** | **System** |
| | 1. Patient requests to pay for the appointment.<br>2. Receptionist collects payment from the patient (cash or card).<br>3. Receptionist records the payment in the Billing & Payment System. | 1.1 System generates a payment request for the appointment.<br><br>3.1 System validates the payment.<br>3.2 System generates a receipt and updates the visit status. |
| **Exception Conditions:** | 1.1 If online payment is chosen during booking, the system securely processes the transaction through a Payment gateway before confirming the appointment.<br>3.1 If the payment is declined or unsuccessful, system alerts the actor and requests an alternative payment method. | |

## 4. Record Diagnosis

| | | |
| :--- | :--- | :--- |
| **Use Case Name:** | Record Diagnosis | |
| **Actors:** | Doctor | |
| **Preconditions:** | The patient has checked in, payment is verified, and the consultation has started. | |
| **Postconditions:** | The patient's medical record is updated with the new diagnosis and notes. | |
| **Flow of Activities:** | **Actor** | **System** |
| | 1. Doctor starts the consultation in the system.<br>2. Doctor examines the patient and enters diagnosis details and medical notes.<br>3. Doctor submits the notes.<br>4. Doctor ends the consultation. | 1.1 System retrieves and displays the patient's medical history.<br><br>3.1 System saves the medical notes to the Patient Records System.<br>4.1 System updates the visit status. |
| **Exception Conditions:** | 3.1 If the system is unable to save the record, it prompts the doctor to save a local draft and retry later. | |
