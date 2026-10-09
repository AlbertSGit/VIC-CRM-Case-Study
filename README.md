<p align="center">
  <img src="assets/cover.svg" alt="VIC CRM - custom web application case study" width="100%">
</p>

<p align="center"><strong>Real business workflows · Responsive interface · Relational data · API integrations</strong></p>

<p align="center">JavaScript / HTML / CSS &nbsp; · &nbsp; PHP &nbsp; · &nbsp; MySQL / SQL &nbsp; · &nbsp; REST API / JSON</p>

# VIC CRM

A custom web application supporting everyday operations in the medical and cosmetology sector. Built around real business processes, with functionality developed iteratively using user feedback.

**Author:** [Albert Smoliński](https://github.com/AlbertSGit)  
**Documented development period:** May - August 2026  
**Repository scope:** Portfolio documentation. Application source code is not included.

## Application preview

Actual VIC CRM screens showing a test client and sample appointment. The interface is in Polish.

### Appointment calendar

The weekly calendar keeps appointments and the selected visit in one view. The side panel brings together visit status, timing, services, series and settlement controls.

<p align="center">
  <a href="assets/01-calendar-visit.png"><img src="assets/01-calendar-visit.png" alt="VIC CRM weekly calendar with a test appointment and visit details" width="100%"></a>
</p>

### Client overview

A single client view combines visit history, recent activity, notes and follow-up actions.

<p align="center">
  <a href="assets/02-client-overview.png"><img src="assets/02-client-overview.png" alt="VIC CRM test client overview with appointment history and follow-up actions" width="100%"></a>
</p>

<details>
<summary><strong>Explore the workflow: adding a client</strong></summary>

A focused dialog collects client details, assigns an employee and records the acquisition source and segment.

<p align="center">
  <a href="assets/03-add-client.png"><img src="assets/03-add-client.png" alt="New client dialog with name, phone, employee, email, source and segment fields" width="100%"></a>
</p>

</details>

<details>
<summary><strong>Explore the workflow: calendar actions</strong></summary>

Selecting a time slot exposes three actions: a new appointment, a time reservation or a time block.

<p align="center">
  <a href="assets/04-calendar-actions.png"><img src="assets/04-calendar-actions.png" alt="Calendar time-slot menu with new appointment, reservation and time block actions" width="100%"></a>
</p>

</details>

### Mobile calendar

The mobile view presents the day's schedule with date navigation, appointment cards and bottom navigation for Calendar, Clients, Tasks and Profile.

<p align="center">
  <a href="assets/05-mobile-calendar.jpeg"><img src="assets/05-mobile-calendar.jpeg" alt="VIC CRM mobile daily calendar with a test appointment and bottom navigation" width="310"></a>
</p>

<p align="center"><sub>Click any screenshot to view it at full size. VIC CRM · Albert Smoliński</sub></p>

---

## Business context

Managing clients, appointments, documentation, service series, settlements and tasks involves interconnected workflows. VIC CRM brings these areas into one application and supports access from desktop computers, tablets and mobile devices.

## My contribution

- Designed functionality based on real operational needs and refined it through user feedback.
- Developed the desktop, mobile and tablet interface in JavaScript, HTML and CSS.
- Implemented asynchronous communication and data updates using AJAX and `fetch`.
- Implemented backend logic in PHP and operations on a relational MySQL database.
- Designed integrations and data synchronization using REST API and JSON.

## Functional scope

| Area | Scope described in the project |
| --- | --- |
| Clients | Client records supporting daily operations |
| Appointments | Visit management |
| Documentation | Documentation connected with operational workflows |
| Service series | Management of multiple-service workflows |
| Settlements | Settlement records and related business operations |
| Tasks | Tasks supporting the team's work |
| Integrations | Communication and data synchronization with external services |
| Responsive UI | Desktop, tablet and mobile interfaces |

## Architecture overview

The diagram below is a conceptual overview based on the technologies used. It deliberately omits endpoints, database structure and deployment details.

```mermaid
flowchart TD
    UI["Responsive web interface"]
    PHP["PHP application backend"]
    DB["MySQL database"]
    EXT["External services"]
    UI -->|"AJAX / fetch"| PHP
    PHP -->|"SQL operations"| DB
    PHP <-->|"REST API / JSON"| EXT
```

| Layer | Technologies | Responsibility |
| --- | --- | --- |
| Interface | JavaScript, HTML, CSS | Responsive screens and asynchronous updates |
| Application | PHP | Backend logic and data operations |
| Data | MySQL, SQL | Relational storage |
| Integration | REST API, JSON | External communication and synchronization |

## QA perspective

This project connects application development with my background in software testing. Its linked workflows provide practical examples for discussing data consistency, error handling and regression risk during a technical interview.

The following are **suggested validation areas**, not a claim that an automated test suite or specific coverage level has been delivered:

- Consistency of client and appointment data across related screens.
- Validation of required fields and handling of invalid input.
- Service-series and settlement flows, including repeated user actions.
- Failed asynchronous requests and recovery without displaying stale data.
- Integration failures and synchronization behavior.
- Responsive behavior on desktop, tablet and mobile screens.

## About this repository

This case study describes the application and my implementation scope. It does not expose the source code, production configuration or real client records, and is not intended as evidence of code quality or automated test coverage.

**Albert Smoliński** · [GitHub](https://github.com/AlbertSGit) · [LinkedIn](https://www.linkedin.com/in/AlbertSm12)
