# CODIV — Premium Web Development & Digital Solutions

[![License: Custom Attribution](https://img.shields.io/badge/License-Custom%20Attribution-red.svg)](LICENSE)
[![HTML5](https://img.shields.io/badge/HTML5-E34F26?style=flat&logo=html5&logoColor=white)](https://developer.mozilla.org/en-US/docs/Web/Guide/HTML/HTML5)
[![CSS3](https://img.shields.io/badge/CSS3-1572B6?style=flat&logo=css3&logoColor=white)](https://developer.mozilla.org/en-US/docs/Web/CSS)
[![JavaScript](https://img.shields.io/badge/JavaScript-F7DF1E?style=flat&logo=javascript&logoColor=black)](https://developer.mozilla.org/en-US/docs/Web/JavaScript)
[![Firebase](https://img.shields.io/badge/Firebase-FFCA28?style=flat&logo=firebase&logoColor=black)](https://firebase.google.com/)
[![Three.js](https://img.shields.io/badge/Three.js-black?style=flat&logo=three.js&logoColor=white)](https://threejs.org/)

CODIV is a high-performance, ultra-premium digital solutions platform built with an editorial dark-mode aesthetic. It offers seamless web development services, real-time order lifecycle tracking, UPI token payments, an administrative command center, dynamic client analytics, and an integrated AI assistant.

---

## ✨ Features

- **🖤 Editorial Noir Design System**: Precision dark typography, fluid micro-animations, glassmorphism, responsive grid architecture, and customized cursor physics.
- **🌐 3D Interactive WebGL Background**: Immersive particle & geometry effects powered by Three.js.
- **📦 Complete Order Management**:
  - Full Order ID display with 1-click clipboard copy (`📋 Copy ID`) and compact/full toggle options.
  - Multi-tier package configuration with real-time quote generation and coupon discount engine.
  - Real-time status pipeline (Order Received → Designing → Developing → Completed).
- **💳 Token & UPI Payment Integration**:
  - Dual-tier token deposit flow (₹99 Standard / ₹199 Priority queue locks).
  - Dynamic QR code generator and 1-tap deep links for Google Pay, PhonePe, and Paytm.
- **👑 Admin Management Console (`admin.html`)**:
  - Live orders control board with status updater, budget editor, preview URL dispatcher, and token verifier.
  - Role-based admin access control, review moderation, and site metrics publisher.
- **📈 Live Analytics & Activity Stream (`analytics.html`)**:
  - Visual metrics, revenue charts, live project activity stream, and verified testimonial cards.
- **🤖 Integrated AI Assistant**:
  - Built-in technical query assistant powered by n8n workflow integration.

---

## 🗂️ Project Structure

```text
├── index.html              # Main customer portal (SPA homepage, ordering, tracker, reviews)
├── admin.html              # Administrator console & control panel
├── analytics.html          # Public / admin analytics dashboard & metrics
├── portfolio.html          # Work portfolio & showcase catalog
├── profile.html            # User account settings & profile management
├── documentation.html      # Platform documentation & user guide
├── faq.html                # Frequently asked questions & help center
├── INTEGRATION-GUIDE.html  # Developer API & Firebase integration guide
├── styles.css              # Shared editorial design system & utility tokens
├── sitemap.xml             # Search engine sitemap
├── robots.txt              # Search engine crawler policies
├── LICENSE                 # Custom Mandatory Attribution License
└── README.md               # Project documentation
```

---

## 🚀 Quick Start & Local Setup

1. **Clone the repository**:
   ```bash
   git clone https://github.com/your-username/codiv-web.git
   cd codiv-web
   ```

2. **Run locally**:
   Since CODIV is built using standard modern Web APIs, you can run it using any static HTTP server:

   *Using VS Code Live Server:*
   - Right-click `index.html` → **Open with Live Server**.

   *Using Node.js (`npx`):*
   ```bash
   npx serve Site-main
   ```

   *Using Python:*
   ```bash
   python -m http.server 8000
   ```

3. **Open in browser**:
   Navigate to `http://localhost:3000` (or `http://localhost:8000`).

---

## ⚙️ Configuration & Customization

### 1. Firebase Setup
Open `index.html`, `admin.html`, and `portfolio.html` to configure your Firebase Project credentials:
```javascript
const firebaseConfig = {
    apiKey: "YOUR_API_KEY",
    authDomain: "YOUR_PROJECT_ID.firebaseapp.com",
    databaseURL: "https://YOUR_PROJECT_ID-default-rtdb.firebaseio.com",
    projectId: "YOUR_PROJECT_ID",
    storageBucket: "YOUR_PROJECT_ID.appspot.com",
    messagingSenderId: "YOUR_SENDER_ID",
    appId: "YOUR_APP_ID"
};
```

### 2. Admin Access
In `index.html` and `admin.html`, update the `ADMIN_EMAILS` array with your authorized administrator emails:
```javascript
const ADMIN_EMAILS = [
    'admin@yourdomain.com'
];
```

### 3. Payment UPI Configuration
Update the default UPI ID and receiver name in `index.html`:
```javascript
const UPI_ID_DEFAULT = 'yourname@bank';
const UPI_NAME_DEFAULT = 'Your Business Name';
```

---

## 🌐 Deploying to the Web

### Deploying to Cloudflare / Workers
This site is configured for deployment to Cloudflare at [https://codiv.codiv.workers.dev/](https://codiv.codiv.workers.dev/).

### Deploying to GitHub Pages
1. Go to your repository on GitHub.
2. Navigate to **Settings** → **Pages**.
3. Under **Build and deployment** → **Source**, select `Deploy from a branch`.
4. Choose the `main` branch and `/Site-main` folder (or root).
5. Click **Save**.

### Deploying to Vercel
1. Import your GitHub repository on [Vercel](https://vercel.com).
2. Set Root Directory to `Site-main`.
3. Click **Deploy**.

### Deploying to Netlify
1. Drag and drop the `Site-main` folder into [Netlify Drop](https://app.netlify.com/drop) or connect your GitHub repository.
2. Set publish directory to `Site-main`.
3. Click **Deploy Site**.

---

## 📄 License & Mandatory Attribution

This project is protected under the **CODIV Attribution & Source-Available License** — see the [LICENSE](LICENSE) file for complete legal terms.

### Terms for Any Use or Fork:
1. **Mandatory Name & Logo**: Any deployment, fork, or public use **MUST** retain and visibly display the **CODIV** name and official logo in the user interface.
2. **Attribution & Backlink**: A visible link directing to [https://codiv.codiv.workers.dev/](https://codiv.codiv.workers.dev/) stating *"Powered by CODIV"* or *"Built with CODIV"* is required.
3. **No White-Labeling**: Removing, altering, or hiding author credits, trademarks, or logo assets from the UI or code is strictly prohibited.
