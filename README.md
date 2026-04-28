Automated Employee Onboarding & Offboarding System

Platform
ServiceNow Developer Instance

Overview
A fully automated HR workflow system built on ServiceNow that manages employee onboarding and offboarding requests—from request submission to final task completion—using Flow Designer with zero custom scripting.
The system improves HR efficiency by automating approvals, task assignments, notifications, and employee lifecycle tracking across departments such as HR, IT, Facilities, and Security.

Features
Employee submits onboarding/offboarding request via Service Portal
Automatic manager approval workflow
Auto-generation of IT, Facilities, and Security tasks after approval
Rejection handling with requester notification and request cancellation
Email notifications at every important workflow stage
Complete request tracking using a custom Employee Lifecycle table
Dynamic UI Policies for onboarding and offboarding request types
Role-based access control using ServiceNow roles and groups

Key Components
Roles & Groups
Role	Group	Responsibility
hr.manager	HR – People Ops	Approval management
it.admin	IT Team	Account provisioning
facilities.staff	Facilities Team	Workspace preparation
security.officer	Security Team	Access and badge management
Custom Table
u_employee_lifecycle

Stores employee request details including:
Employee ID
Requested For
Department
Manager
Joining Date / Exit Date
Request Type
RITM
Status
Catalog Item
Onboard New Employee

Service Catalog form containing:
11 input variables
Dynamic UI Policies
Conditional field visibility based on:
Onboarding
Offboarding
This ensures users only see relevant fields based on request type.

Flow Designer
On or Off Boarding Flow
16-Step Automated Flow
Get Catalog Variables
Create Employee Lifecycle Record
Ask For Approval (Manager)
If Approved
Send Approval Email
Create IT Task
Create Facilities Task
Create Security Task
Wait for All Tasks Completion
Update Employee Lifecycle Record
Update Requested Item (RITM)
Send Completion Email
If Rejected
Update Records
Cancel Request
Send Rejection Email
Technologies Used
ServiceNow Flow Designer
Service Catalog
Catalog Builder
Custom Tables
UI Policies
Role-Based Access Control (ACLs)
ServiceNow Notifications
Approval Workflows
Developer Instance

Author
M N Niharika Shree
B.E. Computer Science – Data Science
Ballari Institute of Technology and Management
GitHub: https://github.com/niharikashree
LinkedIn: https://www.linkedin.com/in/m-n-niharika-shree-886915279/
