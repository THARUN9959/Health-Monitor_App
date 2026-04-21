# 🫀 Health Monitor
Health-Monitor APK

> A real-time Android health & safety app that monitors vital signs, detects critical conditions, and triggers cascading emergency workflows — all running silently in the background.

## 📲 Download APK

> Ready to try the app? Download the latest debug build directly:

**⬇️ Download Health-Monitor App.apk (releases/Health-Monitor%20App.apk)**

> Requires Android 8.0 (API 26) or higher. Enable **"Install from unknown sources"** in your device settings before installing.

---

## ✨ Features

| Feature | Description |
|---|---|
| 💓 **Vital Signs Monitoring** | Real-time heart rate, oxygen saturation (SpO2), and sleep tracking |
| 🔗 **Health Connect Integration** | Reads data from wearables and health apps via Android Health Connect |
| 🔕 **Background Monitoring** | Runs silently with exact AlarmManager scheduling + WorkManager fallback |
| ⚠️ **Critical Condition Detection** | Threshold-based detection with cooldown and stale-reading validation |
| 🚨 **Cascading Emergency System** | Auto-triggers SMS → Phone Call → Personal Safety alerts with location |
| 💊 **Medication Management** | Track medications, set reminders, and get refill notifications |
| 🔐 **Security & Privacy** | onboarding flow, encrypted Room database (SQLCipher) |
| 📍 **Live Location Sharing** | Shares GPS location during emergency events |

---


## 🛠️ Tech Stack

- **Language**: Kotlin
- **UI**: Jetpack Compose + Material 3
- **Navigation**: Navigation Compose
- **Database**: Room + SQLCipher (encrypted)
- **Background Work**: WorkManager + AlarmManager
- **Health Data**: Android Health Connect Client
- **Location**: Google Play Services — FusedLocationProviderClient
- **Build**: Gradle with KSP (Kotlin Symbol Processing)

---

## 📋 Requirements

- **Physical Android device** recommended for:
  - Health Connect data (wearable integration)
  - SMS / Phone / Location permission testing
  - Background & foreground monitoring behavior


| Component | Version |
|---|---|
| AGP | 9.1.0 |
| Kotlin | 2.2.10 |
| KSP | 2.3.2 |
| Java / Kotlin Target | 11 |
| App Version | 1.0 (versionCode 1) |

---

## 🚀 Getting Started

### First Launch

- Complete the **onboarding flow** and grant all requested permissions
- Connect a **Health Connect** compatible device or app as a data source
- Enable **background monitoring** from the Settings screen


## 🔐 Permissions Used

| Permission | Purpose |
|---|---|
| `READ_HEART_RATE`, `READ_OXYGEN_SATURATION`, `READ_SLEEP_SESSION` | Health Connect vital signs |
| `health.READ_HEALTH_DATA_IN_BACKGROUND` | Background Health Connect reads |
| `ACCESS_FINE_LOCATION`, `ACCESS_BACKGROUND_LOCATION` | Emergency location sharing |
| `SEND_SMS` | Emergency SMS alerts |
| `CALL_PHONE` | Emergency call functionality |
| `POST_NOTIFICATIONS` | Monitoring and emergency notifications (Android 13+) |
| `FOREGROUND_SERVICE`, `FOREGROUND_SERVICE_HEALTH` | Background monitoring service |
| `BODY_SENSORS`, `ACTIVITY_RECOGNITION` | Sensor and activity data |
| `RECEIVE_BOOT_COMPLETED` | Restart monitoring after device reboot |



## 🙋‍♂️ Author

**THARUN9959**  
GitHub: [@THARUN9959](https://github.com/THARUN9959)
