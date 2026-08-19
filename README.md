# TaskDeck Web (`taskdeck-web`)

Static web assets for **TaskDeck** (formerly ATask), a native multi-account Google Tasks and Google Calendar desktop application built for macOS.

This repository hosts the static landing page, privacy policy, and terms of service deployed via GitHub Pages at [taskdeck.agoldschmidt.com](https://taskdeck.agoldschmidt.com). These pages satisfy the official web verification requirements for **Google Cloud Console OAuth Verification** and **Apple App Store Connect Submission**.

---

## 📁 Repository Structure

```text
.
├── CNAME           # Custom domain mapping (taskdeck.agoldschmidt.com)
├── index.html      # Product landing page and app overview
├── privacy.html    # Privacy policy covering local storage and Google OAuth scope usage
├── terms.html      # Terms of service for TaskDeck users
└── README.md       # Project documentation
```

---

## 🌐 Live Hosted Pages

* **Homepage**: [https://taskdeck.agoldschmidt.com](https://taskdeck.agoldschmidt.com) — Product introduction and feature overview.
* **Privacy Policy**: [https://taskdeck.agoldschmidt.com/privacy.html](https://taskdeck.agoldschmidt.com/privacy.html) — Details local-first storage (macOS Keychain & SQLite) and compliance with Google API User Data Policies.
* **Terms of Service**: [https://taskdeck.agoldschmidt.com/terms.html](https://taskdeck.agoldschmidt.com/terms.html) — Terms of use for the native application.

---

## ⚙️ OAuth & Store Verification Requirements

### Google Cloud Console
Hosts the required authorized domain URLs for Sensitive Scope OAuth Verification:
1. Application Homepage URL
2. Privacy Policy detailing Google Tasks (`/auth/tasks`) and Google Calendar (`/auth/calendar`) scope usage, local-only data retention, and macOS Keychain security.
3. Terms of Service Link

### Apple App Store Connect
Provides the required **Privacy Policy URL** and **Marketing/Support URL** metadata for macOS App Store submission.

---

## 🛠️ Local Development & Deployment

This project consists of pure static HTML/CSS with zero build steps or external dependencies.

1. **Local Preview**: Open `index.html` directly in any web browser.
2. **Deployment**: Pushes to the `main` branch automatically deploy via GitHub Pages using the custom domain configured in standard DNS and the `CNAME` file.
