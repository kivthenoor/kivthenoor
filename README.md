<h1 align="center">Hi, I'm Akif 👋</h1>

<p align="center">
  <b>Mobile developer in Malaysia</b> · Android (Kotlin and Java) in production · Flutter, Kotlin Multiplatform,
  SwiftUI and React Native apps of my own, mostly offline-first apps for Malaysian users.
</p>

<p align="center">
  <a href="https://play.google.com/store/apps/details?id=com.thenoor.app"><img src="https://img.shields.io/badge/Now%20at-TheNoor-0E7C66?style=flat-square&logo=googleplay&logoColor=white" alt="Now at TheNoor" /></a>
  <img src="https://img.shields.io/badge/Based%20in-Malaysia-CC0001?style=flat-square" alt="Based in Malaysia" />
  <a href="https://github.com/kivfauzi"><img src="https://img.shields.io/badge/Earlier%20work-%40kivfauzi-24292F?style=flat-square&logo=github&logoColor=white" alt="Earlier work on @kivfauzi" /></a>
</p>

---

### 🧑‍💻 Languages I code in

<p align="center">
  <img src="https://img.shields.io/badge/Kotlin-7F52FF?style=for-the-badge&logo=kotlin&logoColor=white" alt="Kotlin" />
  <img src="https://img.shields.io/badge/Java-ED8B00?style=for-the-badge&logo=openjdk&logoColor=white" alt="Java" />
  <img src="https://img.shields.io/badge/Dart-0175C2?style=for-the-badge&logo=dart&logoColor=white" alt="Dart" />
  <img src="https://img.shields.io/badge/Swift-F05138?style=for-the-badge&logo=swift&logoColor=white" alt="Swift" />
  <img src="https://img.shields.io/badge/TypeScript-3178C6?style=for-the-badge&logo=typescript&logoColor=white" alt="TypeScript" />
</p>

### 📱 Platforms and frameworks

<p align="center">
  <img src="https://img.shields.io/badge/Android-3DDC84?style=for-the-badge&logo=android&logoColor=white" alt="Android" />
  <img src="https://img.shields.io/badge/Jetpack%20Compose-4285F4?style=for-the-badge&logo=jetpackcompose&logoColor=white" alt="Jetpack Compose" />
  <img src="https://img.shields.io/badge/Kotlin%20Multiplatform-7F52FF?style=for-the-badge&logo=kotlin&logoColor=white" alt="Kotlin Multiplatform" />
  <img src="https://img.shields.io/badge/Flutter-02569B?style=for-the-badge&logo=flutter&logoColor=white" alt="Flutter" />
  <img src="https://img.shields.io/badge/SwiftUI-0D96F6?style=for-the-badge&logo=swift&logoColor=white" alt="SwiftUI" />
  <img src="https://img.shields.io/badge/React%20Native-20232A?style=for-the-badge&logo=react&logoColor=white" alt="React Native" />
  <img src="https://img.shields.io/badge/Expo-000020?style=for-the-badge&logo=expo&logoColor=white" alt="Expo" />
</p>

### 🛠 Tools

<p align="center">
  <img src="https://skillicons.dev/icons?i=kotlin,java,dart,flutter,swift,ts,react,androidstudio,gradle,firebase,sqlite,githubactions,git,github,vscode,apple&perline=8" alt="Kotlin, Java, Dart, Flutter, Swift, TypeScript, React, Android Studio, Gradle, Firebase, SQLite, GitHub Actions, Git, GitHub, VS Code, Apple" />
</p>

### 🧭 What I'm working on

**Now:** Android developer on [TheNoor](https://play.google.com/store/apps/details?id=com.thenoor.app), a Muslim
lifestyle and worship app (Quran reading and audio, prayer times and azan alerts, donations and commerce), its car
head-unit app and a Wear OS companion. Main author of the current Android codebase (590+ commits).

Earlier work and most of my TheNoor history (2022–2025) is on my previous account,
[@kivfauzi](https://github.com/kivfauzi).

---

### 📈 Progress

About 940 commits across TheNoor's Android, iOS, car and SDK repos since May 2024, plus 12 personal apps.

| When | Milestone |
|---|---|
| 2022 | First Kotlin Android apps (QuizAppKotlin) on [@kivfauzi](https://github.com/kivfauzi) |
| 2023 | Android UI practice projects (calendar and schedule app UI) |
| Feb 2024 | MarketingApps (Android) |
| May 2024 | Joined TheNoor: Android app (Java), 180+ commits in its first codebase |
| Sep 2024 | TheNoor Car, the in-car head-unit app (MVVM, Hilt, Room) |
| Feb 2025 | Started contributing to TheNoor iOS |
| Aug 2025 | TheNoor Android Kotlin project |
| Oct 2025 | TheNoor Pro Android codebase: main author (590+ commits), GitHub Actions CI, 200+ unit tests |
| Jul 2026 | SolatSDK, a Swift package for prayer times used by the iOS app |
| Oct 2026 | TheNoor admin/monitoring app, Wear OS companion, iOS Quran parity |
| Oct–Nov 2026 | Personal apps: Kotlin Multiplatform (SplitBill, ResitKu, MoewKita, Cerita Nusantara), native Android and iOS (Banjir Sepang, Layar Kita, HurufPlay, Coway Remote), Flutter (ServiceBiz, Go Coffee + staff app) |
| Nov 2026 | First React Native app: StudyNest (Expo, TypeScript, SQLite) |

---

### 🏗 Architecture and state management I've used

| Where | Architecture | State / data |
|---|---|---|
| TheNoor Android (production) | Activities/Fragments, ViewModel, central deep-link router (IntentRouter/IntentRegistry), ongoing Java → Kotlin migration | LiveData, Kotlin Coroutines, WorkManager, foreground services, Volley, SharedPreferences, Firebase Cloud Messaging |
| TheNoor Car (production) | MVVM with Hilt dependency injection | ViewModel, Coroutines, Room |
| Flutter apps (Go Coffee, ServiceBiz) | Feature folders, repository pattern behind interfaces, offline-first | Riverpod (Notifier / AsyncNotifier), go_router, Drift and sqflite (SQLite) |
| Kotlin Multiplatform apps (SplitBill, ResitKu, MoewKita, Cerita Nusantara) | Shared domain and data in `commonMain`, Compose Multiplatform UI, `expect`/`actual` for platform code | Compose state and StateFlow (ViewModel in Cerita Nusantara), SQLDelight / SQLite |
| Native Android apps (Banjir Sepang, Layar Kita, HurufPlay, Coway Remote) | Jetpack Compose, single activity | ViewModel, StateFlow / Compose state, AndroidX Media3 |
| iOS (Banjir Sepang, TheNoor Quran features) | SwiftUI | Swift concurrency |
| React Native (StudyNest) | Expo Router, pure domain layer separate from screens, repositories over SQL | expo-sqlite with versioned migrations, Zustand for UI state |

### ✅ Automated testing

- **TheNoor Android:** wrote most of its unit test suite (69 test files, 213 tests) with JUnit and Robolectric;
  Espresso set up for UI tests.
- **Kotlin Multiplatform:** shared `commonTest` unit tests with kotlin.test (bill-splitting maths, Malaysian receipt
  parsing, cat-photo matching).
- **React Native:** Vitest tests for the spaced-repetition scheduler, streaks, quiz scoring, backup rollback and
  the data layer against real SQLite.
- **Flutter:** unit tests (pricing, cart totals, vouchers, rewards, receipt layout) and widget tests (menu, product
  options to cart, checkout validation).

### ⚙️ CI/CD

- **GitHub Actions, TheNoor Android (I wrote it):** on every push and pull request it checks resources (XML,
  duplicates, translation placeholders), builds, runs lint and unit tests; it also builds a signed release
  `.aab` when the signing secrets are present.
- **GitHub Actions, personal apps (HurufPlay, Layar Kita):** unit tests, lint and a debug APK on every push, with
  the APK and the test/lint reports uploaded as build artifacts.
- **Monitoring:** Firebase Crashlytics and Performance Monitoring in the TheNoor apps; BigQuery exports for usage
  and crash analysis.

### 🌙 Work highlights at TheNoor

- Made azan (prayer-time) alerts reliable: fixed missed and stale alarms and added a WorkManager watchdog and a health
  log to catch failures.
- Built an offline fallback for the muezzin audio after the API started returning broken data.
- Quran module: offline playback, media notifications, verse highlight sync, Mushaf ayah highlighting, dark mode.
- Crash fixes across the main screens: fragment transactions after state save, JSON parsing, null safety,
  Geocoder moved off the main thread.
- Fixed a multi-layer location bug ("Earth, Unknown") with a three-step GPS fallback.

---

### 🚀 Projects

| Project | What it is | Stack |
|---|---|---|
| **Go Coffee** | Order-ahead app for a Malaysian coffee shop, plus a staff app that receives orders over the shop Wi-Fi, marks items sold out, shows the day's sales and prints receipts on a Sunmi V2 | Flutter, Riverpod, Drift, local HTTP server, Android foreground service, Sunmi printer |
| **StudyNest** | Offline flashcards, quizzes and spaced review, with study packs and JSON backup | React Native, Expo, TypeScript, expo-sqlite |
| **SplitBill** | Snap a restaurant receipt, split it with tax, send each person their amount on WhatsApp | Kotlin Multiplatform, Compose Multiplatform, ML Kit / Apple Vision OCR |
| **ResitKu** | Receipt keeper for spending and LHDN tax-relief claims, read on the phone with no internet | Kotlin Multiplatform, Compose Multiplatform, SQLite, on-device OCR |
| **ServiceBiz** | Run an aircon service business: customers, units, bookings, quotations, invoices, WhatsApp follow-ups | Flutter, Riverpod, go_router, sqflite |
| **Banjir Sepang** | Flood watch for Sepang: river levels, gauges, sirens, rainfall, CCTV, alerts when water near you rises | Kotlin + Compose (Android), Swift + SwiftUI (iOS) |
| **Layar Kita** | Malaysian TV and radio player with background radio, car mode and Android Auto | Kotlin, Compose, AndroidX Media3, GitHub Actions |
| **Cerita Nusantara** | Offline read-aloud storybook of Malaysian folklore for kids, phones and tablets | Kotlin Multiplatform, Compose Multiplatform |
| **MoewKita** | Get to know the stray cats in your taman: profiles, photos, comments, a cat scanner | Kotlin Multiplatform, SQLDelight |
| **HurufPlay** | Kids practise writing A–Z and draw freely, with Malay prompts | Kotlin, Compose, GitHub Actions |
| **Coway Aircond Remote** | Turns a phone with an IR blaster into a remote for Coway inverter air conditioners | Kotlin, Compose, ConsumerIrManager |

Most of these repos are private. Happy to share access or a live demo on request.

### 🧰 Full toolset

- **Languages:** Kotlin · Java · Dart · Swift · TypeScript
- **Android:** Jetpack Compose · XML views · Hilt · Room · WorkManager · Media3 · Coroutines · Firebase (FCM, Crashlytics, Performance)
- **Cross-platform:** Flutter (Riverpod, go_router, Drift) · Kotlin Multiplatform + Compose Multiplatform (SQLDelight) · React Native + Expo (Expo Router, expo-sqlite)
- **iOS:** SwiftUI · Xcode
- **Testing:** JUnit · Robolectric · Espresso · kotlin.test · flutter_test · Vitest
- **CI/CD and tooling:** GitHub Actions · Gradle · signed AAB builds · Android lint · Git / GitHub · Android Studio
