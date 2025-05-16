# Live Voting App

A simple real-time yes/no voting web app using Firebase Realtime Database.

Users can vote "YES" or "NO" once per round from any device. An admin page allows resetting the votes, which starts a new voting round and unlocks voting for everyone again.

## Features

- Real-time voting updates using Firebase Realtime Database
- One vote per user per round (tracked locally in the browser)
- Percentage and visual bar display of votes
- Admin page to reset votes and start a new round
- Responsive design, works on mobile devices
- QR code support to quickly access the voting site

## Files

- `index.html` — Main voting page for users
- `admin.html` — Admin page to reset votes
- `QRCODE.png` — QR code image linking to the voting site

## Setup Instructions

1. **Firebase Setup:**
   - Create a Firebase project at [Firebase Console](https://console.firebase.google.com/)
   - Enable Realtime Database and set rules to allow read/write as needed (for demo, rules can be open; for production, secure accordingly)
   - Copy your Firebase config object

2. **Configure Your App:**
   - Replace the `firebaseConfig` object in both `index.html` and `admin.html` with your Firebase project's config

3. **Deploy:**
   - Upload your files to your hosting environment (GitHub Pages, Firebase Hosting, etc.)
   - Ensure `QRCODE.png` is in the same directory as your HTML files or adjust the image path accordingly

## Usage

- Users visit `index.html` to vote
- Each user can vote once per round (tracked via browser localStorage)
- Votes update live for all users
- Admin visits `admin.html` to reset the votes and start a new round

## Notes

- The voting restriction relies on browser localStorage — users can clear storage or use different browsers/devices to vote again.
- For stronger user authentication, consider integrating Firebase Authentication.
- Customize styles and colors in the CSS as desired.

---

Feel free to open issues or contribute!

---

© 2025 Your Name
