# MiniKart Deployment Guide

This guide provides step-by-step instructions to deploy MiniKart to production.

---

## 1. Database Setup (MongoDB Atlas)

1. Sign up / Log in to [MongoDB Atlas](https://www.mongodb.com/cloud/atlas).
2. Create a new Cluster.
3. Under **Database Access**, create a user with readWrite permissions.
4. Under **Network Access**, add `0.0.0.0/0` (allow access from anywhere).
5. Copy your connection string:
   `mongodb+srv://<username>:<password>@cluster.mongodb.net/minikart?retryWrites=true&w=majority`

---

## 2. Backend Deployment (Render / Railway)

### Deploying on Render:
1. Create a new **Web Service** on Render connected to your GitHub repo.
2. Set **Root Directory** to `backend`.
3. Set **Build Command**: `npm install`
4. Set **Start Command**: `npm start`
5. Add Environment Variables:
   - `MONGODB_URI`: Your MongoDB Atlas URI
   - `JWT_SECRET`: A secure random secret phrase
   - `RAZORPAY_KEY_ID`: Your Razorpay Key ID
   - `RAZORPAY_KEY_SECRET`: Your Razorpay Key Secret
6. Deploy service. Note down the backend URL (e.g. `https://minikart-backend.onrender.com`).

---

## 3. Frontend Deployment (Vercel / Netlify)

### Deploying on Vercel:
1. Import your GitHub repository to Vercel.
2. Set **Root Directory** to `frontend`.
3. Framework Preset: **Vite**.
4. Set Build Settings:
   - Build Command: `npm run build`
   - Output Directory: `dist`
5. Deploy project.

---

## 4. Razorpay Live Key Configuration

1. Log into your [Razorpay Dashboard](https://dashboard.razorpay.com).
2. Switch to **Live Mode**.
3. Generate API Key & Secret under **API Keys**.
4. Update `RAZORPAY_KEY_ID` and `RAZORPAY_KEY_SECRET` in your backend deployment environment variables.
