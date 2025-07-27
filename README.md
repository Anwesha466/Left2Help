# 🍲 Left2Help – Smart Leftover Exchange & Chat System for Local Food Vendors
*Left2Help* is a full-stack web application that empowers local street food vendors (like momo walas, chai walas, etc.) to *exchange leftover ingredients, **chat in real-time, and **reduce food waste*, all through a friendly, mobile-first interface.

> 💡 *Mission:* Reduce food waste, support local communities, and bring tech to the streets—literally!

---

## 🌟 Main Features
### 🛒 Ingredient Exchange Marketplace
- Post leftover ingredients with quantity, expiry, and location
- Discover nearby vendors (1–5 km radius filter)
- Add/remove listings anytime

### 💬 Chat System (ChatGPT-style)
- Real-time 1:1 vendor chat with full message history
- Timestamps and sender info
- Clear chat history feature

### 📞 Call Log & Records
- Logs for audio/video calls
- Track: who called whom, when, and for how long
- Option to clear call history

### 🔔 Notifications
- SMS/WhatsApp alerts for:
  - New ingredient listings nearby
  - Incoming chat messages

### 📱 PWA Support
- Works offline and can be installed on phones
- Optimized for low-end devices with limited bandwidth

---

## 🔐 Additional Features
- Hindi & English UI  
- Vendor Trust Score system  
- Weekly impact report: ₹ saved + waste reduced  
- Cold storage alerts (e.g., “Cabbage expiring in 2 hrs”)  
- AI Chatbot for tips like “How to store paneer?” or “Best momo chutney?” 😎

---

## 🧰 Tech Stack

| Part            | Tech Stack                       |
|-----------------|----------------------------------|
| *Frontend*    | React.js + Tailwind CSS          |
| *Backend*     | Node.js + Express.js             |
| *Notifications*| Twilio /                        |
| *PWA*         | React + Manifest + Service Worker|
| *Deployment*  | Replit Monorepo / GitHub Pages   |

---

## 🚀 Getting Started

### 1. Clone the Repo
```bash
git clone https://github.com/your-username/Left2Help.git
cd Left2Help

2. Install Dependencies
npm install
# or yarn install

3. Set Up Environment Variables
Create a .env file and include:
TWILIO_SID=your_twilio_sid
TWILIO_AUTH=your_twilio_auth_token
WHATSAPP_API_KEY=your_api_key

4. Run the App
npm run dev

---

📂 Folder Structure
.
├── client/              # React frontend
│   └── ...
├── server/              # Express backend
│   ├── routes/
│   ├── models/
│   └── ...
├── .replit
├── README.md
└── package.json
---

🌍 Real-World Impact
♻ Reduce daily food waste
💬 Build strong local communities
📱 Bring street vendors into the digital economy

---

🙌 Contributing
Pull requests are welcome! For major changes, please open an issue first to discuss what you’d like to change.

> Let's give momo bhaiya & chai didi a digital upgrade.
Tech for thadiwalas FTW! 🚲💻
