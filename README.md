# ⚽ Football Tracker

<p align="center">
  <strong>Track. Analyze. Improve. Succeed.</strong>
</p>

<p align="center">
  <img src="https://img.shields.io/badge/Platform-Android-green?logo=android" />
  <img src="https://img.shields.io/badge/Language-Kotlin-blue?logo=kotlin" />
  <img src="https://img.shields.io/badge/Firebase-Connected-orange?logo=firebase" />
  <img src="https://img.shields.io/badge/AI-Gemini-purple?logo=google" />
  <img src="https://img.shields.io/badge/Min_SDK-26-brightgreen" />
</p>

---

## 📱 About

**Football Tracker** is a fully-featured native Android app for managing and tracking football players' performance. Built with **Kotlin**, powered by **Firebase**, and enhanced with **Gemini AI** for personalized coaching reports.

---

## ✨ Features

### 👤 Player
- 🥤 Daily water intake tracking with wave animation
- 🍎 Calorie tracking (barcode scanner + USDA search + manual)
- 🏃 Training tracker with animated circular timer
- 🤖 AI Coach Report (Gemini AI) — 300+ word personalized report
- 📊 Interactive analytics with PDF export
- 💪 BMI calculator with dynamic color bar
- 🃏 Professional player card generator (1080×1920)
- 🔄 Automatic daily reset at midnight

### 👨‍💼 Coach
- 🔑 Unique coach code for player recruitment
- 📋 Player management with performance charts
- 🎯 Custom training creation with images/videos
- 💬 Real-time messaging with players

### 🛡️ Admin
- 👥 Full user management (delete, ban, subscriptions)
- 📬 Inbox with conversation status tracking
- 📈 Platform statistics dashboard

---

## 🛠️ Tech Stack

```
Language        → Kotlin
Architecture    → MVVM + Hilt DI
Database        → Cloud Firestore
Auth            → Firebase Authentication
Storage         → Firebase Storage
AI              → Gemini AI (gemini-2.5-flash)
Payments        → Google Play Billing v7
Charts          → MPAndroidChart
Images          → Glide
Barcode         → ZXing
Background      → WorkManager
Network         → Retrofit + OkHttp
```

---

## 📦 External APIs

| API | Purpose |
|-----|---------|
| Gemini REST API | AI coaching reports |
| USDA FoodData Central | Food & calorie database |
| Open Food Facts | Barcode nutritional data |

---

## 🌍 Languages Supported

| Language | Code |
|----------|------|
| Arabic (العربية) | | ar |
| English | en |
| Türkçe (Turkish) | tr |
| Français (French) | fr |
| Español (Spanish) | es |

---

## 🏗️ Architecture

```
com.webiodd.footballtracker/
├── core/
│   ├── base/          # BaseActivity
│   └── utils/         # LanguageManager, PremiumManager, BMICalculator
├── data/
│   ├── remote/        # Firebase, Food APIs, Gemini
│   └── workers/       # DailyResetWorker, HourlyAIWorker, NotificationWorker
├── di/                # Hilt Modules (Firebase, App)
└── presentation/
    ├── auth/          # Login, SignUp, Splash
    ├── player/        # Dashboard, Nutrition, Training, Analytics, Profile
    ├── coach/         # Dashboard, Players, Training, Profile, Chat
    ├── admin/         # Dashboard, Inbox, Settings
    ├── premium/       # Plan Selection, Upgrade, Gate
    └── dialogs/       # BMI, Water, AddMeal, AddTraining, JoinCoach
```

---

## 🔐 Security

- Firebase Security Rules with RBAC (Role-Based Access Control)
- Each user can only access their own data
- Coaches can read their players' data
- Admin has full controlled access

---

## 💎 Subscription Plans

| Feature | Free | Premium |
|---------|------|---------|
| Water tracking | ✅ | ✅ |
| Manual calorie tracking | ✅ | ✅ |
| Training tracking | ✅ | ✅ |
| BMI calculator | ✅ | ✅ |
| Support chat | ✅ | ✅ |
| AI Coach Report | ❌ | ✅ |
| Barcode scanner | ❌ | ✅ |
| Food search | ❌ | ✅ |
| Analytics & PDF | ❌ | ✅ |
| Coach messaging | ❌ | ✅ |
| Player card | ❌ | ✅ |

---

## 👨‍💻 Developer

**Tarik Salih** — WebioDD

---

## 📄 License

This project is proprietary software. All rights reserved.
