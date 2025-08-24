# Interview-Prep - Video Calling Interview Platform

---

## 📖 Introduction
**Interview-Prep** is a full-stack coding interview platform designed to facilitate **video/audio calls, screen sharing, and screen recordings**, all integrated with a **VS Code-like editor**.  

This platform is built for **companies**, allowing:
- **Candidates** to join calls, share their screen, and solve coding problems.  
- **Interviewers** to conduct structured interviews, add comments, and evaluate outcomes.  
- **Admins** to manage candidate results (mark as *failed* or *succeeded*).  

It supports **light and dark modes**, features a **responsive UI**, and is built using free-tier services—making it completely free to get started.

---

## ✨ Key Features

### 🔐 Authentication & User Management
- **Secure Authentication:** Login via **GitHub**, **Google**, or **email/password**.  
- **Role-Based Access:**  
  - By default, all users are **candidates**.  
  - Admins can assign roles (**candidate** or **interviewer**) from the dashboard.  

---

### 👨‍💻 Candidate Experience
- **Interview Dashboard:** View past, live, and upcoming interviews.  
- **Setup Page:** Configure and test camera/microphone before joining calls.  
- **Interactive Call Interface:**  
  - 🎥 **Live Video & Audio Calls** – Real-time communication  
  - 💻 **Code Editor** – VS Code-like editor (supports **JavaScript, Python, Java**)  
  - 📑 **Coding Problems** – With starter code  
  - 🎛️ **Call Actions:**  
    - Toggle camera/microphone  
    - Add reactions  
    - Share screen (single window / full screen)  
    - Record screen  
    - Change layout  
    - View participant list  
    - Leave the call  

---

### 🧑‍🏫 Interviewer Experience
- **Initiate Calls:** Start instant calls or join via link.  
- **Meeting Scheduling:**  
  - Create meetings with **title, description, candidate, multiple interviewers, date & time**  
  - Saved to **real-time database**  
  - Supports **1 candidate & multiple interviewers** per call  

- **Post-Interview Actions:**  
  - Add comments on candidates  
  - Mark outcome → **failed** / **succeeded**  

- **Call Control:**  
  - End call for everyone (as call owner)  

- **Recordings Access:**  
  - View past interview recordings directly from the dashboard  

---

### ⚙️ General Features
- **Real-time Updates:** Powered by **Convex** for instant data synchronization.  
- **Responsive UI:** Works seamlessly across devices.  
- **Light & Dark Mode:** Choose your preferred theme.  

---

## 🛠️ Technologies Used

- **Frontend Framework:** React with **Next.js (v14.2.23)**  
- **Styling:** Tailwind CSS + ShadCN UI Component Library  
- **Database:** **Convex** → real-time, type-safe backend with:  
  - Vector search  
  - Cron jobs  
  - File storage  
- **Authentication:** **Clerk Authentication** → pre-built UI + GitHub, Google, email/password sign-in  
- **Video/Audio Calls & Screen Sharing:** **Stream (GetStream.io) SDKs**  
  - Offers $100 free credit/month for production-grade video features  
- **Code Editor:** **Monaco Editor** (used by VS Code)  
- **Webhook Verification:** **Svix** – Verifies Clerk webhook events  
- **UI Components (ShadCN):**  
  - ResizablePanel  
  - ScrollArea  
  - Select  
  - Switch  
  - Calendar  
  - Textarea  
  - Dropdown Menu  
  - Avatar  
  - Badge  
- **Icons:** Lucid React icon library  
- **Notifications:** React Hot Toast  
- **Date Formatting:** date-fns  

---
