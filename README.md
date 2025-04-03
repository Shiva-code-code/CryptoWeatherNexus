# CryptoWeather Nexus

CryptoWeather Nexus is a modern dashboard that displays live cryptocurrency prices, weather data, and crypto news, with real-time notifications using WebSocket. Built with Next.js, React, Redux, and Tailwind CSS, it’s fast, responsive, and practical.

---

## 📌 Overview

- **Framework:** Next.js 13+
- **Frontend:** React with Hooks
- **Styling:** Tailwind CSS
- **State Management:** Redux Toolkit (with Thunks)
- **Live Data:** CoinGecko, OpenWeatherMap, NewsData.io
- **WebSocket:** CoinCap (live crypto prices), mock alerts for weather

---

## 🚀 Features

- Real-time cryptocurrency prices, 24h change, market cap
- Current weather data for major cities
- Crypto news headlines from NewsData.io
- Crypto and city detail pages with history
- Live WebSocket-based price/weather alerts
- Favorite cities and cryptos
- Fully responsive layout

---

## ⚙️ Setup & Installation

### 1. Clone the repo
```bash
git clone https://github.com/yourusername/crypto-weather-nexus.git
cd crypto-weather-nexus
2. Install dependencies
bash
Copy
Edit
npm install
3. Add environment variables
Create a .env.local file:

ini
Copy
Edit
NEXT_PUBLIC_CRYPTO_API_KEY=your_crypto_key
NEXT_PUBLIC_WEATHER_API_KEY=your_weather_key
NEXT_PUBLIC_NEWS_API_KEY=your_newsdata_key
NEXT_PUBLIC_WEBSOCKET_URL=wss://ws.coincap.io/prices?assets=bitcoin,ethereum
4. Start the dev server
bash
Copy
Edit
npm run dev
Visit: http://localhost:3000

📁 Folder Structure
bash
Copy
Edit
src/
├── app/
├── components/
├── lib/api/
├── redux/
└── styles/
🔌 APIs Used
CoinGecko – Crypto prices

OpenWeatherMap – Weather data

NewsData.io – Crypto news

CoinCap WebSocket – Live crypto updates

🔔 Real-Time Notifications
BTC/ETH prices update live using WebSocket

Weather alerts simulated via custom dispatch

Notifications handled via Redux & shown as toasts

🌐 Routing
/ – Dashboard (Weather, Crypto, News)

/crypto/[id] – Crypto detail page

/city/[name] – City weather detail page

📦 Deployment
Deployed on Vercel

All API keys managed with .env.local

🧠 Challenges Solved
API rate limiting handled via retry + caching

SSR-compatible deep links for detail pages

Responsive design with Tailwind CSS

Mock WebSocket events for weather alerts

📄 Assignment Scope
Multi-page dashboard (Weather, Crypto, News)

Detail pages with history/charts

Real-time updates via WebSocket

Favorites & local storage state

Public GitHub + deployed site

