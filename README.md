# 💕 WinkLink

WinkLink is a **fun social app for couples and singles** that lets users send **private winks** to their partner or **local winks** to nearby WinkLink users using Bluetooth/WiFi.  
Cute animations, sounds, and date suggestions make it playful and engaging.  

---

## ✨ Features

### ❤️ Couples Mode
- Send unlimited **private winks** to your partner.
- Receive winks with **cute animations and tones**.
- **History timeline** of winks between partners.
- **Daily streaks** for consistent love bytes.

### 🌍 Local Wink Mode
- Discover nearby WinkLink users via **Bluetooth / WiFi Direct**.
- Send **random winks** to users in the area.
- Receiver can **Accept** or **Ignore**.
  - **Accept** → creates a match in the backend and suggests a random date.
  - **Ignore** → wink disappears.
- Safety features: block or report users.

### 🔔 Common Features
- Firebase authentication (email/Google login).
- User profile setup: name, gender, relationship status, profile picture.
- Notifications for received and accepted winks.
- Fun animations (Lottie) and sounds for interactions.

---

## 🛠 Tech Stack

### Frontend (Flutter)
- **Flutter** (cross-platform: iOS & Android)
- **State Management**: Riverpod / Provider / Bloc (team preference)
- **Animations**: [Lottie](https://pub.dev/packages/lottie)
- **Sounds**: [audioplayers](https://pub.dev/packages/audioplayers)
- **Nearby Communication**:
  - [`flutter_blue_plus`](https://pub.dev/packages/flutter_blue_plus) → Bluetooth Low Energy (BLE)
  - [`wifi_p2p`](https://pub.dev/packages/wifi_p2p) → WiFi Direct

### Backend (Firebase)
- **Firebase Auth** → user authentication
- **Cloud Firestore** → winks, matches, user profiles
- **Firebase Cloud Messaging (FCM)** → push notifications
- **Firebase Storage** → profile images

---
📊 App Flow

Authentication → User logs in with Firebase Auth.

Profile Setup → Name, gender, photo, relationship status.

Couples Mode:

Send/receive private winks with animations + sounds.

Stored in couple_winks.

Local Wink Mode:

Discover nearby users (Bluetooth/WiFi).

Send random wink → Accept/Ignore.

Accepted winks stored in local_winks + match created.

🚀 Roadmap
Phase 1 (MVP)

Auth + profiles

Couple winks

Local winks (send/receive, accept/ignore)

Phase 2

Notifications (FCM)

Wink streaks and gamification

Random date suggestions

Phase 3

In-app chat for matches

Advanced filters (interests, distance)

Premium features (unlimited winks, boosted visibility)

🧑‍🎨 Credits

Designed and thought by Rajat Srivastav
