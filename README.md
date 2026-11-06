# EmergencyQR - Offline Emergency Medical ID QR Web App (PWA)

A cross-platform, accessible, and offline-capable Emergency Medical ID Progressive Web App. EmergencyQR generates a high-density, human-readable emergency QR code that can be scanned by **ANY standard smartphone camera** (iPhone, Android, Samsung, Google Lens) or hospital barcode scanner without requiring a specialized app or internet connection.

---

## 🚑 Key Features

- **Universal Scanner Compatibility**:
  - Encodes structured emergency medical data in plaintext.
  - Default camera apps on iOS and Android instantly display complete medical details and provide one-tap emergency calling (`CALL: <number>`).
- **Critical Medical Profile**:
  - Full Name, Date of Birth, Age, and Blood Type badge.
  - Allergies and Medical Conditions alert box.
  - Current Medications and Emergency Instructions.
  - In Case of Emergency (I.C.E.) contact person and phone number.
  - Personal contact number and residential address.
  - Registered Identification Documents (Driver's License, PhilHealth, SSS, UMID, Passport, National ID, etc.).
- **PWD & Inclusive Accessibility**:
  - **Digit-by-Digit Number Speech**: ID numbers and phone numbers are spoken digit-by-digit (e.g., `1, 2, 3, dash, 4, 5`) rather than grouped into large numbers.
  - **Voice Dictation (Speech-to-Text)**: Fill out fields hands-free using microphone speech recognition.
  - **Text-to-Speech Voice Guidance**: Audio readouts for individual fields, full emergency profile summary, and live status announcements.
  - **Theme Toggle**: One-click toggle between Dark Mode and High-Contrast Light Mode.
  - **Dynamic Font Scaling**: Quick `A-` / `100%` / `A+` font size adjustments.
  - **WCAG Compliant Touch Targets**: Minimum 48px touch targets and full keyboard tab navigation.
- **100% Offline & Private**:
  - Built as a Progressive Web App (PWA) with a Cache-First Service Worker.
  - Stores all profile data and ID photos locally on the device (LocalStorage & IndexedDB).
  - Zero analytics, zero cookies, zero external server tracking.
- **Backup & Restore**:
  - Export and import complete encrypted JSON backups including compressed photo attachments.

---

## 🛠️ Tech Stack

- **HTML5 & Modern CSS3**: Responsive grid layouts, CSS custom properties, zero-overflow mobile fitting.
- **Vanilla JavaScript**: Pure zero-dependency client logic.
- **Lucide Vector Icons**: Clean, scalable inline SVG icons (no raw emojis).
- **Web Speech API**: `SpeechRecognition` for voice dictation and `SpeechSynthesis` for audio readouts.
- **Web Audio API**: Synthesized audio frequency feedback beeps (`AudioContext`).
- **HTML5 Canvas & QR Generator**: Local client-side QR matrix rendering.
- **IndexedDB**: Local photo storage with automatic canvas thumbnail resizing.
- **Service Worker API**: Offline asset caching.

---

## 🚀 How to Run Locally

1. Clone this repository:
   ```bash
   git clone https://github.com/Chardddyyy/EmergencyQR.git
   cd EmergencyQR
   ```

2. Start a local static HTTP server:
   ```bash
   # Python 3
   python3 -m http.server 8080
   ```

3. Open your browser:
   ```
   http://localhost:8080
   ```

---

## 📱 Installation as PWA

- **iOS Safari**: Tap the Share button (`⎋`) $\rightarrow$ Tap **Add to Home Screen**.
- **Android Chrome**: Tap the menu (`⋮`) $\rightarrow$ Tap **Install App** or **Add to Home screen**.

---

## 📄 License

MIT License. Free to use for personal, medical, and emergency rescue purposes.
