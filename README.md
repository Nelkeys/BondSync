# 💞 BondSync — A Simple Relationship Tracker for Couples

**BondSync** is a web-based relationship tracking system that helps couples build better emotional awareness and connection. It allows two users to link their accounts, receive thoughtful reminders, and log emotional check-ins — all without needing AI or a therapist.

---

## 🌟 Features

- 🔗 Couple account linking via email or code  
- 🔔 Scheduled prompts and gentle reminders  
- 📊 Emotion check-in logs  
- 📅 Weekly summary dashboard  
- 📨 Email notifications (via free service)  
- ☁️ Built with Firebase (authentication & database)  
- ⚡ Deployed on Vercel  

---

## 🛠️ Tech Stack

- **Frontend:** React.js + Tailwind CSS  
- **Backend:** Firebase Authentication + Firestore Database  
- **Email Notifications:** EmailJS (or similar free service)  
- **Hosting:** Vercel  

---

## 🧱 Folder Structure

```
src/
├── components/
│   ├── Auth/
│   ├── Dashboard/
│   ├── CheckIn/
│   └── Shared/
├── pages/
│   ├── Home.jsx
│   ├── Login.jsx
│   ├── Signup.jsx
│   ├── ConnectPartner.jsx
│   └── Dashboard.jsx
├── services/
│   ├── firebase.js
│   ├── email.js
│   └── prompts.js
├── styles/
│   └── tailwind.config.js
└── App.jsx
```

---

## 🚀 Getting Started

### 1. Clone the Repo

```bash
git clone https://github.com/your-username/bondsync.git
cd bondsync
```

### 2. Install Dependencies

```bash
npm install
```

### 3. Configure Firebase

- Create a Firebase project at [firebase.google.com](https://firebase.google.com)  
- Enable **Email/Password Auth**  
- Create a **Firestore** database  
- Copy your config keys to `src/services/firebase.js`

```js
// firebase.js
export const firebaseConfig = {
  apiKey: "YOUR_KEY",
  authDomain: "YOUR_APP.firebaseapp.com",
  projectId: "YOUR_APP",
  ...
};
```

### 4. Configure EmailJS (or another email service)

- Go to [EmailJS](https://emailjs.com) and create a free account  
- Setup an email template and get your `SERVICE_ID`, `TEMPLATE_ID`, and `USER_ID`  
- Store in `src/services/email.js`  

---

## 🧪 Running Locally

```bash
npm run dev
```

---

## 🌍 Deployment (Vercel)

- Push your repo to GitHub  
- Connect it to [Vercel](https://vercel.com)  
- Set up your Firebase and EmailJS environment variables on Vercel  
- Deploy!

---

## 🔐 Environment Variables

```
VITE_FIREBASE_API_KEY=
VITE_FIREBASE_AUTH_DOMAIN=
VITE_FIREBASE_PROJECT_ID=
VITE_EMAILJS_SERVICE_ID=
VITE_EMAILJS_TEMPLATE_ID=
VITE_EMAILJS_USER_ID=
```

---

## 📃 License

MIT License

---

## ❤️ Acknowledgments

- Firebase for free auth & DB  
- EmailJS for easy email integration  
- You, for building tech that helps people love better
