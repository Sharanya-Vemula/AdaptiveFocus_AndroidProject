# 📱 Adaptive Focus Engine – Android App

Adaptive Focus Engine is a system-level Android application designed to help students track and improve their study focus by monitoring focus sessions, managing breaks, and analyzing session history — all with an offline-first approach.

This project is built to demonstrate strong Android fundamentals, clean architecture, and real-world engineering practices.

---

## 🚀 Features

- ⏱ Live focus timer (updates every second)
- ▶️ Start / Pause / Resume / Stop focus sessions
- 🔔 Foreground Service for uninterrupted tracking
- 📊 Focus score calculation based on session duration and interruptions
- 💾 Offline storage using Room Database
- 📜 Session history using RecyclerView
- 🧾 Session summary dialog after each session
- 🔔 Toast messages for user feedback
- 🎨 Clean UI using XML & ConstraintLayout

---

## 🧠 Focus Score Logic

The focus score is calculated using a simple rule-based approach:

Focus Score = (Session Duration × 4) − (Interruptions × 5)
Score Range: 0 – 100



This keeps the logic transparent while showcasing problem-solving skills.

---

## 🏗 Architecture

The app follows the **MVVM (Model–View–ViewModel)** architecture pattern.

UI (Activity + XML)
↓
ViewModel (LiveData + viewModelScope)
↓
Repository
↓
Room Database

This ensures separation of concerns and scalability.

---

## 🧩 Tech Stack

- **Language:** Kotlin
- **UI:** XML, ConstraintLayout
- **Architecture:** MVVM
- **Database:** Room
- **Concurrency:** Kotlin Coroutines
- **Lifecycle:** ViewModel, LiveData
- **Background Work:** Foreground Service
- **Build System:** Gradle (Kotlin DSL)
- **Minimum SDK:** 24

---

## 📂 Project Structure

com.example.adaptivefocusengine
│
├── data
│ ├── local
│ │ ├── FocusSession.kt
│ │ ├── FocusDao.kt
│ │ └── FocusDatabase.kt
│ └── repository
│ └── FocusRepository.kt
│
├── service
│ └── FocusTrackingService.kt
│
├── ui
│ ├── MainActivity.kt
│ └── SessionAdapter.kt
│
├── viewmodel
│ └── FocusViewModel.kt
│
├── utils
│ └── FocusScoreCalculator.kt



---

## 🛠 How to Run the Project

1. Clone the repository
   ```bash
   git clone https://github.com/Sharanya-Vemula/AdaptiveFocus_AndroidProject.git
Open the project in Android Studio

Sync Gradle files

Run on an emulator or physical device (Android 7.0+)

## 🎯 Why This Project Stands Out
Not a typical To-Do or clone app

Demonstrates Android lifecycle & background services

Offline-first design using Room

Clean MVVM architecture

Suitable for Android Developer Fresher / Intern roles

## 🔮 Future Enhancements
Real app-usage based distraction detection

Weekly/monthly focus analytics

DiffUtil for RecyclerView optimization

Export session history

Jetpack Compose UI version
