# 🏢 Conference Room Booking System

The Conference Room Booking System is an internal organisational platform designed to manage the booking and use of shared conference rooms. Its primary purpose is to enable employees to view room availability, create and manage bookings, and prevent scheduling conflicts in a simple and reliable manner.

The system supports multiple user roles, including employees, administrators, reception staff, and facilities managers, each with distinct responsibilities and access levels. Administrative users gain visibility into room usage, conflicts, and reports, while operational roles can manage visitor bookings and room maintenance schedules.

At its current stage, the system is documented through Agile artefacts such as user stories, sprint plans, and execution records. Future iterations will introduce a fully implemented user interface, backend services, APIs, and supporting infrastructure to transform the system from a documentation-driven project into a working application.

---

## 📌 Purpose of This Repository

The purpose of this repository is to demonstrate professional software development practices focused on documentation, collaboration, and Agile processes rather than full system implementation.

It serves as a learning and simulation environment where Scrum artefacts such as user stories, sprint plans, daily standups, reviews, and retrospectives are created, reviewed, and maintained using industry-standard tools and workflows. The repository is used to practise Git and GitHub fundamentals, including branching strategies, Pull Requests, issue reporting, and peer reviews.

Over time, the repository is intended to evolve from a documentation-focused project into a more technically complete system, with future additions such as API specifications, architecture documentation, and implementation guidelines. This staged approach reflects real-world software development, where strong communication and process foundations are established before full-scale development begins.

## 🗂 Repository Contents

This repository is organised to support Agile documentation, collaboration, and sprint execution.

- README.md
Provides a high-level overview of the project, its purpose, system context, onboarding guidance, and contribution workflow.

- sprint/
Contains all sprint-related artefacts created during Scrum simulations, including:

 * Sprint planning records

 * Daily standups

 * Mid-sprint checkpoints

 * Sprint reviews

 * Sprint retrospectives

 * Sprint summaries

- Process Documentation (Markdown files)
Includes user stories, epics, prioritisation matrices, definitions of done, and reflection documents that support backlog management and sprint execution.

- .github/
Contains issue templates and configuration files that guide consistent communication when reporting bugs or proposing improvements.

- .gitignore
Specifies files and directories that should not be tracked by Git.

- LICENSE
Defines the licensing terms for the repository.

As the project evolves, additional folders will be introduced for implementation code, API documentation, and technical setup instructions.

## ⚙️ Installation

At this stage, the Conference Room Booking System does not require any software installation or runtime setup.

The repository currently focuses on documentation, Agile process simulation, and collaboration workflows, APIs rather than a fully implemented application.

- To get started:

 * Clone the repository:

   * git clone https://github.com/<your-username>/conference-room-booking-system.git
 

 * Open the repository in a text editor (such as VS Code) to review the documentation and sprint artefacts.

---

## 🚀 Usage

- Reviewing and creating Scrum artefacts such as user stories, sprint plans, daily standups, reviews, and retrospectives

- Practising Git and GitHub workflows, including branching, Pull Requests, issue reporting, and peer reviews

- Simulating sprint execution and documenting progress using markdown files

- Collaborating with peers on documentation and process improvements

## 🤝 Contributing

All changes to the Conference Room Booking System repository are made via Pull Requests (PRs) to ensure collaboration, review, and quality control.

### Workflow Steps:

* Branch Creation

Contributors create a new branch from main for each feature, documentation update, or bug fix.

Branch naming follows the format:

feature/<short-description>
doc/<short-description>
bugfix/<short-description>


* Make Changes

Contributors implement updates in their branch, which can include documentation, user stories, sprint artefacts, or future technical additions.

* Commit messages should be clear, concise, and descriptive.

* Open a Pull Request

The contributor submits a PR from their branch to the main branch.

The PR title and description explain the purpose of the change.

* Review Process

Team members or supervisors review the PR for clarity, accuracy, and alignment with project standards.

Feedback is provided via comments. Contributors make updates as needed.

* Approval and Merge

Once the PR is approved and passes checks, it is merged into main.

This ensures the repository maintains a single, verified source of truth.

* Traceability and Documentation

PRs act as a record of changes, supporting transparency and accountability.

Each sprint’s work can be traced through PRs corresponding to sprint artefacts or features.

---

## Developer Onboarding (In Progress)


- Clone the Repository

 * git clone https://github.com/<https://github.com/Mapp17/ConferenceBookingSystem_Demos.git>/conference-room-booking-system.git
 * cd conference-room-booking-system


- Review Project Documentation

 * README.md — project overview and context

 * sprint/ directory — sprint planning and execution artefacts

- Understand Repository Structure

/sprint
  ├── sprint-1-planning.md
  ├── sprint-1-dailies.md
  ├── sprint-1-checkpoint.md
  ├── sprint-1-review.md
  ├── sprint-1-retrospective.md
  └── sprint-1-summary.md


- Markdown files for user stories, epics, prioritisation matrices, and definitions of done are maintained separately for clarity and traceability

### What this system is intended to become

The Conference Room Booking System is intended to become a centralized internal platform that enables employees to efficiently book, manage, and monitor conference room usage within an organisation. The system will support availability checks, conflict prevention, recurring meetings, room capacity and equipment requirements, and booking management.

### How documentation  is organised
Documentation for the Conference Room Booking System is organised to reflect an Agile, sprint-based workflow and to support gradual system evolution.

- High-level project documentation is maintained in the root README.md, which explains the purpose, scope, and current maturity of the system.

- Sprint-specific documentation is stored in the sprint/ directory, with each sprint containing planning, execution, review, retrospective, and summary artefacts.

- Process artefacts such as user stories, epics, prioritisation matrices, and definitions of done are written as standalone markdown files.


### Where to find key project artefacts
- [sprint-1/]()Sprint documentation is located in the sprint-1/ directory. This includes sprint planning records, daily standups, checkpoints, reviews, retrospectives, and summaries.

- [Project Overview]() Project overview and context can be found in the README.md file at the root of the repository.

- Process-related artefacts, such as user stories, epics, prioritisation matrices, and definitions of done, are documented as markdown files created during Scrum simulations on a differnt repository.

- Version control and collaboration rules are defined through Git history, branches, and Pull Requests.

- Future technical artefacts, including API specifications and setup instructions, will be added in later modules as the system moves from documentation to implementation.

### Required Tools:
 #### Operating system
- Windows/Mac/Ubuntu

- Git (latest stable version)
- A GitHub account
- Markdown editor (VS Code recommended)
- .NET and React.


---
## System Context
- A centralized program called the Conference Room Booking System was created to oversee shared meeting areas inside a company. 
- It ensures that reservations are precise, conflict-free, and traceable by serving as a middleman between users and organizational resources.

The System Context at high level consists of:
- User Interface
 * for All users: employees, administrators, and facility 
 managers.
 * View room availability.
 * Create, update, or cancel bookings.
- Booking management component
 * This component handles the business logic.
 * Handles booking creation and validation.
 * Deals with conflict prevention.
- Room management component
 * Stores conference room details (capacity, equipment)
 * Maintainance room schedule.

At this stage, the system is documented through:
- Sprint planning artefacts

Implementation details will be added in later modules


## Explanation of Key Folders and Markdown Artefacts

The repository is organised to clearly separate project context, process documentation, and sprint execution artefacts.

 ### Root directory

* README.md – Provides a high-level overview of the project, its purpose, scope, and current maturity.

* .gitignore – Defines files and folders excluded from version control.

* LICENSE – Specifies the licensing terms for the project.

### sprint/ folder

* Contains all Scrum-related artefacts created during sprint-1.

* Includes planning documents (sprint-1-planning.md), daily standups (sprint-1-dailies.md), mid-sprint checkpoints, sprint reviews, retrospectives, and summaries.

* Each sprint is documented separately to reflect real Agile execution and traceability.

### Process documentation (markdown files)

* User stories, epics, prioritisation matrices, and definitions of done are maintained as markdown files to ensure clarity, version control, and easy review.

* These artefacts support backlog management, sprint planning, and acceptance criteria.



## Project Documentation
This repository contains sprint documentation created during Scrum Simulations:
- `sprint-1\`- Sprint planning, execution and review artefacts

## Upcoming Documentation (Placeholders)

- API Documentation — endpoints for CRUD operations, report downloads, authentication

- Architecture Diagrams — system context, components, and data flow

- Developer Setup Guide — instructions for running the system locally or in Docker

- Testing & CI/CD — unit tests, integration tests, automated pipelines


## LICENCE
This project is licensed under the MIT [LICENSE](LICENSE).

---
✍️ Author
Masoka Andile Mohono: masokaandile17@gmail.com
Created as part of Software Development Trainee Program.
