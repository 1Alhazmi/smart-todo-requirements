> Converted from the submitted Word document for GitHub reading. Student IDs removed; wording, team credits and embedded figures retained. Original pagination and Word formatting are not reproduced.



![Figure from course report](assets/image1.png)

Smart To-Do List Application

Foundations of Software Engineering

SE1201

The team members: 

| [student ID removed] |  | يوسف محمودي |

| --- | --- | --- |

| [student ID removed] |  | عبد الرحمن الحازمي |

| [student ID removed] |  | عيسى كومارا |

Second Semester

1447 – 2026

Table of Contents:

1.1 Problem Definition………………………….. 3

1.2 Supposed Solution………………………….. 4

1.3 Steps Toward Implementing the Solution… 5

Requirements Engineering Table…………………… 6

Expected Outcome……………………………... 10

References………………………………............. 10

1.1 Problem Definition

Daily tasks are a must-have in today’s world, most critically for students and working professionals who do many things at once. This includes responsibilities for assignments, projects, meetings, exams, personal work, and more. For today’s users, simple methods like using pens and paper, notes, or basic note programs on their phones are still the primary methods. However, such methods do not allow for proper organization, prioritization, or monitoring of progress. Therefore, users frequently forget what they need to do, finish work late or lack an understanding of what to do first. The challenge is to maintain attention from task to task. If everyone is working on their own projects as students, we need a reliable system for remembering tasks when we have project deadlines and exams due. When things are not organized, users spend more effort trying to remember the tasks that need doing instead of doing them. Consequently, loss of productivity and stress are increased. Task prioritization does not occur with traditional methods. Users can document tasks but do not know which tasks are more significant. Without focus, users may perform less important tasks, while urgent ones have yet to be accomplished. This lack of clear organization impacts academic and personal performance.

Also, old task management tools do not offer a clear approach to monitor completed tasks. Users cannot easily see the finished and pending duties. This causes confusion and wastes time in handling task inefficiencies. Users might mistakenly do the same task again or forget unfinished tasks. This issue is important since task management belongs to most ordinary activities. Students and workers rely on consistent procedures to accomplish their tasks on time. Incomplete task organization results in missed deadlines, decreased work performance, and undue anxiety. A straightforward and methodical system for task management will improve productivity and reduce confusion.

Project Objectives 

To directly address these issues, this project aims to achieve the following explicit goals:

Improve task prioritization so users automatically know what to focus on first.

Lower the rate of missed deadlines through intelligent tracking and alerts.

Make task tracking easier, reducing the mental effort required to organize daily schedules.

Scope Boundaries 

To ensure the project remains achievable and focused, the scope is strictly defined as follows:

In-Scope: Individual user task management, AI-assisted OCR for text extraction from images, automated AI priority prediction, daily focus plan generation, and smart deadline reminders.

Out-of-Scope: Multi-user collaborative workspaces, enterprise-level project management, team task assignment, and complex cross-account cloud syncing.

1.2 Supposed Solution

The project aims to design and implement a Smart To-Do List application that allows users to efficiently organize and track their tasks from the beginning of the day to the end. Users can easily create, edit, delete, assign a priority, and mark tasks as completed. The system will be designed strictly for individual single-user task management to ensure a streamlined and focused MVP (Minimum Viable Product).

Comparison with Existing Tools To demonstrate novelty, our application addresses the gaps left by current market offerings:

Versus Basic Note Apps (e.g., Apple Notes, physical planners): While traditional notes leave tasks as unstructured text, our app uses OCR and NLP to automatically extract, structure, and categorize tasks from physical handwriting or images.

Versus Complex Project Tools (e.g., Jira, Asana): Enterprise tools are often too heavy and require tedious manual configuration. Our solution utilizes an AI-driven Daily Focus Plan Generator that automatically timeboxes and prioritizes tasks, requiring minimal manual setup from the user.

To solve the issues mentioned earlier, our application will introduce the following key features:

Structure from Unstructured (OCR + NLP): Traditional methods like pen and paper do not provide enough structure for organizing tasks. Our AI solution will use OCR (Optical Character Recognition) to turn images or scanned notebook pages into text you can edit and copy. Then, NLP (Natural Language Processing) will enable the application to understand this text and convert it into structured, editable task lists (e.g., using Azure AI Document Intelligence).

Priority Prediction: Because it is hard to prioritize tasks manually, a smart model will rank tasks (High/Medium/Low) using deadlines, impact, estimated effort, and dependencies, while still allowing manual override by the user.

Daily Focus Plan Generator: To prevent time wasted on remembering tasks, the AI will summarize open tasks and generate a 1-day execution plan, highlighting the top 3 tasks with timeboxing and expected durations.

Smart Reminders and Duplication Prevention: To ensure users do not forget tasks or complete them late, the app will feature smart notifications to alert users before deadlines. It will also prevent task duplication and highlight pending tasks that require attention.

Calm and User-Friendly Interface: Existing task management tools are often too complicated. We will design a system specifically tailored for individual users, providing a calm, clean, and user-friendly interface to reduce mental load and lower stress levels without unnecessary complicated features.

1.3 Steps Toward Implementing the Solution

Methodology We will use the Agile methodology, specifically the Scrum framework. This is the most suitable choice for our project because it allows us to build the application in short steps (called sprints). This way, we can test features early and make changes easily.

Stages We will divide our work into four main phases:

Requirements and Design: We will design simple, clean, and stress-free user interfaces using Figma.

Development: First, we will build the basic features (add, edit, and delete tasks). Second, we will add smart AI features like OCR and NLP.

Testing: We will test the application to make sure the AI predicts priorities correctly and the smart reminders work on time.

Deployment: We will prepare the final version of the application for users.

Resources To build this project, we will use the following tools and technologies:

Design Tool: Figma for UI/UX design.

Frontend (User Interface): React Native to build a mobile application for Android and iOS.

Backend & AI: Python to run the AI models (like NLP and Priority Prediction).

Cloud Services: Azure AI for reading documents (OCR) and Firebase for saving data.

Challenges & Risks We might face some challenges during the project:

Risk 1: The AI (OCR) might not read handwriting 100% correctly.

Solution: We will allow users to easily edit the text manually after scanning.

Risk 2: We have many features, and time is limited.

Solution: We will strictly focus on building the most important features first (MVP) for individual users, deliberately leaving out multi-user capabilities.

Requirements Engineering Table

| Student name | Requirement type | Requirement description | Reviewer name | Reviewer remarks |

| --- | --- | --- | --- | --- |

| Youssef Mahmoudi | Functional | The system shall allow users to upload an image or scan a notebook page to extract text using OCR. | Abdulrahman Al-Hazmi | Clear and precise functional requirement that directly addresses our "Structure from Unstructured" goal. |

| Youssef Mahmoudi | Functional | The system shall convert extracted text into structured, editable task items using Natural Language Processing (NLP). | Abdulrahman Al-Hazmi | Good requirement. It clearly defines the system's role after the OCR process. |

| Youssef Mahmoudi | Functional | The system shall allow users to manually edit, delete, or add task details after the OCR extraction process. | Abdulrahman Al-Hazmi | Important inclusion to handle OCR inaccuracies as discussed in our risk management plan. |

| Youssef Mahmoudi | Non-Functional | The OCR extraction process shall complete and display the extracted text within 5 seconds of image upload. | Abdulrahman Al-Hazmi /  | Excellent use of a measurable metric for performance. |

| Youssef Mahmoudi | Non-Functional | The application interface shall maintain an availability rate of 99.9% during any given month. | Abdulrahman Al-Hazmi | Solid reliability requirement that aligns with standard system expectations. |

| Abdulrahman Al-Hazmi | Functional | The system shall automatically rank uncompleted tasks as High, Medium, or Low priority based on deadlines and estimated effort. | Issa Camara | Well-defined behavior for the priority prediction model. |

| Abdulrahman Al-Hazmi | Functional | The system shall generate a 1-day execution plan highlighting the top 3 priority tasks for the user. | Issa Camara | Very clear and directly supports the "Daily Focus Plan Generator" feature. |

| Abdulrahman Al-Hazmi | Functional | The system shall allow users to manually override the AI-generated priority level of any specific task. | Issa Camara | Good catch. Giving the user control over the AI is essential for a good experience. |

| Abdulrahman Al-Hazmi | Non-Functional | The daily focus plan generator shall process and display the execution plan in under 3 seconds after the user requests it. | Issa Camara | Clear performance metric. We must ensure the backend AI processing is optimized to meet this. |

| Abdulrahman Al-Hazmi | Non-Functional | The application shall be compatible and fully functional on both Android (version 10.0 and above) and iOS (version 14.0 and above) devices. | Issa Camara | Great operational constraint that defines our target mobile platforms clearly. |

| Issa Camara | Functional | The system shall send a push notification to the user for pending tasks at least 2 hours before their set deadline. | Youssef Mahmoudi | Accurately describes the smart reminder functionality. |

| Issa Camara | Functional | The system shall detect exact duplicate task entries and prompt the user with a warning before saving. | Youssef Mahmoudi | Very useful requirement for preventing user errors and keeping the list clean. |

| Issa Camara | Functional | The system shall allow users to mark tasks as completed, automatically moving them to a dedicated "Finished Tasks" view. | Youssef Mahmoudi | Clear functional behavior for task tracking and status updates. |

| Issa Camara | Non-Functional | Push notifications shall be delivered to the user's device within 1 minute of the scheduled trigger time. | Youssef Mahmoudi | Measurable and realistic performance metric for the notification system. |

| Issa Camara | Non-Functional | The application's local database shall store up to 5,000 tasks without degrading search query response times beyond 2 seconds. | Youssef Mahmoudi | Excellent capacity and performance constraint to ensure the app remains fast as data grows. |

Expected Outcome 

At the end of this project, we will deliver a working prototype of the Smart To-Do List application. It will successfully read tasks from images, organize them automatically using AI, and have a calm, easy-to-use interface tailored for individual task management. We will also deliver the final project report.

References

Baumeister, R. F., & Masicampo, E. J. (2011). Consider it done! Plan making can eliminate the cognitive effects of unfulfilled goals. Journal of Personality and Social Psychology, 101(4), 667–683. https://doi.org/10.1037/a0024192

Microsoft. (2023). What is Azure AI Document Intelligence? Microsoft Learn. https://learn.microsoft.com/en-us/azure/ai-services/document-intelligence/overview

Schwaber, K., & Sutherland, J. (2020). The Scrum Guide: The definitive guide to Scrum: The rules of the game. Scrum.org. https://scrumguides.org/scrum-guide.html
