# mystudyspace


**MyStudySpace** is a full-stack web application to help students manage their study life. It features authentication, personal dashboard, and tools to manage courses and tasks.

## 🚀 Features

- 🔐 Authentication with **Email** and **Google** using NextAuth.js
- 🧠 Personalized dashboard after login
- 📚 Manage courses (Create / Read / Update / Delete)
- ✅ Manage tasks linked to each course (CRUD)
- 📅 Dashboard with daily quote and overview
- 🌗 Toggle button (dark/light mode)
- 📦 Deployed on Vercel

---

## 🛠 Tech Stack

- **Frontend**: Next.js 14 (App Router), React, TypeScript, CSS Modules
- **Backend**: Node.js, NextAuth.js
- **Database**: MongoDB Atlas with Mongoose
- **Styling**: Pure CSS (no Tailwind)
- **Auth Providers**: Google OAuth, Email (magic link)
- **Deployment**: Vercel

---

## ⚙️ Project Structure

```

my-study-space/
├── public/
├── src/
│   ├── app/
│   │   ├── api/
│   │   │   └── auth/
│   │   │       └── \[...nextauth]/route.ts
│   │   ├── dashboard/
│   │   ├── courses/
│   │   ├── tasks/
│   │   ├── signin/
│   │   ├── layout.tsx
│   │   ├── page.tsx
│   │   ├── globals.css
│   ├── lib/
│   │   └── mongodb.ts
├── .env.local
├── package.json
├── README.md

````

---

## 🧪 Installation & Setup

### 1. Clone the repo

```bash
git clone https://github.com/your-username/my-study-space.git
cd my-study-space
````

### 2. Install dependencies

```bash
npm install
```

### 3. Add environment variables

Create a `.env.local` file in the root directory and add:

```env
# MongoDB
MONGODB_URI=mongodb+srv://<user>:<password>@cluster.mongodb.net/myStudySpace

# NextAuth
NEXTAUTH_URL=http://localhost:3000
NEXTAUTH_SECRET=your-random-secret

# Google Auth
GOOGLE_CLIENT_ID=your-google-client-id
GOOGLE_CLIENT_SECRET=your-google-client-secret

# Email Auth (Gmail + App Password)
EMAIL_SERVER=smtp://your-email@gmail.com:your-app-password@smtp.gmail.com:587
EMAIL_FROM="MyStudySpace <your-email@gmail.com>"
```

> 🔑 Generate a strong secret:
> `openssl rand -base64 32` (or use an online generator)

### 4. Run the app locally

```bash
npm run dev
```

Visit: [http://localhost:3000](http://localhost:3000)

---



Ready to continue with the dashboard or CRUD part next?
```
