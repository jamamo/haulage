# 🚛 Haulage HQ — Driving Hours Tracker
 
A web-based driving hours tracker for UK/EU road haulage, compliant with **EC Regulation No 561/2006**.
 
## Features
 
### Driver Dashboard
- **Live timer** with Start / Pause (break) / Stop controls
- **Real-time warnings** when approaching continuous (4.5h), daily (9h), or weekly (56h) limits
- **Browser notifications** — get alerted even when the tab is in the background (permission prompt on first use)
- **Visual gauges** showing usage against legal maximums
- **Tab title updates** — shows live driving/break time in the browser tab
- Automatic continuous driving reset after 45-minute break
 
### History & Export
- Browse driving records by date
- View individual session breakdowns with break durations
- Export to **CSV** filtered by week, month, or all time
- Ready for tachograph compliance and employer records
 
### Admin Panel
- Add, disable, and delete drivers
- Reset driver PINs
- View any driver's full session history
- Export combined records for all drivers
- Fleet overview stats (total drivers, sessions, hours)
 
### Regulatory Compliance
- UK/EU Drivers' Hours rules enforced:
  - 4h 30m max continuous driving → 45-min mandatory break
  - 9h daily driving limit (10h twice per week)
  - 56h weekly / 90h fortnightly caps
  - 11h minimum daily rest
- Quick-reference rules page built in
 
## Hosting on GitHub Pages
 
1. Create a new GitHub repository
2. Upload `index.html` to the repo root
3. Go to **Settings → Pages**
4. Under "Source", select **Deploy from a branch**
5. Choose `main` branch and `/ (root)` folder
6. Click **Save**
7. Your app will be live at `https://yourusername.github.io/repo-name/`
 
## Login
 
**Admin access:** Use the Admin tab on the login screen with your registered email and password.
 
**Drivers:** Drivers log in with their name and PIN as set up by the admin.
 
## Technical Details
 
- **Single-file app** — no build step, no dependencies to install
- **React 18** via CDN with Babel for JSX transpilation
- **localStorage** for data persistence (data stays on the user's device/browser)
- **Fully responsive** — works on mobile, tablet, and desktop
- **Offline-capable** once loaded (no server calls needed)
 
## ⚠️ Important Notes
 
- This is a **tracking aid only** — it does not replace an approved tachograph or legal record-keeping obligations
- Data is stored in the browser's localStorage — clearing browser data will remove all records
- Admin credentials are visible in source code — suitable for personal/small-team use only. For production use, implement proper backend authentication
 
## License
 
MIT
