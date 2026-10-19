<div align="center">

# ⚡ StreakMaster
### *Zero-Tolerance Habit & Discipline Tracker for Android & Windows*

StreakMaster is a strict, cross-platform habit tracking application built with pure web technologies and packaged into native Android and Windows executables. Designed for absolute consistency: miss even a single habit, and your streak resets.

<br/>

[![Download Android APK](https://img.shields.io/badge/📥_Download-Android_APK-059669?style=for-the-badge&logo=android&logoColor=white)](../../releases/latest/download/app-debug.apk)
[![Download Windows PC](https://img.shields.io/badge/💻_Download-Windows_PC_(ZIP)-4f46e5?style=for-the-badge&logo=windows&logoColor=white)](../../releases/latest/download/HabitMaster-Windows-PC.zip)

<br/>

[![Latest Release](https://img.shields.io/github/v/release/shauryanshjha127-dev/Habit-Tracker-App?style=flat-square&color=indigo)](../../releases/latest)
[![Build Pipelines](https://img.shields.io/badge/CI%2FCD-GitHub_Actions-2088FF?style=flat-square&logo=githubactions&logoColor=white)](../../actions)
[![License: MIT](https://img.shields.io/badge/License-MIT-emerald?style=flat-square)](LICENSE)

</div>

---

## 📥 Direct Downloads

Download the latest pre-compiled binaries directly from our [Releases page](../../releases/latest):

* 📱 **[Android APK (`app-debug.apk`)](../../releases/latest/download/app-debug.apk)**  
  Download directly to your Android device, enable *"Install unknown apps"* if prompted, and install.
* 💻 **[Windows Executable (`HabitMaster-Windows-PC.zip`)](../../releases/latest/download/HabitMaster-Windows-PC.zip)**  
  Extract the ZIP archive and run `Habit & Streak Master.exe`. No additional setup required.

---

## ⚡ Core Features

- **Strict Zero-Tolerance Streaks**: Streaks only advance when **100% of your daily habits** are checked off. If a day ends incomplete, the active streak resets to 0.
- **Dynamic Discipline Meter**: Real-time consistency score calculated from your completion rate across the last 7 days.
- **Goal Challenges**: Lock into 7, 14, 21, or 30-day endurance challenges with progress bars and remaining day countdowns.
- **Monthly Visual Calendar**: Dedicated monthly view highlighting all perfect days in emerald green versus missed days.
- **Analytics & History**: Integrated Chart.js weekly bar chart tracking your daily completions.
- **Gamified Progression**: Earn XP with every completed habit, increase your player level, and unlock milestone trophies (*3-Day Spark, 7-Day Titan, 14-Day Iron, 30-Day Master, Century 100*).
- **Habit Management**: Easily add new custom habits or delete existing habits with full history cleanup.
- **Audio Feedback**: Completion chimes powered by Web Audio API and celebratory confetti effects for 100% days.
- **100% Offline & Private**: Zero accounts, zero analytics, zero external backend. All state persists securely in your device's `localStorage`.

---

## 📱 App Pages & Navigation

| Screen | Functionality |
| :--- | :--- |
| **Today** | Daily checklist, live streak count, discipline score, and habit addition/deletion. |
| **Goals** | Active duration challenge countdown, completion progress, and strict rules. |
| **Calendar** | Monthly performance grid mapping perfect days and consistency trends. |
| **Stats** | 7-day completion bar chart, player level, and milestone badges. |

---

## 🛠️ Tech Stack & Architecture

- **Frontend Core**: HTML5, Tailwind CSS, Modern JavaScript (ES6+)
- **Visuals & Charts**: [Chart.js](https://www.chartjs.org/), [FontAwesome 6](https://fontawesome.com/), [Canvas-Confetti](https://github.com/catdad/canvas-confetti)
- **Android Runtime**: [Capacitor 6](https://capacitorjs.com/)
- **Desktop Runtime**: [Electron 29](https://www.electronjs.org/)
- **Automated CI/CD**: GitHub Actions (Ubuntu and Windows runner pipelines)

---

## 📂 Repository Layout

```text
Habit-Tracker-App/
├── .github/
│   └── workflows/
│       ├── build-apk.yml       # Cloud build for Android APK
│       └── build-pc.yml        # Cloud build for Windows standalone executable
├── capacitor.config.json       # Capacitor configuration
├── index.html                  # Single-file UI, router, and logic engine
├── main.js                     # Electron main process entry point
└── package.json                # App metadata, scripts, and dependencies

# Clone the repository
git clone [https://github.com/shauryanshjha127-dev/Habit-Tracker-App.git](https://github.com/shauryanshjha127-dev/Habit-Tracker-App.git)
cd Habit-Tracker-App

# Install dependencies
npm install

# Run desktop version locally
npm start
