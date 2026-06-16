# Niramaya: Healthcare Appointment Booking System with AI integration

## 1. Project Objectives

### 1.1 Primary Objective

The primary objective of developing **Niramaya** is to create a comprehensive, AI-powered healthcare appointment booking system that addresses modern healthcare appointment management challenges by providing intelligent scheduling, queue management, document processing, and patient-doctor interaction capabilities.

---

## 2. Primary Objectives

### 2.1 Dual-Plan Subscription System

Develop a flexible platform offering two distinct subscription plans:

#### 2.1.1 Elite Plan

* QR code-based walk-in queue management.
* Dynamic patient handling for clinic-based practices.
* Real-time queue status and token allocation.
* Ideal for doctors with high walk-in patient volume.

#### 2.1.2 Pro Plan

* Advance slot booking system.
* Structured appointment scheduling.
* Ideal for specialists and consultants.
* Better suited for planned consultation practices.

### 2.2 AI-Powered Conversational Booking

Design and deploy an intelligent chatbot using **LangChain** and **LangGraph** that:

* Guides patients through the booking process using natural conversation.
* Collects symptoms and vital information.
* Collects basic patient details such as:

  * Height
  * Weight
  * Blood Group

### 2.3 Voice AI Appointment Confirmation

Develop a voice-based AI agent using **Vapi** that:

* Makes outbound calls to patients.
* Collects preliminary consultation details such as:

  * Symptoms
  * Reason for visit
  * Height
  * Weight
  * Blood Group
* Provides appointment booking confirmation.

### 2.4 Smart Document Processing

Implement AI-driven medical report processing using **Hugging Face** models to:

* Validate uploaded medical reports.
* Generate concise patient summaries.
* Provide doctors with quick patient briefings.

### 2.5 Secure Payment Infrastructure

Integrate **Stripe Payment Gateway** to provide:

* Secure transaction processing.
* Automated receipt generation.
* Email notifications for successful payments.

### 2.6 Real-Time Queue Management

Develop a dynamic queue management system for Elite Plan doctors that supports:

* Token allocation.
* Waiting time estimation.
* Queue capacity management.

---

## 3. Secondary Objectives

### 3.1 User-Friendly Interface

Design intuitive and responsive interfaces for:

* Patients
* Doctors
* Guest Users

### 3.2 Comprehensive Appointment Management

Enable:

* Appointment booking.
* Appointment status tracking.
* email notifications through smtp nodemailer.

### 3.3 Digital Prescription System

Create a prescription generation module with:

* Medication instructions.
* Dosage schedules.
* Meal timing guidance.

### 3.4 Rating and Review System

Implement a feedback mechanism that allows patients to:

* Rate doctors.
* Submit reviews.

### 3.5 Analytics Dashboard

Provide doctors with insights into:

* Appointment statistics.
* Revenue analytics.
* Availability demographics.

### 3.6 Automated Availability Management

Implement cron-based automation for:

* Generating doctor availability schedules.
* Maintaining schedules up to 30 days in advance.

### 3.7 Data Security

Implement secure mechanisms including:

* Authentication.
* Authorization.
* JWT Token-based security.
* HTTP communication.

---

# 4. System Overview

Niramaya is a comprehensive, AI-powered healthcare appointment booking system that bridges the gap between patients and healthcare providers.

The platform enables:

* Seamless appointment booking for patients.
* Efficient practice management for healthcare providers.
* Modern digital healthcare workflows.

---

## 4.1 Core Concept

The system operates using a dual-plan subscription model that accommodates different doctor practice styles.

### 4.1.1 Elite Plan

* QR code-based walk-in queue management.
* Dynamic patient handling for clinic-based practices.
* Real-time queue status and token allocation.
* Ideal for doctors with high walk-in patient volume.

### 4.1.2 Pro Plan

* Traditional advance slot booking system.
* Structured appointment scheduling.
* Ideal for specialists and consultants.
* Suitable for planned consultation practices.

---

## 4.2 System Users

The platform serves three primary user groups.

### 4.2.1 Patients

Registered users who can:

* Browse doctors.
* Book appointments.
* Manage health records.
* Access prescriptions.

### 4.2.2 Doctors

Healthcare providers who can:

* Subscribe to the platform.
* Manage availability.
* View appointments.
* Create prescriptions.
* Access analytics.

### 4.2.3 Guest Users

Walk-in patients who can:

* Use QR code-based booking.
* Book appointments without registration.

---

# 5. Key Features

## 5.1 Features for Patients

### 5.1.1 Doctor Search

Browse and filter doctors based on:

* Specialty
* City
* Availability
* Consultation Fee

### 5.1.2 AI Chatbot Booking

Conversational appointment booking with intelligent information collection.

### 5.1.3 Voice AI Booking

Outbound voice interaction for collecting:

* Symptoms
* Basic patient details
* Consultation information

before booking confirmation.

### 5.1.4 Medical Report Upload

* Upload up to 5 medical reports per appointment.
* AI-based report validation.

### 5.1.5 AI Summary Generation

Automatic generation of patient briefings from uploaded medical documents.

### 5.1.6 Secure Payments

Stripe-integrated payment gateway with:

* Secure payments.
* Receipt generation.

### 5.1.7 Appointment Management

View and manage appointments with status tracking.

### 5.1.8 Digital Prescriptions

Access prescriptions after completed consultations.

### 5.1.9 Rating System

Rate and review doctors after consultations.

### 5.1.10 Profile Management

Manage:

* Personal information.
* Medical history.
* Emergency contacts.

---

## 5.2 Features for Doctors

### 5.2.1 Subscription Plans

Choose between:

* Elite Plan (QR-based)
* Pro Plan (Slot-based)

### 5.2.2 Profile Management

Manage:

* Specialties
* Qualifications
* Experience
* Consultation Fees

### 5.2.3 Availability Management

Configure:

* Monthly schedules.
* Working durations.
* Break timings.
* Slot durations.

### 5.2.4 Automated Scheduling

Cron-based automatic generation of 30-day availability schedules during Pro doctor signup.

### 5.2.5 QR Code Generation

Generate and display QR codes for walk-in patients under the Elite Plan.

### 5.2.6 Appointment Dashboard

View and manage appointments using filtering options.

### 5.2.7 Patient Summaries

Access AI-generated patient briefings before consultations.

### 5.2.8 Digital Prescriptions

Create detailed prescriptions with medication schedules.

### 5.2.9 Analytics Dashboard

Track:

* Appointments
* Revenue
* Ratings
* Practice performance

### 5.2.10 Dynamic Walk-In Integration

High-velocity queue management system that:

* Prioritizes patient arrivals.
* Automatically sequences walk-in patients.
* Optimizes queue flow.

---

## 5.3 Features for Guest Users

### 5.3.1 QR Code Scanning

Scan doctor QR codes to access booking pages.

### 5.3.2 Queue Status View

View:

* Current waiting count.
* Estimated waiting time.

### 5.3.3 Quick Booking

Book walk-in appointments with minimal information.

### 5.3.4 Payment Processing

Secure payment for walk-in consultations.

### 5.3.5 Token Assignment

Receive queue token numbers via email.

### 5.3.6 Email Confirmation

Receive:

* Booking confirmation.
* Payment receipt.

---

## 5.4 AI-Powered Features

### 5.4.1 Conversational Chatbot

**Technology:** LangChain + LangGraph

**Description:** Multi-turn conversation for appointment booking.

### 5.4.2 Voice AI Agent

**Technology:** Vapi

**Description:** Outbound voice calls for appointment confirmation.

### 5.4.3 Document Validation

**Technology:** Hugging Face

**Description:** AI validation of medical report authenticity.

### 5.4.4 Summary Generation

**Technology:** Hugging Face

**Description:** Automatic patient briefing generation.

### 5.4.5 Information Extraction

**Technology:** LLM (OpenRouter)

**Description:** Extraction of structured patient information from conversations.

---

# 6. Project Screenshots

## 6.1 Landing Page

![Landing Page](images/Landing%20Page.png)

**Description:** Landing page displaying the system introduction with primary navigation options through **Sign In** and **Get Started** buttons for user access and onboarding.

---

## 6.2 Login Page

![Login Page](images/Login%20Page.png)

**Description:** The primary interface for users to sign into their registered accounts.

---

## 6.3 Role Selection Page

![Role Selection Page](images/Role%20Selection%20Page.png)

**Description:** Screen prompting the user to select either the **Patient** or **Doctor** role before registration.

---

## 6.4 Patient Registration Page

![Patient Registration Page](images/Patient%20Registration%20Page.png)

**Description:** The form used for new patients to enter personal and demographic information.

---

## 6.5 Plan Selection Page for Doctors

![Plan Selection Page for Doctors](images/Plan%20selection%20Page%20for%20doctors.png)

**Description:** Doctor's onboarding screen for selecting the Elite (QR-based) or Pro (slot-based) subscription plan.

---

## 6.6 Doctor Registration Page

![Doctor Registration Page](images/Doctor%20Registration%20Page.png)

**Description:** Form for doctors to enter professional credentials, qualifications, and specialties during signup.

---

## 6.7 Doctor Analytics Dashboard

![Doctor Analytics Dashboard](images/Doctor%20Analytics%20Dashboard.png)

**Description:** The doctor's main panel showing key practice metrics, appointments, and overall performance analytics.

---

## 6.8 Appointments Page on Doctor Side

![Appointments Page on Doctor Side](images/Appointments%20Page%20on%20Doctor%20Side.png)

**Description:** Interface for doctors to view and manage all appointments in Ongoing, Scheduled, and History tabs.

---

## 6.9 Doctor Availability Calendar Page

![Doctor Availability Calendar Page](images/Doctor%20Availability%20Calendar%20Page.png)

**Description:** Calendar view for doctors to check and update their consultation schedules and slot availability.

---

## 6.10 Doctor Availability Updation Page

![Doctor Availability Updation Page](images/Doctor%20Availability%20Updation%20Page.png)

**Description:** Form for setting specific working hours, break times, and slot duration for selected dates.

---

## 6.11 Doctor Details

![Doctor Details](images/Doctor%20Details.png)

**Description:** Modal displaying the comprehensive details of a selected doctor, including ratings and experience.

---

## 6.12 Doctor Listing Page on Patient Side

![Doctor Listing Page on Patient Side](images/Doctor%20Listing%20Page%20on%20Patient%20Side.png)

**Description:** Patient interface for searching, filtering, and browsing available doctors by specialty, location, and other filters.

---

## 6.13 Doctor Profile Page

![Doctor Profile Page](images/Doctor%20Profile%20Page.png)

**Description:** Read-only view of the doctor's professional profile, including bio, qualifications, and consultation fee.

---

## 6.14 Edit Medical Report

![Edit Medical Report](images/Edit%20Medical%20Report.png)

**Description:** Interface for a patient to modify, upload, or remove medical reports associated with an upcoming appointment.

---

## 6.15 Landing Page

![Landing Page](images/Landing%20Page.png)

**Description:** Main landing interface of the Niramaya Healthcare Appointment Booking System.

---

## 6.16 Login Page

![Login Page](images/Login%20Page.png)

**Description:** User authentication page for secure access to the platform.

---

## 6.17 Patient Details

![Patient Details](images/Patient%20Details.png)

**Description:** Doctor-side modal view of patient history, including AI-generated summaries of medical reports.

---

## 6.18 Patient Profile

![Patient Profile](images/Patient%20Profile.png)

**Description:** Patient profile management screen showing personal information and medical history.

---

## 6.19 Payment Page

![Payment Page](images/Payment%20Page.png)

**Description:** Secure Stripe-integrated payment interface for consultation fee processing.

---

## 6.20 Payment Receipt

![Payment Receipt](images/Payment%20Receipt.png)

**Description:** Digital receipt summarizing transaction details and payment confirmation.

---

## 6.21 Pending Payment Tab

![Pending Payment Tab](images/Pending%20Payment%20Tab.png)

**Description:** Displays appointments awaiting payment completion.

---

## 6.22 Prescription Issue Page

![Prescription Issue Page](images/Prescription%20Issue%20Page.png)

**Description:** Interface allowing doctors to generate digital prescriptions with medication instructions.

---

## 6.23 Report Upload

![Report Upload](images/Report%20Upload.png)

**Description:** Upload interface for attaching medical reports before appointment confirmation.

---

## 6.24 Scheduled Appointment Tab

![Scheduled Appointment Tab](images/Scheduled%20Appointment%20Tab.png)

**Description:** View of all confirmed upcoming appointments with status tracking.

---

## 6.25 Update Patient Profile Page

![Update Patient Profile Page](images/Update%20Patient%20Profile%20Page.png)

**Description:** Editable profile page for updating patient contact details, vitals, and emergency information.

---

## 6.26 Appointment Booking Through Chatbot

![Appointment Booking Through Chatbot](images/Appointment%20booking%20through%20chatbot.png)

**Description:** AI-powered conversational interface that collects symptoms and patient details for appointment booking.

---

## 6.27 Availability Slots of Selected Doctor

![Availability Slots of Selected Doctor](images/Availability%20slots%20of%20selected%20Doctor.png)

**Description:** Displays available consultation slots for the selected doctor on a chosen date.

---

## 6.28 Chat Bot and Voice Call Selection

![Chat Bot and Voice Call Selection](images/Chat%20Bot%20and%20Voice%20Call%20selection.png)

**Description:** Allows patients to choose between chatbot-assisted booking and voice AI-assisted booking.

---

## 6.29 Booking Confirmation Page

![Booking Confirmation Page](images/Booking%20Confirmation%20page.png)

**Description:** Confirmation screen shown immediately after successful appointment booking and payment.

---

## 6.30 QR Code for ELITE Doctor

![QR Code for ELITE Doctor](images/QR%20code%20for%20ELITE%20doctor.png)

**Description:** QR code generated for an Elite Plan doctor and displayed in the doctor's profile section. Patients can scan this QR code to directly access the doctor's appointment booking page for walk-in consultations.

---

## 6.31 Queue Status and Appointment Form for Guest Patient

![Queue Status and Appointment Form for Guest Patient](images/Queue%20status%20and%20appointment%20form%20for%20Guest%20patient.png)

**Description:** Appointment booking form for guest patients accessed through QR code scanning. The page allows patients to enter their details, view the current queue status, and book a consultation without creating an account.

---

## 6.32 Queue Token Assignment and Queue Status

![Queue Token Assignment and Queue Status](images/Queue%20Token%20Assignment%20and%20Queue%20status.png)

**Description:** Displays the assigned queue token number and real-time queue status for guest patients after successful appointment booking through the QR-based walk-in system.

---

## 6.33 Ongoing Appointment on Doctor Side with Timer

![Ongoing Appointment on Doctor Side with Timer](images/Ongoing%20Appointment%20on%20Doctor%20side%20with%20Timer.png)

**Description:** Doctor-side interface displaying an ongoing patient appointment along with a live consultation timer, helping doctors monitor appointment duration and manage patient flow efficiently.