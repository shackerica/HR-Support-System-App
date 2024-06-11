# HR Support System

## Business Requirements and Goals

The HR team primarily engages with employees via email, resulting in significant inefficiencies and challenges in handling HR-related requests and inquiries. Employees encounter difficulties in submitting and tracking HR tickets, leading to delays in issue resolution and a lack of transparency in service delivery. The absence of a centralized system hampers HR professionals' ability to prioritize, assign, and manage various tasks effectively. Automation in routine processes is lacking, contributing to increased response times, decreased employee satisfaction, and hindered operational efficiency. The HR team seeks an application that:

- Centralizes the management of HR-related requests and inquiries.
- Facilitates effective communication between HR and employees.
- Ensures the confidentiality and security of sensitive HR information.
- Enhances the overall user experience by providing a user-friendly platform.
- Reduces the time it takes to acknowledge and resolve HR requests.
- Utilizes reporting to gather insights and make informed decisions for process improvement.

## Functional Overview

The HR Support System, built within the ServiceNow platform, aims to solve current HR process challenges. Key functionalities include:

- Submission of HR-related requests and inquiries through an intuitive interface.
- Centralized Ticket Management for HR personnel.
- Support for automated workflows for routine HR processes.
- Tracking of ticket status by employees and HR staff.
- Assignment of priority levels to tickets based on urgency and impact.
- Built-in communication features for discussions within the ticketing system.
- Generation of reports and analytics on ticket trends and resolution times.
- Implementation of security measures to protect sensitive HR data.

## Process Overview

### Ticket Creation and Submission

Employees access a custom portal to select from a list of Catalog Items corresponding to different HR Services. Each catalog item acts as an intake form routed to the appropriate group upon submission. Initially, three Catalog items will be built:

1. General HR Inquiry
2. Confidential Inquiry
3. Employee Separation Request

### Ticket Triage

Upon submission, each ticket is automatically assigned to a group based on user selections. The support team performs an initial review to understand the issue's nature, service, and provided information. An initial triage decision is made, which may involve assigning the ticket to an individual, routing it to a different group, or flagging it as work in progress. Once a resolution is reached, the ticket is set to resolved for user verification. The ticket is closed if not reopened within three days after resolution.

### Communication

The system notifies end users and HR support personnel of certain actions on the ticket:

**End user notifications:**
- Email upon ticket submission.
- Email when a comment is added to the ticket.
- Email when the ticket state is set to resolved.
- Email when the ticket state is set to closed.

**HR Support notifications:**
- Email when the ticket is assigned to a group.
- Email when the ticket is assigned to an individual.
- Email when the requester adds a comment to the ticket.

## Service Level Agreements (SLAs)

To maintain quality service, the following SLAs are defined:

- **Response Time:** 15 minutes after ticket submission.
- **Resolution Time:**
  - Priority 1: 4 hours after ticket submission.
  - Priority 2: 2 business days after ticket submission.
  - Priority 3: 5 business days after ticket submission.
  - Priority 4: 10 business days after ticket submission.
