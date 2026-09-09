# SOFTWARE ENGINEERING LAB

## PES University

### Department of Computer Science and Engineering

**Course:** UE24CS341A – Software Engineering  
**Semester:** 5th Semester  
**Academic Year:** 2026–27  

---

## Student Details

| Detail | Information |
|---|---|
| **Name** | Pratham Kumar |
| **SRN** | PES2UG24CS368 |
| **PRN** | PES2202400086 |
| **Section** | F |
| **Course** | UE24CS341A – Software Engineering |
| **University** | PES University |
| **Department** | Computer Science and Engineering |

---

# About Software Engineering

Software Engineering is the systematic and disciplined approach to the development, operation, testing, maintenance, and management of software systems. It applies engineering principles, methods, practices, and structured processes to develop software that is reliable, maintainable, efficient, and suitable for its intended purpose.

Unlike simply writing program code, software engineering considers the complete software development process. It begins with understanding and analysing the problem, identifying the requirements of the users and the system, designing an appropriate solution, implementing the system, testing its behaviour, and maintaining and improving the software throughout its life cycle.

Software engineering also focuses on important software qualities such as correctness, reliability, performance, security, usability, maintainability, and scalability. These qualities help ensure that a software system not only performs its required functions but can also be understood, maintained, and used effectively.

A structured software engineering approach helps developers manage complexity by dividing a large problem into smaller and understandable parts. Techniques such as requirements engineering, UML modelling, architectural design, component modelling, testing, and documentation are used to represent and develop software systems in a systematic manner.

The Software Engineering laboratory provides practical experience in applying these concepts to a given problem statement. Through the laboratory activities, the software system is progressively analysed and modelled, starting from understanding the problem and identifying requirements, followed by system modelling and architectural design.

The laboratory work therefore demonstrates how a software system can be developed systematically from its requirements towards a structured software architecture and component-level design.

---

## Purpose of This Repository

This repository contains the laboratory work completed for the **UE24CS341A – Software Engineering** course at **PES University, Department of Computer Science and Engineering**.

The laboratory work demonstrates the application of software engineering concepts through multiple stages of analysis, modelling, architectural design, and documentation.

The repository contains the work completed for:

- **Lab 1**
- **Lab 2**
- **Lab 3**

Each laboratory extends the work from the previous stage and contributes towards the systematic analysis and design of the selected software system.

---

## Laboratory Work

Detailed explanations and deliverables for **Lab 1, Lab 2, and Lab 3** are provided in their respective sections below.

---
# Lab 1 – Requirements Engineering & UML Use-Case Modelling

## 1. Introduction

Lab 1 focused on **Requirements Engineering and UML Use-Case Modelling** for a given software problem statement. The selected problem for this laboratory was the **Podcast Guest Scheduling & Outline Builder**.

The purpose of the laboratory was to understand a short problem scenario, identify the important functions and constraints of the proposed system, convert them into clear and testable software requirements, identify the actors and their interactions with the system, and represent these interactions using UML Use-Case Modelling.

The laboratory also required the development of a detailed use-case flow for one important system function. Through this process, the problem was gradually converted from a simple textual description into structured software requirements and UML models.

---

## 2. Aim of the Lab

The main aim of Lab 1 was to practice the process of **requirements elicitation, requirements specification, and UML use-case modelling**.

The laboratory required the identification of:

- Functional Requirements (FRs)
- Non-Functional Requirements (NFRs)
- System actors
- Major system use cases
- Relationships between use cases
- Main success scenarios
- Alternate flows

The final requirements had to be clear, verifiable, and measurable so that they could be tested later.

---

## 3. Objective

The objective of Lab 1 was to take a short instructor-provided scenario and:

1. Understand the given problem.
2. Identify the key functions required from the system.
3. Identify important system constraints.
4. Write clear Functional Requirements (FRs).
5. Write measurable Non-Functional Requirements (NFRs).
6. Assign priorities to the requirements.
7. Define measurable acceptance criteria for each requirement.
8. Provide a short rationale for each requirement.
9. Identify the actors interacting with the system.
10. Identify the major use cases.
11. Create a UML Use-Case Diagram.
12. Include at least one `<<include>>` or `<<extend>>` relationship.
13. Select one important use case and document its complete flow.
14. Define the Main Success Scenario.
15. Define at least one Alternate Flow.

The original laboratory instructions required exactly five Functional Requirements and two Non-Functional Requirements, along with the required UML diagram and one-page use-case flow document. :contentReference[oaicite:1]{index=1}

---

# 4. Problem Statement

## Podcast Guest Scheduling & Outline Builder

The selected system is a **media production system designed to simplify the organization of podcast interviews**.

The system allows podcast hosts to share their available interview time slots. Podcast guests can view these available slots and book a suitable time. Guests can also submit discussion topics and biography links for the episode.

The collected information is then used to help prepare the podcast episode by generating structured production information and a run-of-show outline.

Therefore, the system brings together the main activities involved in preparing a podcast interview:

```text
Host Availability Management
          ↓
Guest Slot Selection
          ↓
Interview Booking
          ↓
Guest Information Submission
          ↓
Calendar Information
          ↓
Episode Outline / Production Preparation
```
# 5. Requirements Engineering

After understanding the problem statement, the next step was to identify and document the requirements of the system.

The requirements were divided into two categories:

- **Functional Requirements (FRs)** – describe what the system should do.
- **Non-Functional Requirements (NFRs)** – describe how effectively and securely the system should operate.

Each requirement was documented with:

- Requirement ID
- Requirement Type
- Description
- Priority
- Acceptance Criteria
- Rationale

The acceptance criteria were written in a measurable way so that each requirement could be verified through testing.

---

# 6. Functional Requirements

Five Functional Requirements were identified for the Podcast Guest Scheduling & Outline Builder.

### FR-001 – Interview Slot Booking

The system shall allow podcast guests to select and book an available interview time slot.

The system must ensure that a booking is successful only when the selected slot is available. Already-booked or blocked slots cannot be booked.

**Priority:** High

**Purpose:** Prevent scheduling conflicts and allow guests to book an interview slot.

### FR-002 – Host Availability Management

The system shall allow the Show Host to create, update, and block available interview time slots.

Any changes made by the host must be correctly reflected in the list of slots available to guests.

**Priority:** High

**Purpose:** Allow the Show Host to control interview availability.

### FR-003 – Guest Information Submission

The system shall allow guests to submit structured discussion points and biography links for the podcast episode.

The submitted information must be saved and associated with the correct guest booking.

**Priority:** High

**Purpose:** Collect the information required for episode preparation.

### FR-004 – Calendar Invitation

The system shall send a calendar invitation after a guest successfully books an interview slot.

The calendar invitation must contain the confirmed interview date and time.

**Priority:** Medium

**Purpose:** Keep the host and guest informed about the scheduled interview.

### FR-005 – Run-of-Show Outline Generation

The system shall generate a structured run-of-show episode outline using the submitted guest information and discussion topics.

The generated outline must contain the guest details and submitted discussion topics in a structured format.

**Priority:** High

**Purpose:** Help the Show Host prepare and organize the podcast episode.

---

# 7. Non-Functional Requirements

Two Non-Functional Requirements were identified to define important system qualities.

### NFR-001 – Performance

The system shall generate the formatted PDF production sheet in **under 1 second**.

**Priority:** High

**Purpose:** Ensure fast generation of the required production notes.

### NFR-002 – Security

The system shall restrict host-specific scheduling and episode-management functions to **authorized users**.

Unauthorized users attempting to access host-management functions must be denied access.

**Priority:** High

**Purpose:** Protect scheduling and episode information from unauthorized changes.

---

# 8. Requirements Analysis

The requirements were analysed to understand the main responsibilities of the system.

The Functional Requirements define the primary operations:

```text
FR-001 → Book Interview Slot
FR-002 → Manage Host Availability
FR-003 → Submit Guest Information
FR-004 → Send Calendar Invitation
FR-005 → Generate Run-of-Show Outline
```
# 9. Identification of Actors

After analysing the requirements, the next step was to identify the actors that interact with the Podcast Guest Scheduling & Outline Builder.

Three main actors were identified:

### Podcast Guest

The Podcast Guest is the primary user who interacts with the system for interview scheduling and episode information submission.

The Podcast Guest can:

- View available interview slots.
- Select and book a suitable interview slot.
- Submit guest details.
- Submit discussion points and biography links.

### Show Host

The Show Host manages the interview availability and uses the information collected from the guest for podcast episode preparation.

The Show Host can:

- Create interview time slots.
- Update interview time slots.
- Block interview time slots.
- Manage interview availability.
- Use guest information for episode preparation.
- Generate the run-of-show episode outline.

### Calendar Service

The Calendar Service is an external supporting actor used for calendar-related operations.

It supports the generation of a calendar invitation after a guest successfully books an interview slot.

---

# 10. Identification of Use Cases

Based on the identified requirements and actors, the major use cases of the system were identified.

The main use cases are:

- **Manage Interview Availability**
- **View Available Slots**
- **Book Interview Slot**
- **Submit Guest Details & Discussion Topics**
- **Send Calendar Invitation**
- **Generate Run-of-Show Outline**

Each use case represents a specific function provided by the Podcast Guest Scheduling & Outline Builder.

The identified use cases were mapped to the actors according to their responsibilities and interactions with the system.

---

# 11. UML Use-Case Diagram

After identifying the actors and use cases, a UML Use-Case Diagram was developed to represent the interactions between the users, external service, and the system.

The diagram represents the **Podcast Guest Scheduling & Outline Builder** as the system boundary.

The main elements represented in the diagram are:

- **Podcast Guest**
- **Show Host**
- **Calendar Service**
- **Manage Interview Availability**
- **View Available Slots**
- **Book Interview Slot**
- **Submit Guest Details & Discussion Topics**
- **Send Calendar Invitation**
- **Generate Run-of-Show Outline**

The Podcast Guest interacts with the system for viewing available slots, booking an interview, and submitting guest information.

The Show Host manages interview availability and prepares the podcast episode using the collected guest information.

The Calendar Service represents an external service involved in calendar invitation handling.

The UML Use-Case Diagram therefore provides a visual representation of the system boundary, actors, use cases, and their associations.

---

# 12. Use-Case Relationships

The UML Use-Case Diagram also represents relationships between related use cases.

Two important UML relationships were used: `<<include>>` and `<<extend>>`.

### `<<include>>` Relationship

The **Book Interview Slot** use case has an `<<include>>` relationship with **View Available Slots**.

Viewing the available slots is required as part of the booking process because the Podcast Guest must select an available interview slot before making a booking.

```text
Book Interview Slot
        |
        | <<include>>
        ↓
View Available Slots
```
# 20. Lab 1 Deliverables

The following deliverables were completed as part of Lab 1 – Requirements Engineering & UML Use-Case Modelling.

### 1. Requirements Table

A structured Requirements Table was prepared containing:

- Five Functional Requirements (FRs)
- Two Non-Functional Requirements (NFRs)
- Requirement IDs
- Requirement Types
- Requirement Descriptions
- Priority Levels
- Measurable Acceptance Criteria
- Short Rationales

The requirements covered important system functions such as interview slot booking, host availability management, guest information submission, calendar invitation generation, and run-of-show outline generation. The non-functional requirements addressed system performance and security.

### 2. UML Use-Case Diagram

A UML Use-Case Diagram was created to represent the interaction between the system and its identified actors.

The diagram includes:

- System Boundary
- Podcast Guest
- Show Host
- Calendar Service
- Major System Use Cases
- Actor Associations
- `<<include>>` Relationship
- `<<extend>>` Relationship

The diagram represents the major functionality of the Podcast Guest Scheduling & Outline Builder and shows how the identified actors interact with the system.

### 3. Use-Case Flow Document

A detailed Use-Case Flow was prepared for the key use case:

**UC-02 – Book Interview Slot**

The flow includes:

- Use-Case ID and Name
- Primary Actor
- Supporting Actor
- Purpose
- Preconditions
- Postconditions
- Main Success Scenario
- Alternate Flow

The Main Success Scenario describes the complete process of selecting and booking an available interview slot, recording the booking, generating confirmation, and generating the calendar invitation.

The Alternate Flow describes how the system handles the situation where the selected interview slot is already booked or blocked.

---

# 21. Outcome of Lab 1

Lab 1 established the initial requirements and behavioural understanding of the **Podcast Guest Scheduling & Outline Builder**.

The given problem scenario was analysed and converted into a structured set of Functional and Non-Functional Requirements. The requirements were provided with priorities, measurable acceptance criteria, and rationales, making them clear and verifiable.

The major actors and system use cases were then identified and represented using a UML Use-Case Diagram. The diagram also showed the required `<<include>>` and `<<extend>>` relationships between related use cases.

A detailed use-case flow was also developed for **UC-02 – Book Interview Slot**, covering both the normal successful booking process and the alternate situation where the selected slot is unavailable.

Overall, Lab 1 provided a clear **requirements and behavioural foundation** for the system. It established what the system should do, who interacts with it, and how its key functionality behaves. This foundation was then used for the subsequent software architecture and component-level modelling work.

---

# Lab 2 – Agile Backlog Creation & Sprint Simulation in Jira

## 1. Objective

The main objective of Lab 2 was to use **Jira** to convert the Functional Requirements identified in Lab 1 into an Agile product backlog, organize and prioritize the backlog, estimate the effort using Story Points, simulate sprints, and analyse the progress of the planned work.

The lab helped in understanding how Agile and Scrum practices can be applied to manage software development work in a structured manner.

---

## 2. Work Completed

The **Podcast Guest Scheduling & Outline Builder** project from Lab 1 was continued in Jira.

The following activities were completed:

- Created a Company-managed Scrum project in Jira.
- Created **4 Epics** based on the major functional areas of the system.
- Created **9 User Stories** and linked them to their respective Epics.
- Prioritized the User Stories based on functional importance and dependencies.
- Assigned Story Points using the Fibonacci estimation scale.
- Created a product backlog with a total estimated effort of **33 Story Points**.
- Planned and configured **Sprint 1** with 3 User Stories and **13 Story Points**.
- Planned and completed **Sprint 2** with 6 User Stories and **20 Story Points**.
- Simulated the movement of User Stories through **To Do → In Progress → Done**.
- Used Jira Sprint Reports and Burndown Charts to analyse sprint progress.

The four Epics created were:

1. **Interview Scheduling & Availability Management**
2. **Guest Information & Content Collection**
3. **Calendar & Notification Integration**
4. **Episode Outline & Production Preparation**

The User Stories were written using the Agile format:

> **As a [user role], I want [goal], so that [benefit].**

The complete backlog contained **9 User Stories with 33 Story Points**. :contentReference[oaicite:1]{index=1}

---

## 3. Sprint Simulation

### Sprint 1

Sprint 1 focused on the core interview scheduling functionality.

It contained **3 User Stories with a total of 13 Story Points**, covering:

- Creating interview availability slots
- Viewing available slots
- Booking an interview slot

All three planned User Stories were completed successfully. :contentReference[oaicite:2]{index=2} :contentReference[oaicite:3]{index=3}

### Sprint 2

Sprint 2 focused on the remaining functionality related to:

- Guest information collection
- Calendar notification integration
- Episode production preparation

It contained **6 User Stories with a total of 20 Story Points**, and all planned User Stories were completed. :contentReference[oaicite:4]{index=4}

---

## 4. Deliverables

The Lab 2 deliverables included Jira-based evidence and a short reflection document.

The completed work included:

- Jira backlog containing Epics and User Stories
- Story Point assignments
- Sprint board / Active Sprint view
- Sprint Reports
- Burndown Charts
- Reflection answers analysing estimation, prioritization, sprint planning, and team capacity

The lab therefore demonstrated the complete Agile workflow from **requirements → backlog → estimation → sprint planning → sprint execution → progress analysis**. :contentReference[oaicite:5]{index=5}

---

## 5. Outcome of Lab 2

Lab 2 provided practical experience in applying **Agile and Scrum practices using Jira**.

The Functional Requirements from Lab 1 were successfully transformed into an organized Agile backlog, estimated using Story Points, prioritized, and divided across two simulated sprints.

Both sprints were completed successfully, with **33 total Story Points** completed across the two sprints. The Sprint Reports and Burndown Charts were used to demonstrate and analyse the progress of the simulated development work.

Overall, Lab 2 established an Agile planning and sprint-management view of the same Podcast Guest Scheduling & Outline Builder system developed in Lab 1.

---

# Lab 3 – Component Modelling & Architectural Pattern Selection

## 1. Objective

The main objective of Lab 3 was to analyse different software architectural styles, select the most appropriate architecture for the **Podcast Guest Scheduling & Outline Builder**, and represent the selected architecture using a UML Component Diagram.

The lab focused on understanding how system components are organized, how they communicate through interfaces, and how architectural decisions affect aspects such as maintainability, security, and performance. :contentReference[oaicite:0]{index=0}

---

## 2. Architectural Style Analysis

Three architectural styles were considered:

- **Layered Architecture**
- **Microservices Architecture**
- **Client-Server Architecture**

The strengths and limitations of each style were analysed based on the requirements and scope of the system.

After comparison, **Layered Architecture** was selected as the most appropriate architecture for the Podcast Guest Scheduling & Outline Builder.

The system was organized into:

- Presentation Layer
- Business Layer
- Data Layer

This provided a clear separation between user interaction, application logic, and data management. :contentReference[oaicite:1]{index=1}

---

## 3. Component Identification and Modelling

After selecting the architecture, the major system components and their interfaces were identified.

The component model represents the main application responsibilities, including:

- User Interface Component
- Scheduling & Availability Component
- Guest Information Component
- Episode Outline Generator Component
- Podcast Data Management Component
- External Calendar Service

The interfaces between the components were identified to represent communication and data exchange between different parts of the system.

The UML Component Diagram was created using **draw.io** and shows the component dependencies, interfaces, and major data flows. The diagram follows the layered structure of the selected architecture.

---

## 4. Architecture Justification

The selected **Layered Architecture** was justified based on the system's scope and requirements.

The main reasons were:

- **Clear separation of responsibilities:** Different system functions are organized into appropriate layers, making the system easier to understand and maintain.
- **Suitable for the system scope:** The system has a focused set of related functions and does not require the additional operational complexity of independently deployed microservices.

The architecture also provides a security advantage by allowing authorization checks before host-specific operations reach the data layer. It can also reduce unnecessary communication overhead within the application, supporting the performance requirement for production-sheet generation. :contentReference[oaicite:2]{index=2}

---

## 5. Deliverables

The main deliverables completed for Lab 3 were:

- **UML Component Diagram** showing components, interfaces, dependencies, and data flow.
- **Architecture Justification document** explaining the selected Layered Architecture, reasons for selection, security advantage, and performance benefit.

The final diagram and justification were prepared for submission through the GitHub repository as required by the laboratory instructions. :contentReference[oaicite:3]{index=3}

---

## 6. Outcome of Lab 3

Lab 3 provided practical experience in selecting and applying a software architectural style to the existing system.

The requirements and functionality developed in the previous labs were used to identify system components and their interactions. **Layered Architecture** was selected and represented through a UML Component Diagram, providing a structured view of the Presentation, Business, and Data layers.

The lab therefore extended the work from requirements and Agile planning towards **architectural and component-level design**.
