# ServiceNowSimulation
This is just a quick simulation of ServiceNow ticket system

# ServiceNow Incident Management Homelab

## Project Overview

This homelab demonstrates the fundamentals of IT Incident Management using a ServiceNow Personal Developer Instance (PDI).

The project simulates an enterprise IT infrastructure incident involving an unreachable Windows Server 2022 Active Directory Domain Controller.

Using ServiceNow, I practiced creating, categorizing, prioritizing, assigning, investigating, documenting, and resolving an IT incident.

The purpose of this project is to develop practical experience with IT Service Management (ITSM) workflows commonly used by Help Desk, Network Operations Center (NOC), and IT Infrastructure support teams.

**Note:** This is a simulated incident management exercise. The reported outage, troubleshooting findings, and corrective actions were simulated. No actual server outage or repair was performed.

---

## Technologies Used

- ServiceNow Personal Developer Instance (PDI)
- ServiceNow Incident Management
- IT Service Management (ITSM)
- Windows Server 2022 (simulated incident target)
- Active Directory Domain Services (AD DS)
- Domain Name System (DNS)
- GitHub Markdown

## Skills Demonstrated

- Incident creation and classification
- Impact and urgency assessment
- Incident priority management
- Assignment group and technician selection
- Incident lifecycle management
- Technical documentation using Work notes
- Incident investigation planning
- Simulated infrastructure troubleshooting
- Resolution documentation
- ITIL-aligned incident management fundamentals

---

## Incident Scenario

**Incident Number:** INC0010010

**Short Description:** Windows Server 2022 Domain Controller Unreachable

**Reported Issue:**

Multiple employees reported being unable to access domain resources. The Windows Server 2022 domain controller was suspected to be unreachable.

**Business Impact:**

Multiple employees experienced interruptions accessing domain-dependent resources.

**Simulated Root Cause:**

The DNS Server service stopped running, causing DNS resolution failures.

**Simulated Resolution:**

The DNS Server service was restarted, DNS resolution was verified, and access to domain resources was restored.

---

# Homelab Walkthrough

<details>
<summary><strong>Step 1: Navigate to ServiceNow Incident Management</strong></summary>

### Objective

Access the ServiceNow Incident Management module and familiarize myself with the incident dashboard.

### Actions Performed

1. Logged into the ServiceNow Personal Developer Instance.
2. Navigated to **All > Incidents**.
3. Opened the incident list.
4. Reviewed existing incident records.
5. Examined important columns, including:
   - Incident Number
   - Caller
   - Priority
   - State
   - Category
   - Assignment Group
   - Assigned To

### What I Learned

The ServiceNow incident dashboard provides a centralized interface for managing IT incidents.

Each incident has a unique identifier that allows IT support teams to track the issue throughout its lifecycle.

The dashboard helps technicians identify outstanding incidents, determine priorities, and monitor assigned work.

### Screenshot (Optional)

![[ServiceNow Incident Dashboard](Screenshots/part1.PNG](https://github.com/ChangITTech/ServiceNowSimulation/blob/7d21860c2407289b7d8550faefb3e92458664903/img/part1.PNG))

</details>

---

<details>
<summary><strong>Step 2: Create a New Incident</strong></summary>

### Objective

Create a new incident record representing a Windows Server 2022 domain controller outage.

### Actions Performed

1. Clicked **New** from the incident dashboard.
2. Opened the New Incident form.
3. Reviewed the available incident fields.
4. Identified the required fields, including Caller and Short Description.
5. Prepared the simulated infrastructure incident.

### Incident Information

**Incident Number:** INC0010010

**Short Description:**

Windows Server 2022 Domain Controller Unreachable

**Description:**

Multiple employees reported being unable to access domain resources.

The domain controller was suspected to be unreachable, and the cause of the outage was initially unknown.

### What I Learned

Creating an incident establishes a formal record of a reported IT issue.

Accurate incident descriptions help technicians understand the symptoms, determine the affected infrastructure, and begin troubleshooting.

### Screenshot (Optional)

![New Incident Form](Screenshots/part2.PNG)

</details>

---

<details>
<summary><strong>Step 3: Configure Incident Classification and Priority</strong></summary>

### Objective

Classify the incident and configure its impact and urgency to determine the appropriate priority.

### Actions Performed

1. Selected Andrew Jackson as the Caller.
2. Selected Network as the Category.
3. Selected DNS as the Subcategory.
4. Selected Phone as the reporting Channel.
5. Set Impact to 2 - Medium.
6. Set Urgency to 1 - High.
7. Verified that ServiceNow automatically calculated Priority 2 - High.
8. Entered the incident description.

### Incident Configuration

| Field | Value |
|---|---|
| Caller | Andrew Jackson |
| Category | Network |
| Subcategory | DNS |
| Channel | Phone |
| Impact | 2 - Medium |
| Urgency | 1 - High |
| Priority | 2 - High |
| Initial State | New |

### What I Learned

ServiceNow determines incident priority based on impact and urgency using its configured priority matrix.

**Impact** measures the extent of the disruption to users or business services.

**Urgency** measures how quickly the incident requires attention.

A Priority 2 - High incident requires prompt investigation and resolution according to organizational service-level targets.

The DNS subcategory was an initial classification, not confirmation of the root cause.

### Screenshot (Optional)

![Incident Priority Configuration](Screenshots/part3.PNG)

</details>

---

<details>
<summary><strong>Step 4: Assign the Incident to an IT Support Team</strong></summary>

### Objective

Assign the incident to a support group and technician responsible for investigating the reported issue.

### Actions Performed

1. Located the Assignment Group field.
2. Selected the Network support group.
3. Located the Assigned To field.
4. Selected David Loo as the assigned technician.
5. Verified the incident remained Priority 2 - High.

### Assignment Information

| Field | Value |
|---|---|
| Assignment Group | Network |
| Assigned To | David Loo |
| Priority | 2 - High |
| Category | Network |
| Subcategory | DNS |

### What I Learned

Assignment groups identify the IT teams responsible for investigating and resolving incidents.

The Assigned To field identifies the individual technician responsible for the incident.

Proper incident assignment establishes accountability and supports escalation between different technical support teams.

### Screenshot (Optional)

![Incident Assignment](Screenshots/part4.PNG)

</details>

---

<details>
<summary><strong>Step 5: Submit and Begin Incident Investigation</strong></summary>

### Objective

Submit the incident and begin tracking its investigation through ServiceNow.

### Actions Performed

1. Clicked Submit to create the incident record.
2. Returned to the incident dashboard.
3. Located incident INC0010010.
4. Reopened the incident record.
5. Verified the incident state was In Progress.
6. Reviewed the assigned technician and support group.
7. Located the Work notes section.

### Incident Status

| Field | Value |
|---|---|
| Incident | INC0010010 |
| State | In Progress |
| Priority | 2 - High |
| Assignment Group | Network |
| Assigned To | David Loo |

### What I Learned

Incident states help IT teams track progress throughout the incident lifecycle.

An incident in the In Progress state indicates that investigation or resolution work is underway.

ServiceNow also maintains an activity history that records updates to incident fields and journal entries.

### Screenshot (Optional)

![Incident In Progress](Screenshots/part6.PNG)

</details>

---

<details>
<summary><strong>Step 6: Document the Investigation Using Work Notes</strong></summary>

### Objective

Document an initial troubleshooting plan using ServiceNow Work notes.

### Actions Performed

1. Navigated to the Notes section.
2. Located the Work notes field.
3. Entered the initial investigation plan.
4. Documented the suspected infrastructure issue.
5. Identified troubleshooting actions.
6. Clicked Post to save the investigation notes.
7. Verified the notes appeared in the incident activity history.

### Investigation Plan

The following troubleshooting steps were documented:

1. Verify the Windows Server 2022 VM is powered on.
2. Test network connectivity using ping.
3. Check DNS resolution using nslookup.
4. Verify Active Directory Domain Services status.
5. Review Windows Event Viewer for relevant errors.

**Root Cause:** Unknown at the beginning of the investigation.

**Investigation Status:** In Progress.

These were planned troubleshooting steps. They were not executed against the actual infrastructure during this exercise.

### What I Learned

ServiceNow Work notes allow IT personnel to document internal technical investigations.

Work notes can include troubleshooting plans, diagnostic results, findings, and actions taken.

Work notes differ from customer-visible comments, which are intended to communicate progress to the affected user.

Maintaining accurate investigation records helps other technicians understand the incident and continue troubleshooting if the ticket is reassigned or escalated.

### Screenshot (Optional)

![Incident Investigation Work Notes](Screenshots/part8.PNG)

</details>

---

<details>
<summary><strong>Step 7: Simulate Troubleshooting and Incident Resolution</strong></summary>

### Objective

Practice documenting a simulated technical resolution for an infrastructure incident.

### Simulated Investigation Findings

For this exercise, the following results were assumed:

1. The Windows Server 2022 domain controller was reachable.
2. DNS resolution for domain resources was failing.
3. The DNS Server service was found stopped.
4. The DNS Server service was restarted.
5. DNS resolution was verified using nslookup.
6. Domain resource accessibility was restored.

### Simulated Root Cause

The DNS Server service had stopped running, preventing successful DNS resolution for domain resources.

### Simulated Corrective Action

The DNS Server service was restarted, and normal DNS functionality was assumed to be restored.

### Resolution Documentation

The simulated corrective actions and results were prepared for the incident's Work notes and Resolution Information fields.

The incident could then be transitioned to the Resolved state.

### What I Learned

Incident resolution requires documenting the reported problem, investigation findings, corrective actions, and outcome.

ServiceNow distinguishes between Resolved and Closed states.

**Resolved:** A solution has been applied and the incident is considered restored.

**Closed:** The incident has completed the organization's closure process.

This scenario demonstrates the documentation workflow for a simulated resolution rather than an actual server repair.

### Screenshot (Optional)

<!-- Add a screenshot of the resolved incident here. -->
<!-- ![Incident Resolution](Screenshots/part9.PNG) -->

</details>

---

## Incident Lifecycle Summary

The homelab followed this incident management workflow:

1. **New** - Create and classify the reported incident.
2. **Prioritization** - Assess impact and urgency.
3. **Assignment** - Assign the responsible support group and technician.
4. **In Progress** - Begin investigation and document findings.
5. **Resolution** - Record corrective actions and resolve the incident.
6. **Closure** - Complete the closure process, where applicable.

---

## Key Takeaways

Through this project, I gained hands-on experience navigating ServiceNow and managing a simulated IT infrastructure incident.

I learned how IT support teams use incident records to document issues, determine priorities, assign responsibility, maintain investigation histories, and record resolutions.

This project strengthened my understanding of ITSM workflows and how ServiceNow supports incident management in enterprise IT environments.

## Future Improvements

- Practice additional incident scenarios involving network connectivity and server availability.
- Simulate incident reassignment and escalation.
- Explore ServiceNow Service Level Agreements (SLAs).
- Practice customer-visible incident updates.
- Perform real troubleshooting in a Windows Server and Ubuntu VirtualBox homelab.
- Explore problem management and change management workflows.

---

## Disclaimer

This project was completed using a ServiceNow Personal Developer Instance for educational purposes.

The infrastructure outage, root cause, and resolution were simulated. ServiceNow ticket creation, configuration, assignment, and initial investigation documentation were performed in the developer environment.

No production systems were affected.
