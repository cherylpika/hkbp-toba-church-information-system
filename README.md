# HKBP Toba Region Church Information System

A web-based church information system developed as a Diploma III final project to centralize congregation data, church information, and administrative records for three HKBP churches in the Toba region. This repository contains the project documentation.

## Project Overview

Based on interviews and direct observation at HKBP Godung Laguboti, HKBP Balige Kota, and HKBP Tiberias Lumban Bulbul, the project documentation found that church administration was still handled manually. Congregation records were kept in written documents or simple spreadsheets, financial records were maintained in Excel, and information was shared through notice boards and weekly bulletins. This created risks of data loss, inconsistent records, slow reporting, and uneven information delivery.

The project aimed to design and build a web-based system that:

- Centralizes congregation, activity, and church information for more than one church in the same service region.
- Supports church administration and financial reporting with role-based access.
- Makes church information available digitally to the congregation.

**Scope and limitations (as stated in the report):**

- Limited to HKBP churches and to the web platform (no mobile application).
- Not integrated with any central HKBP system.
- Advanced security (such as data encryption or two-factor authentication) and automatic notifications (email, SMS, WhatsApp) are out of scope.

## Project Information

- **Project Type:** Academic final-year project (Diploma III Information Technology, Faculty of Vocational Studies, Institut Teknologi Del)
- **Project Year:** 2026
- **Team:** Group project by three students
- **Development Methodology:** Waterfall (Communication, Planning, Modeling, Construction, Deployment)
- **Platform:** Web application
- **Technology Stack:** Laravel 12, PHP, MySQL

## Key Features

The system supports three user roles: Super Admin, Admin (church administrator), and Guest (congregation member).

**Super Admin**
- Manage registered churches (add, edit, delete)
- Review, approve, view, and delete user accounts

**Church Admin** (access limited to their own church)
- Congregation member management
- Sacrament and life-event records: baptism, sidi, marriage, birth, death, and transfer
- Sector management
- Church elders (sintua), service periods, and full-time ministers
- News and announcements
- Daily devotionals
- Worship and partangiangan schedules
- Financial reports (Tingting Parhepengon)
- Profile management

**Guest / Congregation**
- View church news, profile, history, and contact information
- View worship and partangiangan schedules
- Read daily devotionals

## Technology Stack

| Technology | Purpose in the project |
|---|---|
| Laravel 12 | Backend framework (MVC) |
| PHP | Server-side programming language |
| MySQL | Database for congregation and operational data |
| XAMPP | Local server (Apache, PHP, MySQL) for development and testing |
| phpMyAdmin | Database administration |
| Visual Studio Code | Code editor |
| GitHub | Version control and team collaboration |
| Trello | Task planning and progress tracking |

The documentation also lists Bizagi Modeler (BPMN), Figma (UI design), and Enterprise Architect (system modeling) as design tools.

## Testing and Quality Assurance

Testing in this project was **manual**. The project documentation states that no automated testing tools were used.

**Test documentation**
- 41 test scripts (BU-01 to BU-41) cover the implemented modules.
- Each script records an identifier, objective, preconditions, test steps, evaluation criteria, and expected versus observed results.
- Scenarios include both valid and invalid input, for example login with wrong credentials and forms with incomplete data.
- Test scenarios were derived from the project's design documents (workflows, data structure, and interface design).
- The three team members each executed part of the test scripts.

**Test environment**
- Personal laptops, XAMPP local server, Microsoft Edge browser.

**Functional testing**
- Covers CRUD operations, form validation, search, and role-based access (for example, an admin can only access their own church's data).

**Performance testing**
- Apache JMeter load test: 100 virtual users across 8 public endpoints (800 requests in total).
- The report records a 0.00% error rate. The average response time recorded under this load was about 18.3 seconds.

**User Acceptance Testing (UAT)**
- Conducted on 15 January 2026 with a church representative, coordinated by the team.
- Scenarios were grouped by user role. The report states all scenarios were accepted (100% acceptance).

**Not documented:** test automation, API testing, or a regression test suite.

## Key Learnings

- Gathering requirements through interviews and observation of real church administration processes.
- Translating requirements into design artifacts (BPMN, use cases, ERD, class and sequence diagrams) and then into test scripts.
- Writing test cases with expected results, covering both valid and invalid input.
- Verifying role-based access across multiple churches in one system.
- Running a basic load test and reading its results.
- Working with Waterfall documentation and team-based planning.

---

*Developed as part of an academic final-year project at Institut Teknologi Del.*
