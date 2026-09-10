# 📱 CampusNews – Android Campus Updates Application

> A Kotlin-based Android application designed to provide students with important campus updates through Academic, Events, and Placement categories.

---

## 📌 Project Overview

**CampusNews** is an Android application developed to provide students with important and regularly updated campus information in a simple and user-friendly interface.

The application uses **Activities, Fragments, Views, Intents, and Notifications** to demonstrate important Android development concepts.

Students can select different news categories such as:

- 📚 Academic
- 🎉 Events
- 💼 Placements

Each category displays relevant campus updates using a **Fragment** instead of creating a separate Activity for every category.

When the user selects **Read More**, the application opens an **Article Activity** using an Intent and displays the complete article. A notification containing the selected article title is also generated.

---

# 🎯 Problem Statement

A college wants to develop an Android application called **CampusNews** to provide students with important campus updates.

### The Home Activity should contain:

- College Logo
- Application Title
- Welcome Message
- Three Category Buttons:
  - Academic
  - Events
  - Placements

When a category is selected, the corresponding content should be displayed using a **Fragment** instead of creating a separate Activity for each category.

### The Fragment should contain:

- Category Title
- News/Update Image
- Short Description
- Read More Button

When **Read More** is selected, an **Article Activity** should be opened using an **Intent**.

### The Article Activity should:

- Display the complete article
- Provide a Back button

When an article is opened, the application should generate a **Notification containing the selected article title**.

---

# 🎯 Aim

To develop a **CampusNews Android application using Kotlin** that demonstrates the use of:

- Activities
- Fragments
- Views
- Intents
- Notifications
- XML layouts
- Event handling

for displaying and managing campus news and updates.

---

# ✨ Features

## 🏠 Home Screen

The Home Activity provides:

- College logo
- CampusNews application title
- Welcome message
- Category navigation buttons
- Dynamic Fragment container

---

## 📚 Academic News

Displays academic-related information such as:

- Examination updates
- Semester registration
- Academic announcements
- Important notices

The user can select **Read More** to view the complete article.

---

## 🎉 Campus Events

Displays information about:

- College fests
- Cultural events
- Technical events
- Sports activities
- Workshops

---

## 💼 Placement News

Displays information about:

- Campus placement drives
- Recruitment opportunities
- Company visits
- Placement announcements
- Student eligibility information

---

## 📖 Read More

The **Read More** button opens the complete article.

Navigation is performed using an **Explicit Intent**.

Article information is passed from the Fragment to the Article Activity.

---

## 🔔 Notifications

Whenever an article is opened, the application generates a notification containing the selected article title.

Example:

```text
CampusNews

Campus Placement Drive

You opened: Campus Placement Drive

## 🛠️ Technologies Used

| Technology | Purpose |
|---|---|
| Kotlin | Android application development |
| Android Studio | Development environment |
| XML | User Interface design |
| Android SDK | Android application development |
| Activities | Screen navigation |
| Fragments | Category-wise content |
| Views | User Interface components |
| Intent | Navigation and data transfer |
| Notifications | Article notifications |
| Git | Version control |
| GitHub | Project repository |

---
## PROJECT STRUCTURE
CampusNews
│
├── app
│   │
│   ├── manifests
│   │   └── AndroidManifest.xml
│   │
│   ├── kotlin+java
│   │   │
│   │   ├── com.example.campusnews
│   │   │   │
│   │   │   ├── AcademicFragment
│   │   │   ├── ArticleActivity
│   │   │   ├── EventFragment.kt
│   │   │   ├── MainActivity
│   │   │   └── PlacementFragment.kt
│   │   │
│   │   ├── com.example.campusnews (androidTest)
│   │   │
│   │   └── com.example.campusnews (test)
│   │
│   ├── res
│   │   │
│   │   ├── drawable
│   │   │
│   │   ├── layout
│   │   │
│   │   ├── mipmap
│   │   │
│   │   ├── values
│   │   │
│   │   └── xml
│   │
│   └── keepRules
│
├── Gradle Scripts
│
└── README.md
