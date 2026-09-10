# 📱 CampusNews – Android Campus Updates Application

<p align="center">

  <img src="https://img.shields.io/badge/Platform-Android-green?style=for-the-badge&logo=android" alt="Android">

  <img src="https://img.shields.io/badge/Language-Kotlin-purple?style=for-the-badge&logo=kotlin" alt="Kotlin">

  <img src="https://img.shields.io/badge/UI-XML-blue?style=for-the-badge&logo=android" alt="XML">

  <img src="https://img.shields.io/badge/IDE-Android%20Studio-orange?style=for-the-badge&logo=androidstudio" alt="Android Studio">

  <img src="https://img.shields.io/badge/License-Educational-lightgrey?style=for-the-badge" alt="License">

</p>

<p align="center">
  <b>A Kotlin-based Android application for delivering important campus updates through Academic, Events, and Placement categories.</b>
</p>

---

## 📌 Project Overview

**CampusNews** is an Android application developed using **Kotlin and XML** to provide students with important and regularly updated campus information through a simple, organized, and user-friendly interface.

The application demonstrates several important Android development concepts, including:

* Activities
* Fragments
* Views
* XML layouts
* Explicit Intents
* Data passing between screens
* Click event handling
* Notifications
* Notification Channels
* Activity navigation
* Fragment-based UI

Instead of creating a separate Activity for every news category, **CampusNews uses reusable Fragments** to display category-specific content.

The application contains three primary categories:

| Category      | Purpose                                         |
| ------------- | ----------------------------------------------- |
| 📚 Academic   | Academic announcements and examination updates  |
| 🎉 Events     | College events, workshops, fests and activities |
| 💼 Placements | Placement drives and recruitment opportunities  |

When the user selects **Read More**, the selected article is opened in a separate **ArticleActivity** using an Explicit Intent. At the same time, a notification containing the selected article title is generated.

---

# 🎯 Problem Statement

A college wants to develop an Android application called **CampusNews** to provide students with important campus updates in one centralized application.

The application should provide:

### Home Activity

The Home Activity should contain:

* 🏫 College Logo
* 📱 Application Title
* 👋 Welcome Message
* 📚 Academic Button
* 🎉 Events Button
* 💼 Placements Button
* 📦 Fragment Container

### Category Fragment

Each category Fragment should contain:

* Category Title
* News/Update Image
* Short Description
* Read More Button

### Article Activity

When **Read More** is selected:

* An Article Activity should open.
* Complete article information should be displayed.
* Article data should be passed using an Explicit Intent.
* A Back button should be available.
* A notification containing the selected article title should be generated.

---

# 🎯 Aim

To develop a **CampusNews Android application using Kotlin** that demonstrates the implementation and integration of:

> **Activities + Fragments + Views + Intents + Notifications + XML Layouts + Event Handling**

for managing and displaying campus news and updates.

---

# ✨ Key Features

## 🏠 1. Home Screen

The Home Screen acts as the central navigation area of the application.

It provides:

* College branding
* CampusNews title
* Welcome message
* Category navigation
* Dynamic Fragment container

---

## 📚 2. Academic Updates

The Academic section displays academic-related information such as:

* Examination announcements
* Semester registration
* Academic notices
* Important deadlines
* University-related updates

Students can select **Read More** to view the complete article.

---

## 🎉 3. Campus Events

The Events section provides information about:

* College fests
* Cultural programs
* Technical events
* Sports activities
* Workshops
* Student activities

---

## 💼 4. Placement Updates

The Placement section provides information related to:

* Campus placement drives
* Recruitment opportunities
* Company visits
* Placement announcements
* Eligibility information
* Recruitment activities

---

## 📖 5. Read More Functionality

Each news category provides a **Read More** button.

When selected:

```text
Fragment
   ↓
Read More
   ↓
Explicit Intent
   ↓
ArticleActivity
   ↓
Complete Article
```

Article information is transferred from the Fragment to `ArticleActivity` using **Intent Extras**.

---

## 🔔 6. Notification System

Whenever a user opens an article, the application generates a notification.

Example:

```text
CampusNews

Campus Placement Drive

You opened: Campus Placement Drive
```

The notification functionality demonstrates:

* Notification Channel
* Notification Builder
* Notification Manager
* Notification permission handling

---

## ◀️ 7. Back Navigation

The Article Activity contains a Back button that allows the user to return to the previous screen.

```text
ArticleActivity
       ↓
   Back Button
       ↓
  Previous Screen
```

---

# 🛠️ Technologies & Tools

| Technology         | Purpose                         |
| ------------------ | ------------------------------- |
| **Kotlin**         | Android application development |
| **Android Studio** | Development environment         |
| **Android SDK**    | Android application framework   |
| **XML**            | User interface design           |
| **Activities**     | Screen-level navigation         |
| **Fragments**      | Reusable category-based UI      |
| **Views**          | UI components                   |
| **Intent**         | Navigation and data transfer    |
| **Notifications**  | User notifications              |
| **Git**            | Version control                 |
| **GitHub**         | Source-code hosting             |

---

# 🧩 Android Concepts Demonstrated

This project demonstrates the following Android concepts:

### Activities

Used for:

* `MainActivity`
* `ArticleActivity`

Activities represent major screens of the application.

### Fragments

Used for:

* `AcademicFragment`
* `EventFragment`
* `PlacementFragment`

Fragments allow category content to be displayed without creating separate Activities for each category.

### Views

The project uses common Android UI components such as:

* `TextView`
* `ImageView`
* `Button`
* `ScrollView`
* Layout containers
* Fragment containers

### Explicit Intent

Explicit Intent is used to navigate from a Fragment to `ArticleActivity`.

```text
AcademicFragment
       ↓
    Intent
       ↓
ArticleActivity
```

### Intent Extras

Article information can be transferred using Intent extras.

Conceptually:

```text
Article Title
Article Description
Article Image
Article Content
        ↓
   Intent Extras
        ↓
 ArticleActivity
```

### Notifications

The application demonstrates Android notification functionality through:

```text
Notification Channel
        ↓
Notification Builder
        ↓
Notification Manager
        ↓
User Notification
```

---

# 📂 Project Structure

```text
CampusNews/
│
├── app/
│   │
│   ├── manifests/
│   │   └── AndroidManifest.xml
│   │
│   ├── kotlin+java/
│   │   │
│   │   ├── com.example.campusnews/
│   │   │   │
│   │   │   ├── AcademicFragment.kt
│   │   │   ├── ArticleActivity.kt
│   │   │   ├── EventFragment.kt
│   │   │   ├── MainActivity.kt
│   │   │   └── PlacementFragment.kt
│   │   │
│   │   ├── com.example.campusnews (androidTest)/
│   │   │
│   │   └── com.example.campusnews (test)/
│   │
│   ├── res/
│   │   │
│   │   ├── drawable/
│   │   ├── layout/
│   │   ├── mipmap/
│   │   ├── values/
│   │   └── xml/
│   │
│   └── keepRules/
│
├── Gradle Scripts/
│
└── README.md
```

---

# 🔄 Application Workflow

The overall development workflow can be represented as:

```text
START
  │
  ▼
Create Android Project
  │
  ▼
Select Kotlin
  │
  ▼
Create MainActivity
  │
  ▼
Design Home Screen
  │
  ├── Add College Logo
  ├── Add CampusNews Title
  ├── Add Welcome Message
  └── Add Category Buttons
  │
  ▼
Create Fragments
  │
  ├── AcademicFragment
  ├── EventFragment
  └── PlacementFragment
  │
  ▼
Add News Images
  │
  ▼
Add News Descriptions
  │
  ▼
Add Read More Button
  │
  ▼
Create ArticleActivity
  │
  ▼
Implement Explicit Intent
  │
  ▼
Pass Article Data
  │
  ▼
Display Complete Article
  │
  ▼
Generate Notification
  │
  ▼
Implement Back Button
  │
  ▼
Run & Test Application
  │
  ▼
END
```

---

# 🔀 Application Flow Diagram

```text
                         ┌───────────────────┐
                         │   START APP       │
                         └─────────┬─────────┘
                                   │
                                   ▼
                         ┌───────────────────┐
                         │   MainActivity    │
                         └─────────┬─────────┘
                                   │
                                   ▼
                         ┌───────────────────┐
                         │    Home Screen    │
                         └─────────┬─────────┘
                                   │
             ┌─────────────────────┼─────────────────────┐
             │                     │                     │
             ▼                     ▼                     ▼
      ┌─────────────┐       ┌─────────────┐       ┌─────────────┐
      │  Academic   │       │    Event    │       │  Placement  │
      │   Button    │       │   Button    │       │   Button    │
      └──────┬──────┘       └──────┬──────┘       └──────┬──────┘
             │                     │                     │
             ▼                     ▼                     ▼
      ┌─────────────┐       ┌─────────────┐       ┌─────────────┐
      │  Academic   │       │    Event    │       │  Placement  │
      │  Fragment   │       │  Fragment   │       │  Fragment   │
      └──────┬──────┘       └──────┬──────┘       └──────┬──────┘
             │                     │                     │
             └─────────────────────┼─────────────────────┘
                                   │
                                   ▼
                         ┌───────────────────┐
                         │    Read More      │
                         └─────────┬─────────┘
                                   │
                                   ▼
                         ┌───────────────────┐
                         │ Explicit Intent   │
                         └─────────┬─────────┘
                                   │
                                   ▼
                         ┌───────────────────┐
                         │ ArticleActivity   │
                         └─────────┬─────────┘
                                   │
                      ┌────────────┴────────────┐
                      │                         │
                      ▼                         ▼
              ┌───────────────┐        ┌────────────────┐
              │ Complete      │        │ Notification   │
              │ Article       │        │                │
              └───────┬───────┘        └────────────────┘
                      │
                      ▼
                ┌───────────┐
                │ Back Button│
                └─────┬─────┘
                      │
                      ▼
                ┌───────────┐
                │Home Screen│
                └───────────┘
```

---

# 🔁 User Journey

```text
Open Application
       ↓
View Home Screen
       ↓
Select Category
       ↓
View Category Fragment
       ↓
Read News Summary
       ↓
Click "Read More"
       ↓
ArticleActivity Opens
       ↓
Read Complete Article
       ↓
Notification Generated
       ↓
Click Back
       ↓
Return to Previous Screen
```

---

# 📱 Screenshots

The following screenshots demonstrate the application's user interface and navigation flow.

### 🏠 Home Screen

<img width="360" height="791" alt="CampusNews Home Screen" src="https://github.com/user-attachments/assets/7a5847ca-a413-42f7-a683-a8529a7c83ae" />

---

### 📚 Academic Updates

<img width="357" height="797" alt="Academic Updates" src="https://github.com/user-attachments/assets/90d5afaa-0017-400e-b44a-bce6f4e1204c" />

---

### 🎉 Events

<img width="355" height="787" alt="Campus Events" src="https://github.com/user-attachments/assets/cfbfc536-68da-4fdb-a22f-39cf3c8164da" />

---

### 💼 Placement Updates

<img width="352" height="790" alt="Placement Updates" src="https://github.com/user-attachments/assets/8a55a880-28e7-43b1-a61f-e2c28b19ad70" />

---

### 📖 Article / Notification Flow

<img width="360" height="793" alt="Article Activity" src="https://github.com/user-attachments/assets/cb1f4b36-257e-4954-b625-b0a5caf8b4da" />

---

# ⚙️ How to Run the Project

## 1. Clone the Repository

```bash
git clone https://github.com/your-username/CampusNews.git
```

## 2. Open in Android Studio

Open **Android Studio** and select:

```text
File → Open → CampusNews
```

## 3. Sync Gradle

Allow Android Studio to download and synchronize all required dependencies.

## 4. Connect Device or Emulator

You can use:

* Android Emulator
* Physical Android Device

## 5. Run the Application

Click:

```text
▶ Run
```

The application will launch on the selected Android device or emulator.

---

# 🧪 Testing

The following functionality should be tested:

| Test Case          | Expected Result                |
| ------------------ | ------------------------------ |
| Launch application | Home screen appears            |
| Click Academic     | Academic Fragment opens        |
| Click Events       | Event Fragment opens           |
| Click Placements   | Placement Fragment opens       |
| Click Read More    | ArticleActivity opens          |
| Open article       | Selected article title appears |
| Article opens      | Notification is generated      |
| Click Back         | Previous screen appears        |

---

# 🎓 Learning Outcomes

After completing this project, the following Android development concepts are understood:

### Android Development

* Android Studio
* Android SDK
* Android project structure
* Application resources
* XML layouts

### Kotlin

* Kotlin classes
* Variables
* Functions
* Event handling
* Click listeners

### Activities

* Creating Activities
* Activity lifecycle concepts
* Starting Activities
* Finishing Activities
* Activity navigation

### Fragments

* Creating Fragments
* Fragment lifecycle
* Fragment navigation
* Reusable UI components
* Dynamic content

### Intent

* Explicit Intent
* Activity navigation
* Passing data
* Receiving Intent Extras

### Notifications

* Notification Channel
* Notification Builder
* Notification Manager
* Notification permissions
* Displaying notifications

---

# 🚀 Future Enhancements

The current application can be extended with several real-world features.

### 🔐 User Authentication

Add:

* Student login
* Faculty login
* Admin login

### ☁️ Cloud Database

Connect the application to:

* Firebase Firestore
* Firebase Realtime Database

This would allow administrators to publish updates dynamically.

### 🔎 Search Functionality

Allow students to search for:

```text
Academic
Events
Placements
Announcements
```

### 🔔 Push Notifications

Implement Firebase Cloud Messaging so students can receive real-time campus announcements.

### ❤️ Bookmark Articles

Allow students to save important articles for later reading.

### 🌙 Dark Mode

Add support for:

* Light Mode
* Dark Mode
* System Theme

### 👨‍💼 Admin Panel

Create an admin interface for:

* Adding announcements
* Updating articles
* Managing events
* Managing placement information

### 📊 Analytics

Track:

* Most viewed articles
* Popular categories
* User engagement

---

# 📌 Project Highlights

```text
✔ Kotlin-based Android Application
✔ XML-based User Interface
✔ Activity & Fragment Implementation
✔ Explicit Intent Navigation
✔ Intent Data Passing
✔ Category-based News System
✔ Article Detail Screen
✔ Android Notifications
✔ Notification Channel
✔ Back Navigation
✔ Clean Project Structure
✔ GitHub Ready
```

---

# 🧠 Key Android Architecture Concept

The application follows a simple navigation-based structure:

```text
                 CampusNews
                     │
              ┌──────┴──────┐
              │             │
       MainActivity    ArticleActivity
              │
       ┌──────┼──────┐
       │      │      │
       ▼      ▼      ▼
   Academic Event Placement
   Fragment Fragment Fragment
```

This approach demonstrates how **Fragments can be reused within an Activity**, while separate Activities can be used for major screen-level navigation.

---

# 📋 Expected Output

After successfully running the application, the complete flow should work as follows:

```text
┌───────────────────────┐
│      CampusNews       │
│        START          │
└───────────┬───────────┘
            │
            ▼
┌───────────────────────┐
│     MainActivity      │
└───────────┬───────────┘
            │
     ┌──────┼──────┐
     │      │      │
     ▼      ▼      ▼
 Academic Event Placement
 Fragment Fragment Fragment
     │      │      │
     └──────┼──────┘
            │
            ▼
       Read More
            │
            ▼
         Intent
            │
            ▼
┌───────────────────────┐
│   ArticleActivity     │
└───────────┬───────────┘
            │
       ┌────┴────┐
       │         │
       ▼         ▼
   Complete   Notification
   Article
       │
       ▼
   Back Button
       │
       ▼
 MainActivity
```


