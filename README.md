# StudentOS DZ — Ultimate

StudentOS DZ is a frontend-only student operating system for Algerian university students.

## Features
- Local Register / Login
- Profile + local profile picture
- Arabic / Français / English with RTL/LTR
- Light / Dark mode
- Algerian-style semester average calculator (CC/TD + Exam, configurable weights)
- Pomodoro / Focus Lab: 25/5, 50/10, 90/15 and custom
- Focus session history
- XP, levels and streaks
- Study challenges and badges
- Local Study Rooms + leaderboard
- Study Planner with filters
- Analytics based on real local activity
- JSON Export / Import
- Responsive mobile navigation

## Run
Open `index.html` directly in a browser. No build step and no backend are required.

## Security & Limitations Note
This is a **Frontend/Local Demo**. Authentication is not real security: passwords are stored locally in the browser and are not cryptographically protected. Do not use real sensitive passwords.

Study Rooms are local-only and do not synchronize users between different devices because there is no backend.

For production, replace the local DataStore with a real backend/API, database, authentication, authorization and secure storage (for example Node.js + PostgreSQL, or a managed backend such as Supabase/Firebase).

## Architecture
The app uses a single structured local state under one versioned DataStore key to keep the zero-setup deployment simple. All application persistence goes through the `Store` abstraction in `app.js`, making a future backend migration straightforward.

## GitHub Pages
1. Create a new repository.
2. Upload `index.html`, `style.css`, `app.js`, and `README.md`.
3. In repository Settings → Pages, choose **Deploy from a branch** and select `main` / root.
4. Open the generated Pages URL.

## License
Add your preferred license before public/commercial distribution.
