# Enterprise Incident & Problem Management Implementation in ServiceNow

## Project Overview

This project demonstrates the implementation of an ITIL-aligned Incident and Problem Management solution using the ServiceNow platform.

The goal of the project was to simulate a real enterprise IT support environment by configuring incident workflows, automation rules, SLA tracking, reporting dashboards, and problem management for recurring issues.

The implementation shows how ServiceNow can streamline IT support operations by automatically assigning tickets to the correct support teams, prioritizing incidents based on impact and urgency, tracking resolution timelines through SLAs, and identifying root causes for repeated incidents.

---

## Incident Management Implementation

A complete Incident Management workflow was configured to manage the lifecycle of IT support tickets.

Incident lifecycle states implemented:

New → In Progress → On Hold → Resolved → Closed

Sample incidents were created to simulate real IT support scenarios including:

• VPN not connecting for remote employee  
• Laptop screen flickering intermittently  
• Outlook email not sending messages  
• Wi-Fi disconnecting on second floor  
• Printer not responding in finance department  
• Teams application crashing on startup  
• Shared drive access denied  

These incidents were used to test automation logic, SLA tracking, and reporting dashboards.

---

## Priority Automation

Incident priority is automatically calculated using Impact and Urgency through a Client Script.

Example logic:

Impact 1 + Urgency 1 → Priority 1 (Critical)

Impact 2 + Urgency 2 → Priority 2 (High)

Lower impact incidents receive lower priority levels.

This ensures that business-critical issues are handled first.

---

## Automatic Incident Assignment

A Business Rule was implemented to automatically assign incidents to the appropriate support group based on the selected category.

Assignment logic:

Network incidents → Network Support  
Hardware incidents → Hardware Support  
Software incidents → Application Support  

This automation improves ticket routing efficiency and reduces manual triage work for IT support teams.

---

## SLA Management

A Service Level Agreement (SLA) was configured to monitor incident resolution timelines.

Configured SLA:

Incident Resolution Time — 4 Hours

The SLA automatically attaches to incidents and tracks the remaining time available for resolution. This helps ensure service delivery targets are met and provides visibility into potential SLA breaches.

---

## Reporting & Dashboards

Reports were created to visualize incident data and operational trends.

Reports implemented:

• Incidents by Category  
• Incidents by Priority  

These reports were added to a dashboard to provide a quick overview of incident distribution and workload.

---

## Problem Management

To demonstrate Problem Management, a problem record was created for recurring VPN connectivity issues.

Problem created:

Recurring VPN Connectivity Failures

Multiple related incidents were linked to this problem record to represent repeated user issues.

This process helps identify root causes and prevents recurring incidents.

---

## Key Features Implemented

• Incident lifecycle management  
• Automatic ticket assignment using Business Rules  
• Priority automation using Client Scripts  
• SLA tracking for incident resolution  
• Reporting and operational dashboards  
• Problem management for recurring issues  

---

## Project Outcome

This project demonstrates how ServiceNow can automate IT support workflows, improve ticket routing efficiency, track service performance through SLAs, and identify recurring issues using problem management.

The implementation reflects how enterprise organizations manage IT service operations using the ServiceNow platform.

---
## Screenshots

The following screenshots demonstrate the configuration and testing of the ServiceNow Incident and Problem Management implementation.

![Incident List](screenshots/incident-list.png)
![Assignment Groups](screenshots/assignment-groups.png)
![Business Rule](screenshots/business-rule-auto-assignment.png)
![Auto Assignment](screenshots/incident-auto-assignment-working.png)
![Client Script](screenshots/priority-client-script-config.png)
![SLA](screenshots/incident-sla-running.png)
![Dashboard](screenshots/incident-management-dashboard.png)
![Problem Record](screenshots/problem-record.png)
