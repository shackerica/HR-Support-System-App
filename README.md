# HR Support System App

## Table of Contents
- [Introduction](#introduction)
- [Business Requirements and Goals](#business-requirements-and-goals)
- [Functional Overview](#functional-overview)
- [Process Overview](#process-overview)
- [Design Aspects](#design-aspects)
  - [Tables](#tables)
  - [UI Pages](#ui-pages)
  - [UI Actions](#ui-actions)
  - [Events](#events)
  - [Email Notifications](#email-notifications)
- [Development Process](#development-process)
  - [Sprint 1](#sprint-1)
  - [Sprint 2](#sprint-2)
  - [Sprint 3](#sprint-3)
  - [Sprint 4](#sprint-4)
  - [Sprint 5](#sprint-5)
  - [Sprint 6](#sprint-6)

## Introduction
The HR Support System App is designed to streamline HR processes by centralizing ticket management, enhancing communication, and improving service efficiency. Built on the ServiceNow platform, this app ensures secure, efficient, and transparent handling of HR-related requests and inquiries.

## Business Requirements and Goals
The HR team facilitates the majority of their employee engagements through email. The current approach to handling HR-related requests and inquiries within the organization has resulted in significant inefficiencies and challenges:
- Employees face difficulties in submitting and tracking HR tickets, leading to delays in issue resolution and a lack of transparency.
- The absence of a centralized system makes it challenging for HR professionals to prioritize, assign, and manage various HR tasks effectively.
- The lack of automation in routine processes has contributed to increased response times, decreased overall employee satisfaction, and hindered the HR team's ability to operate at peak efficiency.

The HR team is requesting an application that provides the following capabilities:
- Centralize the management of HR-related requests and inquiries.
- Facilitate effective communication between HR and employees.
- Ensure the confidentiality and security of sensitive HR information.
- Enhance the overall experience for employees by providing a user-friendly platform for submitting requests, tracking progress, and obtaining HR-related information.
- Reduce the time it takes to acknowledge and resolve HR requests.
- Utilize reporting to gather insights into HR operations, identify trends, and make informed decisions to continuously improve processes.

## Functional Overview
The proposed HR Support System aims to solve challenges presented by the current HR process. The application will be built within the ServiceNow platform, providing both the HR team and end-users with their own space within the platform. The functionalities to be built throughout the project include:
- Employees can submit HR-related requests and inquiries through an intuitive and user-friendly interface.
- Centralized Ticket Management that allows HR personnel to manage all requests and inquiries within a single platform.
- Support automated workflows for routine HR processes.
- Employees and HR staff can track the status of each ticket.
- Tickets can be assigned priority levels based on urgency and impact.
- Built-in communication features for discussions within the ticketing system.
- Generate reports and analytics on ticket trends, resolution times, and other key metrics.
- Implement security measures to protect sensitive HR data.

## Process Overview
### Ticket Creation and Submission
Employees will be provided a custom portal where they can select from a list of Catalog Items pertaining to different HR Services. Each catalog item will serve as an intake form and will have specific fields that HR requires for them to work on the request. Each catalog item will be routed to the appropriate group upon submission. The initial phase of this project will only require the team to build 3 Catalog items to demonstrate the tool’s capability. The system will be designed to accommodate more catalog items that would drive specific and more granular processes.

The Catalog items that would be built under this project are:
- General HR Inquiry
- Confidential Inquiry
- Employee Separation Request

### Ticket Triage
The ticket triage process will guide the HR support team to successfully fulfill the request. The process comprises the following internal activities:
- Each ticket will automatically be assigned to a group depending on selections made by the end users during the ticket submission process.
- The support team performs an initial review of each ticket to understand the nature of the issue, service, and any relevant information provided by the user.
- Based on the initial review, an initial triage decision is made. This decision may involve assigning the ticket to an individual, routing it to a different group, or flagging it as work in progress to provide resolution or to further investigate.
- Once a resolution is reached, the team sets the ticket to resolved, allowing users to verify the resolution.
- The final step to this process is met when the ticket is set to closed. Auto-closure is done when the ticket has not been reopened 3 days after ticket resolution.

### Communication
The system notifies the end user and HR support on certain actions on the ticket.

**End user notifications:**
- An email is sent out to the end user upon ticket submission.
- An email is sent out to the end user when a comment is added to the ticket.
- An email is sent out to the end user when the ticket state has been set to resolved.
- An email is sent out to the end user when the ticket state has been set to closed.

**HR Support notifications:**
- An email is sent out when the ticket is assigned to a group.
- An email is sent out when the ticket is assigned to an individual.
- An email is sent out when the requester adds a comment to the ticket.

### Service Level Agreements
The HR Management is committed to providing quality and efficient service; therefore, a set of service measurements will be put in place to make sure that the level of service is always met.

SLAs definitions for the following will be created to keep track of HR support performance:
- **Response Time**: The time it takes for HR Support to acknowledge a request. This will be set to 15 minutes after ticket submission.
- **Resolution Time**: The time it takes for the service provider to resolve a reported issue or fulfill a service request.
  - Priority 1: 4 hours after ticket submission
  - Priority 2: 2 business days after ticket submission
  - Priority 3: 5 business days after ticket submission
  - Priority 4: 10 business days after ticket submission

## Design Aspects
### Tables

#### Human Resource Table

- **Description:** This table stores information about human resources.
- **Structure:**

  ![Human Resource Table Structure](https://github.com/shackerica/HR-Support-System-App/assets/19885127/2f83bc8a-9dba-46e2-adb9-5e7dad42aaec)


- **Relationships:**
  - Extends the Task Table.

- **Prefix:** HR
- **Auto-numbering:** Enabled
- **Role Permissions:**
  - `x_419821_hr.hr_admin`: Assigned to the User role field.

#### HR Task Table

- **Description:** This table manages tasks related to human resources.
- **Structure:**

  ![HR Task Table Structure](https://github.com/shackerica/HR-Support-System-App/assets/19885127/5c39cf47-2c06-479c-8140-b26b05086752)


- **Relationships:**
  - Extends the Task Table.

- **Prefix:** HRT
- **Auto-numbering:** Enabled
- **Role Permissions:**
  - `x_419821_hr.hr_task_user`: Assigned to the User role field.


### UI Pages


### UI Actions


### Events


### Email Notifications


## Development Process
### Sprint 1: 
[View Sprint 1 Details](https://github.com/shackerica/HR-Support-System-App/blob/main/Sprints/Sprint1.pdf)

### Sprint 2
[View Sprint 2 Details](https://github.com/shackerica/HR-Support-System-App/blob/main/Sprints/Sprint2.pdf)

### Sprint 3
[View Sprint 3 Details](https://github.com/shackerica/HR-Support-System-App/blob/main/Sprints/Sprint3.pdf)

### Sprint 4
[View Sprint 4 Details](https://github.com/shackerica/HR-Support-System-App/blob/main/Sprints/Sprint4.pdf)

### Sprint 5
[View Sprint 5 Details](https://github.com/shackerica/HR-Support-System-App/blob/main/Sprints/Sprint5.pdf)

### Sprint 6
[View Sprint 6 Details](https://github.com/shackerica/HR-Support-System-App/blob/main/Sprints/Sprint6.pdf)


## Demo


## Skills Used
![HTML5](https://img.shields.io/badge/HTML5-E34F26?style=flat&logo=html5&logoColor=white)
![JavaScript](https://img.shields.io/badge/JavaScript-F7DF1E?style=flat&logo=javascript&logoColor=black)
![jQuery](https://img.shields.io/badge/jQuery-0769AD?style=flat&logo=jquery&logoColor=white)
![ServiceNow](https://img.shields.io/badge/ServiceNow-5CB85C?style=flat&logo=servicenow&logoColor=white)
