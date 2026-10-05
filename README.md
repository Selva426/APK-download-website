# 📲 Selva's Apps

A simple download page for my Android apps. Open the link on your phone, tap Download, install.

**🌐 Live site:** [[https://selva426.github.io/apps/](https://github.com/actions/runner-images/issues/14748)](https://selva426.github.io/APK-download-website/)

<!-- Add a screenshot: ![Site preview](docs/site.png) -->

## Apps

| App | What it does | Source |
|---|---|---|
| ❄️ **Winter Arc** | Daily habit tracker with streaks, a weekly summary, a water tracker and a daily schedule | [winter-arc](https://github.com/Selva426/winter-arc) |
| 🏋️ **Iron Log** | Workout tracker with custom exercises, auto weight progression, PR tracking and charts | [iron-log](https://github.com/Selva426/iron-log) |

Both apps work fully offline, with no login, no ads and no tracking. Data stays on the device.

## How the site works
```
GitHub Pages (static site)
   ├── index.html          landing page
   ├── assets/             app icons
   └── downloads/          APK files served directly
```
- Plain HTML and CSS, with no framework and no build step
- Download buttons link straight to the APK files in `downloads/`
- File sizes are read from the server at page load
- Mobile-first layout

## Install an app
1. Open the live site in **Chrome on Android**
2. Tap **Download APK**
3. Open the downloaded file and allow *Install unknown apps* if asked
4. Tap Install. If Play Protect warns you, tap *Install anyway*

> These are debug builds shared for personal use, not Play Store releases.

## Update an app
1. Open the `downloads/` folder
2. **Add file → Upload files** and drop in the new APK
3. Keep the same filename (`winter-arc.apk` or `iron-log.apk`) so the link keeps working
4. Commit. The site updates in about a minute

## Run locally
Open `index.html` in a browser. No setup needed.

## Tech
HTML · CSS · vanilla JavaScript · GitHub Pages

## Preview

![Home page](docs/site-home.png)
![Install steps](docs/site-install.png)
