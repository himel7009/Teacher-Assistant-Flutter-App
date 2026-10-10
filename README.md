# 🎓 Teacher Assistant App — Course & Student Activity Manager

[![Flutter](https://img.shields.io/badge/Flutter-02569B?style=for-the-badge&logo=flutter&logoColor=white)](https://flutter.dev)
[![Dart](https://img.shields.io/badge/Dart-0175C2?style=for-the-badge&logo=dart&logoColor=white)](https://dart.dev)
[![Firebase](https://img.shields.io/badge/Firebase-FFCA28?style=for-the-badge&logo=firebase&logoColor=black)](https://firebase.google.com/)
[![Cloud Firestore](https://img.shields.io/badge/Cloud%20Firestore-FFCA28?style=for-the-badge&logo=firebase&logoColor=black)](https://firebase.google.com/docs/firestore)
[![Platform](https://img.shields.io/badge/Platform-Android%20%7C%20iOS-blue?style=for-the-badge)](https://flutter.dev)

A modern, responsive cross-platform mobile application designed for **Teaching Assistants (TAs)** and educators to seamlessly manage university course schedules, track student activities, log attendance, and synchronize class data in real-time.

Developed as a collaborative final project for **CSC464: Mobile Application Development** at **Independent University, Bangladesh (IUB)**.

---

## 📹 Video Demonstration & Walkthrough

Check out the complete mobile walkthrough and live demo of the app in action:
👉 **[Watch Application Demo on Google Drive](https://drive.google.com/file/d/1G1IcH8gaJnuZxVCczSTRPqU6w17uP8X4/view)**

---

## ✨ Key Features

* 📊 **Smart Dashboard**: Centralized hub presenting quick metrics, upcoming class routines, and quick actions for course operations.
* 📚 **Course Management**: Create, view, update, and manage multiple university courses with section details and metadata.
* 👨‍🎓 **Student Directory & Profiles**: Detailed student records with dynamic enrollment and bottom-sheet editing forms.
* 🕒 **Class Routine & Scheduling**: Weekly routine planner to keep track of class schedules, labs, and office hours.
* 📝 **Attendance Tracking**: Real-time attendance logging with complete historical logs per course and session.
* ☁️ **Cloud Synchronization**: Real-time persistent state powered by **Firebase Core** and **Cloud Firestore**.

---

## 🛠️ Personal Engineering Contributions

* **Firebase Core & Cloud Firestore Integration**: Designed database collections and configured asynchronous data synchronization for real-time reads and writes.
* **Student Record Management Flow**: Implemented `AddStudentSheet` and student validation forms with clean UI feedback.
* **Course Editing & Update UI**: Reworked and streamlined `EditCourseSheet` to ensure seamless state reflection across active courses.
* **Provider State Management**: Contributed to reactive state coordination across courses, routines, and student data streams.

---

## 🏛️ Application Architecture

The codebase follows the **Provider State Management** pattern with clear separation of concerns:

```
lib/
├── firebase_options.dart          # Firebase configuration & initialization
├── main.dart                      # App entry point & multi-provider wiring
├── models/                        # Immutable data models
│   ├── attendance_model.dart      # Attendance schemas
│   ├── course_model.dart          # Course information schema
│   ├── routine_model.dart         # Class schedule & timing schema
│   └── student_model.dart         # Student attributes schema
├── providers/                     # State management and Firestore synchronization
│   ├── attendance_provider.dart
│   ├── course_provider.dart
│   ├── routine_provider.dart
│   └── student_provider.dart
├── screens/                       # UI Views
│   ├── attendance/                # Attendance tracking & historical logs
│   ├── courses/                   # Course directory and inspection
│   ├── dashboard/                 # Analytics overview
│   ├── routine/                   # Schedule and calendar timeline
│   ├── students/                  # Student list and details
│   └── main_shell.dart            # Root navigation shell
└── widgets/                       # Reusable bottom sheets and input modals
    ├── add_course_sheet.dart
    ├── add_event_sheet.dart
    ├── add_student_sheet.dart
    ├── edit_course_sheet.dart
    └── edit_student_sheet.dart
```

---

## 🚀 Getting Started

### Prerequisites
* Flutter SDK (3.x or later)
* Android Studio / VS Code with Flutter extension
* Configured Android or iOS emulator / physical device

### Installation
1. Clone the repository:
   ```bash
   git clone https://github.com/himel7009/Teacher-Assistant-Flutter-App.git
   cd Teacher-Assistant-Flutter-App
   ```
2. Install dependencies:
   ```bash
   flutter pub get
   ```
3. Run the app:
   ```bash
   flutter run
   ```

---

## 👨‍💻 Author & Credits

* **Himel Debnath** — [@himel7009](https://github.com/himel7009) | [Kaggle](https://www.kaggle.com/debnathhimel)
* **Course**: CSC464 Mobile Application Development, Independent University Bangladesh (IUB).
