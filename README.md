# Smart To-Do List Requirements Project

A team software engineering project for Foundations of Software Engineering (SE1201), second semester 1447 / 2026, at Umm Al-Qura University. It documents the problem, proposed solution, requirements and models for a task-management application.

## Repository status

This repository currently publishes the project overview. The supporting files described below are prepared locally but have not yet been uploaded to GitHub. File paths describe that prepared package; they are not download links.

## Prepared project materials

- Project report — `docs/project-report.md`
- Functional requirements and peer reviews — `docs/functional-requirements.md`
- Non-functional requirements and peer reviews — `docs/non-functional-requirements.md`
- Priority-prediction context diagram — `diagrams/context-diagram-1.png`
- Daily-plan context diagram — `diagrams/context-diagram-2.png`
- Priority-ranking use case — `diagrams/use-case-diagram-1.png`
- Daily-plan use case — `diagrams/use-case-diagram-2.png`

## Scope

Requirements cover task creation, editing, deletion, priorities, deadlines, reminders and completion tracking. Models explore AI-assisted priority prediction and daily focus plans. These are proposed capabilities, not evidence of a deployed application or trained AI model.

## Problem and proposed workflow

The report addresses missed deadlines and the effort of organizing tasks from notes. The proposed user flow is: capture or enter tasks → correct extracted text → assign or predict priorities → generate a daily focus plan → receive reminders → mark completed tasks.

Optical character recognition (OCR) means reading text from an image. Natural language processing (NLP) means interpreting that text to identify task information. Both are proposed parts of the design.

## Design decisions

The scope is individual task management. Team workspaces, task assignment across users and complex account synchronization are excluded. The report proposes React Native for mobile screens, Python for AI processing, Azure AI for document reading, Firebase for storage and Figma for interface design. These are planned tools; a working implementation was not found.

The requirements distinguish functional behavior (what the system should do) from non-functional constraints (how well it should work). Context diagrams show the system boundary and external interactions. Use-case diagrams show user goals and supported actions. Peer-review tables record who wrote and reviewed requirements.

## Team and contribution

The report lists Yousef Mahmoudi, Abdulrahman Alhazmi and Issa Komara. Requirements tables preserve author/reviewer attribution. Abdulrahman’s listed functional requirements address priorities, deadlines and notifications; his non-functional entries address authentication/access control and secure data storage.

## Verification and limitations

Documents and diagrams were inspected. No running application was found with this submission. The latest-looking report with a requirements table was selected by content; the located files do not conclusively establish which report was ultimately submitted. Original page-number references may not correspond to Markdown layout.

## Publication

Academic portfolio documentation. Team credits are retained. No license has been selected.
