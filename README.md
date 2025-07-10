# 🥗 Nutrition Experts Platform – Documentation

A React-based web application connecting users with certified nutrition experts. Users can search for experts, view detailed profiles, and book consultation slots. Experts can register, manage appointments, and engage with clients. AI-powered coaching and community features enhance the overall wellness experience.

---

## 📌 Table of Contents

- [Overview](#overview)
- [Features](#features)
- [Technical Architecture](#technical-architecture)
- [Authentication System](#authentication-system)
- [User Roles](#user-roles)
- [Core Modules](#core-modules)
- [Integrations](#integrations)
- [Setup & Development](#setup--development)
- [Deployment](#deployment)
- [Security & Optimization](#security--optimization)
- [Future Enhancements](#future-enhancements)

---

## 🧭 Overview

The Nutrition Experts Platform connects individuals with professional nutritionists and AI wellness coaches. Whether it's booking a consultation, logging health metrics, or receiving personalized advice, users are supported through every step of their wellness journey.

---
👉 **[Click here to view the live site](https://theelefit.netlify.app/)**

## 🚀 Features

### For Users
- Search and book expert consultations
- View detailed expert profiles
- Access personalized AI coaching
- Join communities and participate in discussions

### For Experts
- Create and manage professional profiles
- Schedule appointments and manage bookings
- Analyze performance and user engagement
- Receive real-time Email notifications
- Integrate with Google Calendar

### For Admins
- Provided a admin dashboard.
- Manage users and expert applications
- Track the users and experts Progress

---

## 🛠️ Technical Architecture

### Frontend
- React.js for UI
- React Router for navigation
- CSS for styling
- Real-time Firebase SDK Integration

### Backend
- Firebase Authentication
- Cloud Firestore
- Firebase Cloud Storage
- Flask API for AI Coaching
- Redis for caching

---

## 🔐 Authentication System

- **Dual Auth Integration**: Shopify + Firebase  
- **User Sync**: All Shopify customers are also Firebase users  
- **Single Sign-On Flow**: Authenticate once, access everywhere  

### Flow Summary
- New users register → Shopify account + Firebase user created  
- On login → Validate with Shopify → Sync to Firebase  
- Fallback and recovery flows for partial failures

---

## 👥 User Roles

| Role  | Capabilities                                  |
|-------|-----------------------------------------------|
| User  | Booking, Coaching, Tracking, Community        |
| Expert| Scheduling, Analytics, Notifications          |
| Admin | Manage users, Approve experts, Access analytics |

---

## 📚 Core Modules

### 🔎 Expert Discovery & Booking
- Smart filters by name/specialty
- Profile deep-dive with credentials and availability
- Real-time slot booking

### 🤖 AI Coach
- Personalized plans and tips
- Generates meal and workout based on user profile.
- Generates meal[Breakfast,lunch,snack,dinner] and workout plan.
- PDF generation with embedded coach tips

### 👥 Community
- Content sharing
- Social interactions and moderation



## ⚙️ Setup & Development

### Prerequisites
- Node.js and npm installed
- Firebase and Shopify credentials configured

### Install & Run
```bash
git clone <repo-url>
cd nutrition-experts-platform
npm install
npm start

```
### PROJECT STRUCTURE
```
src/
├── components/          # Reusable UI parts
├── pages/               # Page-specific components
├── services/            # Shopify, Firebase integrations
├── data/                # Mock/demo data
├── App.js               # App routing
└── index.js             # Entry point
```

### Environment Variables (.env)
```
REACT_APP_FIREBASE_API_KEY=***
REACT_APP_FIREBASE_AUTH_DOMAIN=***
REACT_APP_FIREBASE_PROJECT_ID=***
REACT_APP_SHOPIFY_ACCESS_TOKEN=***
REACT_APP_OPENAI_API_KEY=***
REACT_APP_GOOGLE_CALENDAR_API_KEY=***
```

### 🚀 Deployment
Build & Deploy

```
npm run build
firebase deploy

```

###🧪 Testing
      - Component & unit testing
      - Integration & API testing
      - End-to-end testing with user scenarios


### 🛡️ Security & Optimization
  - Role-based access
  - Protected APIs & endpoints
  - Input sanitization & file validation
  - Data encryption
  - Performance
  - Code splitting
  - Lazy loading
  - Image and bundle optimization
  - Caching strategies
 
### 🔮Future Enhancements
   - GPT-powered 24/7 chat
   - Voice-based logging and reminders
   - Mini challenges (e.g., "7-Day Sugar-Free Streak")
   - XP points, leveling, and leaderboards
   - Social clubs for users (e.g., "Yoga Tribe", "Shred Squad")
   - QR codes for daily workouts or recipes for showing demo.
   - Personalized “Coach Tip of the Day” in PDFs
   - Payment gateway integration
   - Secure messaging between users and experts
   

