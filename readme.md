# 🎓 College Event Management System – ServiceNow
<img width="1920" height="1080" alt="image" src="https://github.com/user-attachments/assets/2afe8902-3745-475b-8ee5-c2946cd0b8cf" />
<img width="1920" height="1080" alt="image" src="https://github.com/user-attachments/assets/e68558cd-7372-4869-935b-a649651bbdb5" />

## 📌 Project Overview
The **College Event Management System** is a custom application built on the **ServiceNow App Engine** platform.  
It helps colleges manage event requests, approvals, and tracking in a structured and automated way across **web and mobile interfaces**.

This project demonstrates my hands-on understanding of **ServiceNow fundamentals**, **application development**, **UI customization**, **mobile experience configuration**, and **automation using Business Rules and Flows**.

---

## 🎯 Objectives
- Allow students or staff to raise **college event requests**
- Capture important event details in a single form
- Automatically handle **event approval status**
- Provide a **user-friendly web and mobile experience**
- Improve transparency and reduce manual follow-ups

---

## 🛠️ Technologies & Platform
- **Platform:** ServiceNow (App Engine Studio)
- **Language:** JavaScript (Business Rules)
- **Tools Used:**
  - Tables & Fields
  - UI Policies
  - Business Rules
  - Flow Designer (basic)
  - Forms & Lists
  - Application Scope
  - Mobile Record Experience

---

## 🗂️ Application Details

### 🔹 Application Name
**College Event Management System**

### 🔹 Application Scope
`x_event_mgmt_student`

---

## 📊 Data Model

### 📁 Table: College Event
Custom table created to store event request details.

**Key Fields:**
- Event Name (String)
- Event Type (Choice)
- Event Date (Date)
- Requested By (Reference → User)
- Budget (Currency)
- Status (Choice: Requested, Approved, Rejected)
- Description (String)

---

## 🖥️ User Interface Features (Web)

### 🔹 Custom Form
- Clean and simple event request form
- User-friendly layout for fresh users

### 🔹 UI Policy (No Script)
**Goal:** Hide Budget field until Event Type is selected  
- Improves form clarity
- Reduces user confusion

---

## 📱 Mobile Experience

### 🔹 Mobile User Interface
- Created a **mobile-friendly interface** using **ServiceNow App Engine Studio**
- Configured a **record-based mobile experience** for the College Event table
- Enabled users to **create, view, and track event requests** using the **ServiceNow Mobile App**
- Optimized mobile layout for **easy navigation and minimal input**
- Ensured **role-based access** for secure mobile interaction

This mobile experience improves accessibility and allows users to manage event requests on the go.

---

## 🔄 Automation Logic

### 🔹 Approval Logic (Simple Flow)
- Event record is created
- Event status initially set to **Requested**
- Approval request is generated for admin/manager
- Based on approval outcome:
  - Status → Approved
  - Status → Rejected

---

## ⚙️ Business Rule

### 🔹 Auto Update Status on Approval
**Type:** After Insert / Update  
**Purpose:**
- Automatically update event status based on approval state
- Ensures data consistency without manual intervention

**Logic:**
- If approval state is approved → Status = Approved
- If approval state is rejected → Status = Rejected

---

## 👤 User Roles
- **Requester:** Creates event request (Web & Mobile)
- **Approver (Admin/Manager):** Reviews and approves/rejects events

---

## 🧪 Testing
- Created multiple event records via web and mobile
- Verified UI Policy behavior
- Tested approval flow and status updates
- Confirmed Business Rule execution after update
- Validated mobile experience in ServiceNow Mobile App

---

## 📈 Key Learnings
- ServiceNow Application Scope & Tables
- UI Policies vs Client Scripts
- Business Rule execution timing
- Basic approval automation
- Mobile record experience using App Engine Studio
- End-to-end app lifecycle in ServiceNow

---

## 🚀 Future Enhancements
- Email and mobile push notifications on approval/rejection
- Role-based access control
- Dashboards and reports
- SLA tracking for approvals
- Calendar integration for approved events

---

## 📄 Resume Summary (One Line)
> Developed a ServiceNow-based College Event Management application with web and mobile interfaces using App Engine Studio, including automated approvals, UI policies, and business rules.

---

## 👨‍💻 Author
**Ravi Kiran K**  
ServiceNow CSA & CAD Certified  
Fresher | ServiceNow Developer  

---

## 🔗 Notes
This project was developed as part of **hands-on learning and interview preparation**, focusing on real-world ServiceNow concepts suitable for fresher-level roles.
