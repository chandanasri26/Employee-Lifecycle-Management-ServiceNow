# Employee Lifecycle Management | ServiceNow Zurich

## Overview

Employee Lifecycle Management is a custom application developed on the **ServiceNow Zurich** platform to automate the complete employee onboarding and offboarding lifecycle. The application streamlines HR operations by managing employee records, approvals, asset allocation, notifications, and reporting through low-code automation.

This project demonstrates end-to-end ServiceNow application development using **Custom Tables, Flow Designer, Business Rules, Record Producers, Notifications, Reports, ACLs, and Update Sets**.

---

# 🚀 Project Highlights

* Developed a custom Employee Lifecycle Management application on **ServiceNow Zurich**
* Designed **5 custom tables** with relational data modeling
* Automated onboarding and offboarding using **Flow Designer**
* Implemented **Business Rules** for Employee ID generation and default status assignment
* Created **Record Producers** for user-friendly request submission
* Configured **Email Notifications** for onboarding and offboarding events
* Developed **6 analytical reports** for HR monitoring
* Packaged the application using **ServiceNow Update Sets** for deployment

---

# Features

## Employee Management

* Create and manage employee records
* Auto-generate Employee IDs
* Default employee status assignment
* Manager reference using the User table

## Employee Onboarding

* Employee Onboarding Request
* HR Approval creation
* Asset allocation
* Status updates
* Welcome email notification

## Employee Offboarding

* Employee Exit Request
* HR approval workflow
* Asset return process
* Employee status update
* Exit notification email

## Automation

* Flow Designer
* Business Rules
* Record Producers
* Notifications

## Reporting

* Employee Status Report
* Department-wise Employees Report
* Onboarding Requests Report
* Offboarding Requests Report
* HR Approval Status Report
* Asset Allocation Status Report

---

# Technologies Used

| Technology             | Purpose                       |
| ---------------------- | ----------------------------- |
| ServiceNow Zurich      | Application Development       |
| Flow Designer          | Workflow Automation           |
| Business Rules         | Server-side Automation        |
| Record Producers       | User-friendly Record Creation |
| Notifications          | Email Automation              |
| Reports                | Data Visualization            |
| Access Controls (ACLs) | Application Security          |
| Custom Tables          | Data Management               |
| Update Sets            | Application Migration         |

---

# Application Modules

## Employee

Stores employee master information.

**Fields**

* Employee ID
* Employee Name
* Email
* Department
* Designation
* Manager
* Status

---

## Onboarding Request

Captures onboarding requests and automatically initiates the onboarding workflow.

---

## Offboarding Request

Captures employee exit requests and initiates the offboarding workflow.

---

## HR Approval

Stores approval records generated automatically during onboarding and offboarding.

---

## Asset Allocation

Maintains company asset allocation details for employees.

---

# Business Rules

## Auto Generate Employee ID

Automatically generates a unique Employee ID whenever a new employee record is created.

## Set Default Employee Status

Automatically assigns **Onboarding** as the default employee status if no status is provided.

---

# Flow Designer

## Employee Onboarding Flow

**Trigger**

* Onboarding Request Created

**Actions**

* Update Request Status
* Create HR Approval Record
* Create Asset Task
* Create Asset Allocation Record
* Send Welcome Email

---

## Employee Offboarding Flow

**Trigger**

* Offboarding Request Created

**Actions**

* Update Request Status
* Create HR Approval
* Create Asset Return Task
* Update Employee Status
* Send Exit Notification

---

# Record Producers

* Employee Onboarding Request
* Employee Exit Request

---

# Notifications

## Welcome to ABC Company!

Automatically sent after successful onboarding.

## Exit Process Completed

Automatically sent after successful offboarding.

---

# Reports

The application includes six reports for monitoring employee lifecycle activities.

* Employee Status Report
* Department-wise Employees Report
* Onboarding Requests Report
* Offboarding Requests Report
* HR Approval Status Report
* Asset Allocation Status Report

---

# Repository Structure

```text
Employee-Lifecycle-Management-ServiceNow
│
├── README.md
├── UpdateSet/
│   └── Employee_Lifecycle_Management_Update_Set.xml
│
├── Documentation/
│   ├── System_Architecture.pdf
│   ├── Database_Schema.pdf
│   ├── Flow_Diagram.pdf
│   ├── Business_Rules_Explanation.pdf
│   ├── Notifications_Explanation.pdf
│   └── Reports_Explanation.pdf
│
└── Screenshots/
    ├── Application.png
    ├── Employee_Table.png
    ├── Onboarding_Request.png
    ├── Offboarding_Request.png
    ├── HR_Approval.png
    ├── Asset_Allocation.png
    ├── Employee_Onboarding_Flow.png
    ├── Employee_Offboarding_Flow.png
    ├── Business_Rules.png
    ├── Notifications.png
    └── Reports.png
```

---

# Deployment

To deploy this application into another ServiceNow instance:

1. Import the **Employee_Lifecycle_Management_Update_Set.xml** file.
2. Preview the Update Set.
3. Commit the Update Set.
4. Verify the custom tables, Business Rules, Flows, Notifications, and Reports.
5. Test the onboarding and offboarding workflows.

---

# Key Skills Demonstrated

* ServiceNow Studio
* Flow Designer
* Business Rules
* Record Producers
* Notifications
* Reports
* Update Sets
* Access Controls (ACLs)
* Custom Tables
* Workflow Automation
* HR Process Automation

---

# Learning Outcomes

This project provided practical experience in:

* Custom Application Development
* Table Design and Relationships
* Workflow Automation
* Business Rule Implementation
* Email Notification Configuration
* Reporting and Analytics
* Application Security
* Update Set Migration
* End-to-End HR Process Automation

---

# Future Enhancements

* Employee Self-Service Portal
* Service Portal Integration
* Manager Approval Workflow
* Performance Analytics Dashboard
* SLA Tracking
* Mobile Application Support
* Microsoft Teams Integration
* Active Directory Integration

---
# Conclusion

This project demonstrates end-to-end ServiceNow application development by combining custom application design, automation, reporting, and deployment. It reflects practical experience in building business solutions using the ServiceNow platform.

---
# Author

**Bobbili Chandana Sri**

B.Tech – Computer Science Engineering

**ServiceNow Certified System Administrator (CSA)**

**ServiceNow Certified Application Developer (CAD)**

**GitHub:** https://github.com/chandanasri26

**LinkedIn:** https://linkedin.com/in/bobbili-chandana-sri

---

# License

This project is developed for educational purposes to demonstrate practical ServiceNow application development skills.

---


