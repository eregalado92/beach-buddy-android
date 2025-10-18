# Beach Buddy — Android-first (Expo React Native)

> A simple, fast way to check tides, wind, swell, UV, and advisories for South Florida beaches—and log your sessions with alert notifications.

## ✨ Features (MVP)
- Conditions dashboard (today + next 24–48h)
- Personal alerts (thresholds for wind/swell/UV)
- Quick session logs with notes & photos
- Profile: home spot, units, notification settings

## 🧱 Tech Stack
- **Frontend:** React Native (Expo), React Navigation, TypeScript
- **State/Data:** Zustand or Redux Toolkit, React Query
- **Backend:** Firebase Auth, Firestore, Cloud Functions, Storage, FCM
- **Dev:** EAS builds, Jest/React Native Testing Library

## 🏗️ Architecture (High-level)
```
App (RN/Expo) → Services (Conditions/Alerts/Logs) → Firebase (Auth, Firestore, Storage, FCM)
                              ↘ External Data (NOAA/NWS) via Cloud Functions (cache)
```

## 🚀 Getting Started
```bash
# 1) Clone
git clone https://github.com/eregalado92/beach-buddy-android.git
cd beach-buddy-android

# 2) Install deps
npm install

# 3) Configure env
# If .env.example exists:
# cp .env.example .env
# Otherwise create a .env file and add the keys below.

# 4) Run the app
npx expo start
```

## 🔐 Environment
Create a `.env` file with:
```
EXPO_PUBLIC_FIREBASE_API_KEY=...
EXPO_PUBLIC_FIREBASE_AUTH_DOMAIN=...
EXPO_PUBLIC_FIREBASE_PROJECT_ID=...
EXPO_PUBLIC_FIREBASE_STORAGE_BUCKET=...
EXPO_PUBLIC_FIREBASE_MESSAGING_SENDER_ID=...
EXPO_PUBLIC_FIREBASE_APP_ID=...
```

## 📚 Documentation / Wiki
Main outline, architecture details, and wireframes live in the Wiki:  
https://github.com/eregalado92/beach-buddy-android/wiki
- Wireframes: **[Design / Wireframes](https://github.com/eregalado92/beach-buddy-android/wiki/Design-/-Wireframes)**


## 🗺️ Roadmap
- [x] Outline & mock data
- [ ] Dashboard UI
- [ ] Auth + Firestore
- [ ] Alerts + notifications
- [ ] Replace mocks with live data

## 📝 Changelog
- **v0.3 (Week 4):** Updated outline and wireframes; clarified data models and security; added `.gitignore`; verified links.
- **v0.2 (Week 3):** Repo + initial README; Wiki pages (Home/Architecture/Design/Milestones/Testing/Risks) and sidebar created.
- **Full week-by-week details live here:** [CHANGELOG.md](./CHANGELOG.md)

## 📄 License
MIT
