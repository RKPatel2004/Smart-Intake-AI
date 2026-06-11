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
