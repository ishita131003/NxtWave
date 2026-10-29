# NxtWave Growth Hub (assessment prototype, not affiliated with NxtWave)
Single-file app: no npm, no build step, no backend, no secrets, no .env needed.

## Run on Windows (beginner)
1. Right-click the ZIP > Extract All.
2. Double-click `index.html` (opens in Chrome or Edge).
3. Optional, to test `?ref=CODE` links: open the folder, type `cmd` in the address bar, run `python -m http.server 8000`, visit http://localhost:8000

## Build / deploy
Build command: none. The deployable output is `dist/index.html`; upload the `dist` folder to Netlify, Vercel or GitHub Pages.

## Demo logins (local simulation only, never use in production)
Student: student.demo@example.com / StudentDemo@123
Admin (Admin in the header): admin.demo@example.com / AdminDemo@123

## Real vs demo
Real: validation, SHA-256 password hashing, duplicate-email and self-referral blocks, role-guarded views, referral attribution, CSV export, editable targets and budget.
Demo-only: data lives in this browser's localStorage (not shared across devices); seed records are fictional; admin security is client-side only. Not built: Supabase, email sending, click tracking, QR codes, Vite/React/Tailwind.
Reset: Admin > Campaign Settings > Reset demo data.

## Build & Learn video
Student "Build & Learn" shows an honest "video not available" state until you set `VIDEO_URL` (near the top of the v4 section in index.html) to a real MP4/WebM or .m3u8 URL.
