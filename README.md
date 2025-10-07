📈💪 FitNexx Android Application ⚡📱

⚙️ Built With
Technology	Description

	Android SDK

	Primary Language

	Authentication & Cloud Sync

	Backend Storage

	Local Data Persistence

	Build Tool

	CI/CD Automation
🏫 Module & Institution Details

Module: Programming 3D [PROG7314]
Assessment Type: PoE Part 2 – App Prototype Development
Institution: IIE Varsity College, Westville

📁 Repositories & Resources:

🧠 FitNexx Android App Repository

☁️ FitNexx API Repository

📦 FitNexx APK Repository

🎥 Video Demonstration (OneDrive)

📑 Table of Contents

✨ Introduction

🎯 Purpose

🎨 Design Decisions

🤖 GitHub Actions

💻 Setup & Usage

✅ Requirements & Features

⚙️ Functionality

🖼️ Image Assets

🏗️ Architecture

👥 Authors & Contributors

⚖️ License

❓ FAQ

📚 References

✨ 1. Introduction

FitNexx is an advanced fitness tracking Android app developed using Kotlin and Android Studio.
It enables users to take control of their fitness journey through real-time analytics, intelligent insights, and goal tracking.

FitNexx provides a seamless hybrid experience using RoomDB for offline functionality and Firebase + MongoDB for cloud synchronization.

💬 Train. Track. Transform — the next version of you, powered by data.

🎯 2. Purpose

The goal of FitNexx is to make personal fitness intuitive, trackable, and motivating through gamification, visual analytics, and progress tracking.

Core Objectives

🔐 Firebase Authentication (Login & Registration)

🧍 Daily activity tracking (steps, calories, hydration)

🎯 Goal creation and progress tracking

🏆 Gamified streaks, achievements, and leaderboards

☁️ MongoDB backend for real-time updates

📈 Progress insights with MPAndroidChart graphs

🌓 Dark/Light mode support

🎨 3. Design Decisions
Category	Decision
UI	Minimal, motivational layout (blue/white/black palette)
UX	Smooth transitions, easy onboarding, error feedback
Gamification	Rewards, streaks, and progress badges
Storage	RoomDB (local) + MongoDB (cloud)
Data Visualization	Interactive bar, line, and pie charts
Notifications	Personalized reminders and motivational quotes

✨ Designed for clarity, performance, and motivation.

🤖 4. GitHub Actions
name: Android Build

on:
  push:
    branches: [ main ]
  pull_request:
    branches: [ main ]

jobs:
  build:
    runs-on: ubuntu-latest
    steps:
      - name: Checkout Repository
        uses: actions/checkout@v3

      - name: Set up JDK 17
        uses: actions/setup-java@v3
        with:
          distribution: 'temurin'
          java-version: '17'

      - name: Give Gradle Permission
        run: chmod +x ./gradlew

      - name: Build Debug APK
        run: ./gradlew assembleDebug

💻 5. Setting Up the Project Locally & Usage
Prerequisites

🧩 Android Studio Arctic Fox or newer

☕ JDK 17+

💜 Kotlin 1.8+

⚙️ Gradle 8.0+

📱 Android 7.0 (API 24)+

🌐 Internet connection (for Firebase features)

Installation Steps

Clone the repository

git clone https://github.com/yourusername/FitNexx.git


Open the project in Android Studio

Sync Gradle

Add your Firebase google-services.json file (if using Firebase)

Click Run ▶️

✅ 6. Requirements and Features
Type	Description
Non-Functional	Scalable, responsive, user-friendly UI
Functional	Firebase Auth, RoomDB, Graphs, Goal Tracking
Extra Features	Dark Mode, PDF Export, Achievements, Insights
⚙️ 7. Functionality

➕ Add / Edit / Delete fitness entries

📊 View analytics (line and bar charts)

📅 Track daily and weekly goals

🧠 Smart recommendations

📄 Export progress as PDF

🌓 Toggle between dark/light modes

☁️ Cloud sync (Firebase + MongoDB)

🖼️ 8. Image Assets

Screenshots showcasing dashboard, analytics, and user interface will be displayed here once finalized.

🏗️ 9. Architecture
FitNexx/
│
├── api/              → REST API (Node.js / Express)
├── app/              → Android App Source
│   ├── data/         → RoomDB entities + repositories
│   ├── ui/           → Activities / Fragments
│   ├── viewmodel/    → MVVM logic
│   └── utils/        → Helper utilities
└── firebase/         → Firebase Authentication & Storage

👥 10. Authors & Contributors
Name	Role	Email
Nikhile Reddy	Lead Developer & Designer	nikhilereddy@gmail.com
⚖️ 11. License

This project is licensed under the MIT License.
You are free to use, modify, and distribute it with proper credit.

❓ 12. FAQ
Question	Answer
Can I log in?	Yes, via Firebase Authentication.
Does it work offline?	Yes, with RoomDB local storage.
Can I view progress visually?	Yes, via MPAndroidChart graphs.
Will there be cloud sync?	Yes, through MongoDB and Firebase.
📚 13. References

Android Developers – Official Documentation

Firebase Authentication

MPAndroidChart GitHub

MongoDB Atlas

Kotlin Language Docs

GitHub Actions Docs

💙 "Train. Track. Transform."

FitNexx — Because the Next You Starts Now.

✅ Ready to Copy:
Save this as README.md in your FitNexx repository.
Then run in Git Bash:

git add README.md
git commit -m "Added fully formatted README for FitNexx"
git push origin main

the rest api log not showing, and also tekl me where to put the image assets 
