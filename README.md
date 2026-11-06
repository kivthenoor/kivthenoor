### Hi, I'm Akif 👋

Mobile developer in Malaysia. Android (Kotlin and Java) in production, plus Flutter, Kotlin Multiplatform and
SwiftUI apps of my own, mostly offline-first apps for Malaysian users.

**Now:** Android developer on [TheNoor](https://play.google.com/store/apps/details?id=com.thenoor.app), a Muslim
lifestyle and worship app (Quran reading and audio, prayer times and azan alerts, donations and commerce), its car
head-unit app and a Wear OS companion. Main author of the current Android codebase (590+ commits).

Earlier work and most of my TheNoor history (2022–2025) is on my previous account,
[@kivfauzi](https://github.com/kivfauzi).

---

### Progress

About 940 commits across TheNoor's Android, iOS, car and SDK repos since May 2024, plus 11 personal apps.

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

---

### Architecture and state management I've used

| Where | Architecture | State / data |
|---|---|---|
| TheNoor Android (production) | Activities/Fragments, ViewModel, central deep-link router (IntentRouter/IntentRegistry), ongoing Java → Kotlin migration | LiveData, Kotlin Coroutines, WorkManager, foreground services, Volley, SharedPreferences, Firebase Cloud Messaging |
| TheNoor Car (production) | MVVM with Hilt dependency injection | ViewModel, Coroutines, Room |
| Flutter apps (Go Coffee, ServiceBiz) | Feature folders, repository pattern behind interfaces, offline-first | Riverpod (Notifier / AsyncNotifier), go_router, Drift and sqflite (SQLite) |
| Kotlin Multiplatform apps (SplitBill, ResitKu, MoewKita, Cerita Nusantara) | Shared domain and data in `commonMain`, Compose Multiplatform UI, `expect`/`actual` for platform code | Compose state and StateFlow (ViewModel in Cerita Nusantara), SQLDelight / SQLite |
| Native Android apps (Banjir Sepang, Layar Kita, HurufPlay, Coway Remote) | Jetpack Compose, single activity | ViewModel, StateFlow / Compose state, AndroidX Media3 |
| iOS (Banjir Sepang, TheNoor Quran features) | SwiftUI | Swift concurrency |

### Automated testing

- **TheNoor Android:** wrote most of its unit test suite (69 test files, 213 tests) with JUnit and Robolectric;
  Espresso set up for UI tests.
- **Kotlin Multiplatform:** shared `commonTest` unit tests with kotlin.test (bill-splitting maths, Malaysian receipt
  parsing, cat-photo matching).
- **Flutter:** unit tests (pricing, cart totals, vouchers, rewards, receipt layout) and widget tests (menu, product
  options to cart, checkout validation).

### CI/CD

- **GitHub Actions, TheNoor Android (I wrote it):** on every push and pull request it checks resources (XML,
  duplicates, translation placeholders), builds, runs lint and unit tests; it also builds a signed release
  `.aab` when the signing secrets are present.
- **GitHub Actions, personal apps (HurufPlay, Layar Kita):** unit tests, lint and a debug APK on every push, with
  the APK and the test/lint reports uploaded as build artifacts.
- **Monitoring:** Firebase Crashlytics and Performance Monitoring in the TheNoor apps; BigQuery exports for usage
  and crash analysis.

### Work highlights at TheNoor

- Made azan (prayer-time) alerts reliable: fixed missed and stale alarms and added a WorkManager watchdog and a health
  log to catch failures.
- Built an offline fallback for the muezzin audio after the API started returning broken data.
- Quran module: offline playback, media notifications, verse highlight sync, Mushaf ayah highlighting, dark mode.
- Crash fixes across the main screens: fragment transactions after state save, JSON parsing, null safety,
  Geocoder moved off the main thread.
- Fixed a multi-layer location bug ("Earth, Unknown") with a three-step GPS fallback.

---

### Projects

| Project | What it is | Stack |
|---|---|---|
| **Go Coffee** | Order-ahead app for a Malaysian coffee shop, plus a staff app that receives orders over the shop Wi-Fi, marks items sold out, shows the day's sales and prints receipts on a Sunmi V2 | Flutter, Riverpod, Drift, local HTTP server, Android foreground service, Sunmi printer |
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

### Tools

- **Languages:** Kotlin · Java · Dart · Swift
- **Android:** Jetpack Compose · XML views · Hilt · Room · WorkManager · Media3 · Coroutines · Firebase (FCM, Crashlytics, Performance)
- **Cross-platform:** Flutter (Riverpod, go_router, Drift) · Kotlin Multiplatform + Compose Multiplatform (SQLDelight)
- **iOS:** SwiftUI · Xcode
- **Testing:** JUnit · Robolectric · Espresso · kotlin.test · flutter_test
- **CI/CD and tooling:** GitHub Actions · Gradle · signed AAB builds · Android lint · Git / GitHub · Android Studio
