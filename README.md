# 🚕 AutoMeter Pro: Your Digital Fare Companion

> **Transparency in every turn. Accuracy in every meter.**

AutoMeter Pro is a cutting-edge, mobile-first web application designed to bring transparency and trust to auto-rickshaw rides across India. Whether you are a passenger tired of fare disputes or a driver looking for a professional digital dashboard, AutoMeter Pro has you covered.

---

## ✨ Key Features

### 📍 Real-Time GPS Tracking
Watch your journey unfold on a live map. Our high-precision tracking calculates distance to the decimal, ensuring you only pay for the path you actually travel.

### 💰 Multi-City Fare Engine
Pre-configured with official RTO fare rules for:
- **Pune** 🏛️
- **Mumbai** 🌊
- **Bangalore** 🌳
*Switch cities instantly with a single tap.*

### 🔗 Live Ride Sharing
Safety first! Generate a secure, encrypted link of your live route and share it with friends or family. They can track your path, current fare, and estimated arrival without needing an account.

### 🌓 Dual Modes: Passenger & Driver
- **Passenger Mode:** Focus on fare transparency, ride history, and route verification.
- **Driver Mode:** A professional toolkit including an earnings dashboard, daily summaries, and a custom **QR Code Sticker** for passengers to scan and track.

### 📱 Mobile-First, Desktop-Ready
Designed with a "Mobile-Frame" aesthetic on desktop, ensuring a consistent and focused experience across all devices.

### 💾 Offline-First Architecture
Uses **IndexedDB (Dexie)** to store your ride history locally. Your data stays on your device, ensuring privacy and lightning-fast performance even with spotty internet.

---

## 🛠️ Tech Stack

- **Frontend:** [React 19](https://react.dev/) + [Vite](https://vitejs.dev/)
- **Styling:** [Tailwind CSS 4.0](https://tailwindcss.com/) (Utility-first magic)
- **Animations:** [Motion](https://motion.dev/) (Silky smooth transitions)
- **Maps:** [Leaflet](https://leafletjs.com/) & [React Leaflet](https://react-leaflet.js.org/)
- **Database:** [Dexie.js](https://dexie.org/) (Local IndexedDB wrapper)
- **Icons:** [Lucide React](https://lucide.dev/)
- **Analytics:** [Vercel Analytics & Speed Insights](https://vercel.com/analytics)

---

## 🚀 Getting Started

### Local Development

1. **Clone & Enter:**
   ```bash
   git clone <your-repo-url>
   cd autometer-pro
   ```

2. **Install the Magic:**
   ```bash
   npm install
   ```

3. **Ignite the Engine:**
   ```bash
   npm run dev
   ```
   Open [http://localhost:3000](http://localhost:3000) and allow location permissions!

### Deployment
This project is optimized for **Vercel**. Simply push your code to GitHub and link it to Vercel. The included `vercel.json` handles all the routing for you.

---

## 🧠 How It Works (The "Secret Sauce")

### The Fare Algorithm
We don't just multiply distance by rate. Our engine accounts for:
1. **Base Fare:** The minimum charge for the first 1.5km.
2. **Per-Km Rate:** Calculated dynamically after the base distance.
3. **Waiting Charges:** Automatically detects when you are stuck in traffic and adds waiting time to the fare.
4. **Night Charges:** (Coming Soon) Automatic adjustment for late-night rides.

### URL-Encoded Sharing
The "Share Ride" feature uses **Google's Polyline Algorithm** to compress your entire GPS path into a short string. This string is passed via URL parameters, allowing the recipient to reconstruct your route without us ever storing your live location on a central server. **Privacy by Design.**

---

## 🗺️ Roadmap

- [ ] **Night Fare Toggle:** Automatic 25% increase for 11 PM - 5 AM rides.
- [ ] **Voice Alerts:** Audio announcements for fare milestones.
- [ ] **PDF Invoices:** Generate professional receipts for business travelers.
- [ ] **Language Support:** Hindi, Marathi, and Kannada translations.

---

## 🤝 Contributing
Found a bug or have a feature idea? Open an issue or submit a PR. Let's make urban commuting better for everyone!

## 📄 License
MIT License - Feel free to use and remix!

---
*Built with ❤️ for the Indian Commuter.*
