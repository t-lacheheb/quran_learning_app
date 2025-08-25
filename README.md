# 📖 Qur'an Sessions Manager (AR/EN/FR)

A **Flutter mobile application** designed to help individuals, groups, and teachers **manage Qur’an memorization, recitation, and study sessions** with ease.  
The app provides a **multilingual interface** (Arabic / English / French) to make it accessible to a wider audience of learners and educators worldwide.  

---

## 🌟 Features

- 🕌 **Session Management**  
  Create, track, and organize Qur’an sessions (memorization, revision, or recitation).  

- 📊 **Progress Tracking**  
  Monitor student or personal progress by Surah, Juz’, or page.  

- 👥 **Group & Individual Support**  
  Manage sessions for single users or entire study circles (halaqat).  

- 🔔 **Reminders & Notifications**  
  Stay on track with smart notifications for planned sessions.  

- 🌍 **Multilingual Support**  
  Switch seamlessly between **Arabic**, **English**, and **French** interfaces.  

- 📱 **Simple & Modern UI**  
  Lightweight, intuitive design built with Flutter for Android & iOS.  

---

## 🖥️ Use Cases

- **Students**: Track your memorization journey and stay motivated.  
- **Teachers / Imams**: Manage groups, assign Surahs, and monitor progress.  
- **Families**: Organize Qur’an learning at home for children and parents.  

---

## 🌐 Languages

- **🇸🇦 Arabic (العربية)**  
- **🇬🇧 English**  
- **🇫🇷 French (Français)**  

---

## 🚀 Tech Stack

- **Framework**: Flutter  
- **Database**: Firebase 
- **Platform**: Android & iOS  

---

## 📌 Vision

> “To make Qur’an learning and memorization more **organized, accessible, and motivating** for Muslims around the world.”  

---

## 📷 Screenshots (Coming Soon)

---

## 📄 License

This project is licensed under the MIT License – feel free to use and contribute.  

---

### 🙌 Contribute
We welcome contributions in features, translations, and design improvements. Open a pull request or submit issues to help us grow this project together.  

### 📜 Detailed Description

#### Overview
Qur'an Sessions Manager is a Flutter app that helps learners, families, and teachers plan, run, and review Qur'an-focused activities. It supports memorization (hifz), revision (muraja'ah), and recitation practice with structured sessions, progress tracking, and reminders. The app is multilingual by design (AR/EN/FR) and aims to be simple for individuals yet powerful for halaqah/group management.

#### Core Concepts
- **Session**: A scheduled block of time with a purpose (e.g., memorize Surah Al-Mulk ayat 1–10). Sessions can be one-off or recurring.
- **Scope**: Memorization, revision, or recitation. Each scope has different progress metrics.
- **Assignment**: A defined range (by Surah, Juz', page, or ayah range) attached to a session or a learner.
- **Progress Entry**: Evidence of what was completed during/after a session (e.g., “memorized ayat 1–5, needs improvement on 4–5”).
- **Group**: A collection of learners managed by a teacher/imam/parent. Groups can have shared sessions and aggregated reports.

#### User Roles
- **Admin**: Manages institutions/halaqat, user accounts, role assignments, groups, and global settings.
- **Teacher/Imam**: Creates group sessions, assigns ranges to learners, reviews submissions, and monitors class progress.
- **Parent/Guardian**: Manages sessions for children, sets reminders, and views per-child progress.
- **Student/Learner**: Plans personal sessions, completes assignments, submits progress, and receives feedback.

#### Session Lifecycle
1. **Plan**: Create a session with scope, assignment (range), date/time, recurrence, and optional notes.
2. **Notify**: The app sends a reminder before the session.
3. **Conduct**: Run the session; optionally use a timer and checklist for quality criteria (tajwīd focus, fluency, retention).
4. **Review**: Record a progress entry, mark difficulties, and add teacher/parent feedback.
5. **Track**: View updated dashboards by Surah/Juz'/page, including streaks and revision coverage.

#### Progress by Role
- **Admin**
  - View organization-wide metrics (active groups, active learners, session completion rates).
  - Audit activity logs and enforce data retention/security policies.
  - Export high-level reports (by group/teacher/time period).
- **Teacher/Imam**
  - Track per-learner progress by Surah/Juz'/page and recent streaks.
  - Review submissions with flags (accuracy/fluency), leave feedback, and approve.
  - See class dashboards: coverage heatmaps, pending reviews, attendance, and reminders.
- **Parent/Guardian**
  - View each child's assignments, session history, streaks, and areas needing revision.
  - Receive reminders and recap summaries; co-sign reviews where applicable.
- **Student/Learner**
  - See upcoming sessions, assignments, streaks, and targets.
  - Log progress entries, mark difficulties, and view teacher feedback.

#### Data & Tracking
- **Units**: Surah, Juz', page number, and ayah range are supported addressing schemes.
- **Metrics**: Completion status, accuracy/fluency flags, notes, and optional audio attachments (future roadmap).
- **Reports**: Personal trends, per-learner summaries for groups, and coverage heatmaps (planned).

#### Architecture (High Level)
- **Frontend**: Flutter (Android/iOS) with internationalization for AR/EN/FR.
- **Backend/Storage**: Firebase (authentication, Firestore/Realtime DB, Cloud Functions as needed).
- **Sync**: Offline-friendly reads with eventual consistency when online (subject to Firebase rules and caching).
- **Notifications**: Firebase Cloud Messaging or platform schedulers for reminders.

#### Privacy & Safety
- Minimal personal data; data is scoped to the user or their group.
- Role-based access in groups; teachers only see their groups.
- Follows Firebase security rules; do not share sensitive personal info inside free-text notes.

#### Roadmap (Planned)
- Audio notes and self-recitation attachments for review.
- Advanced analytics: revision spacing suggestions and coverage gaps.
- Import/export progress, share reports as PDF.
- Tajwīd focus tags and custom rubrics per session.
- Expanded localization and RTL polishing.

#### Getting Started (Development)
1. Install Flutter and set up Android/iOS tooling.
2. Clone the repository and run `flutter pub get`.
3. Create a Firebase project, add Android/iOS apps, and configure `google-services` files.
4. Run `flutter run` on a connected device/emulator.

#### Contributing & Translations
- Contributions are welcome: features, UI/UX, performance, testing.
- Translation contributions for AR/EN/FR and additional languages are encouraged.
- Please open an issue to discuss substantial changes before submitting an edit.
