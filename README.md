# Employee Lifecycle Management | ServiceNow Zurich

## Overview

Employee Lifecycle Management is a custom ServiceNow application developed on the **ServiceNow Zurich** platform to automate the complete employee onboarding and offboarding lifecycle. The application streamlines HR operations by managing employee records, approvals, asset allocation, notifications, and reporting through low-code automation.

This project demonstrates real-world ServiceNow development using custom tables, Flow Designer, Business Rules, Record Producers, Reports, and Notifications.

---

## Features

### Employee Management

* Create and manage employee records
* Auto-generated Employee IDs
* Default employee status assignment
* Manager reference using the User table

### Employee Onboarding

* Employee Onboarding Request
* HR Approval creation
* Asset allocation
* Status updates
* Email notifications

### Employee Offboarding

* Employee Exit Request
* Exit approval workflow
* Asset return process
* Employee status update
* Exit notification email

### Automation

* Flow Designer
* Business Rules
* Notifications
* Record Producers

### Reporting

* Employee Status Report
* Department-wise Employees Report
* Onboarding Requests Report
* Offboarding Requests Report
* HR Approval Status Report
* Asset Allocation Status Report

---

## Technologies Used

| Technology             | Purpose                       |
| ---------------------- | ----------------------------- |
| ServiceNow Zurich      | Application Development       |
| Flow Designer          | Workflow Automation           |
| Business Rules         | Server-side Automation        |
| Record Producers       | User-friendly Record Creation |
| Notifications          | Email Automation              |
| Reports                | Data Visualization            |
| Access Controls (ACLs) | Security                      |
| Custom Tables          | Data Management               |

---

## Application Modules

### Employee

Stores employee information including:

* Employee ID
* Employee Name
* Department
* Designation
* Email
* Manager
* Status

### Onboarding Request

Captures employee onboarding requests and initiates approval and asset allocation workflows.

### Offboarding Request

Handles employee exit requests and automates the offboarding process.

### HR Approval

Tracks approval requests for onboarding and offboarding.

### Asset Allocation

Maintains employee asset allocation records.

---

## Business Rules

### Auto Generate Employee ID

Automatically generates a unique Employee ID whenever a new employee record is created.

### Set Default Employee Status

Automatically assigns **Onboarding** as the default employee status during record creation.

---

## Flow Designer

### Employee Onboarding Flow

* Trigger: Onboarding Request Created
* Update Request Status
* Create HR Approval Record
* Create Asset Task
* Create Asset Allocation Record

### Employee Offboarding Flow

* Trigger: Offboarding Request Created
* Update Request Status
* Create HR Approval
* Create Asset Return Tasks
* Update Employee Status
* Complete Offboarding Request

---

## Record Producers

* Employee Onboarding Request
* Employee Exit Request

---

## Notifications

### Welcome to ABC Company!

Sent after successful onboarding.

### Exit Process Completed

Sent after successful offboarding.

---

## Reports

* Employee Status Report
* Department-wise Employees
* Onboarding Requests
* Offboarding Requests
* HR Approval Status
* Asset Allocation Status

---

## Project Architecture

```text
Employee
      │
      ├──────────────┐
      │              │
Onboarding      Offboarding
      │              │
      ▼              ▼
HR Approval    HR Approval
      │              │
      ▼              ▼
Asset Allocation   Asset Return
      │              │
      └──────► Notifications
                     │
                     ▼
                  Reports
```

---

## Screenshots

The repository contains screenshots demonstrating:

* Application Overview
* Employee Table
* Onboarding Request
* Offboarding Request
* HR Approval
* Asset Allocation
* Business Rules
* Flow Designer
* Record Producers
* Notifications
* Reports

---

## Learning Outcomes

Through this project I gained practical experience in:

* Custom Application Development
* Table Design
* Flow Designer
* Business Rules
* Record Producers
* Email Notifications
* Reporting
* ServiceNow Studio
* Access Controls (ACLs)
* Application Security
* End-to-End HR Process Automation

---

## Future Enhancements

* Service Portal Integration
* Employee Self-Service Portal
* Performance Analytics Dashboard
* SLA Tracking
* Mobile Experience
* Integration with Microsoft Teams and Active Directory

---

## Author

**Bobbili Chandana Sri**

B.Tech Computer Science Engineering

ServiceNow Certified System Administrator (CSA)

ServiceNow Certified Application Developer (CAD)

GitHub: https://github.com/chandanasri26

LinkedIn: https://linkedin.com/in/bobbili-chandana-sri

---

## License

This project is developed for educational purposes and to demonstrate ServiceNow application development skills.
