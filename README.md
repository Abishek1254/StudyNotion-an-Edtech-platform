# StudyNotion 🎓

StudyNotion is a full-stack EdTech platform built with the MERN stack. It supports student and instructor workflows such as authentication, course creation, media handling, and course consumption through a React frontend and an Express/MongoDB backend.

## 🛠️ Tech Stack

- Frontend: React, Redux Toolkit, Tailwind CSS
- Backend: Node.js, Express.js
- Database: MongoDB
- Authentication: JWT
- Media Storage: Cloudinary
- Payments: Razorpay

## 📂 Project Structure

This repository contains the actual application inside the `studynotion-edtech-project-main` folder.

```text
StudyNotion/
|-- README.md
`-- studynotion-edtech-project-main/
    |-- package.json                  # Frontend package and root dev scripts
    |-- tailwind.config.js
    |-- prettier.config.js
    |-- public/                       # Static frontend assets
    |-- src/                          # React application source
    |   |-- assets/                   # Images, logos, and media
    |   |-- components/               # Shared and feature-based UI components
    |   |-- data/                     # Static app data
    |   |-- hooks/                    # Custom React hooks
    |   |-- pages/                    # Route-level pages
    |   |-- reducer/                  # Root reducer setup
    |   |-- services/                 # API config and async operations
    |   |-- slices/                   # Redux slices
    |   |-- utils/                    # Utility helpers
    |   |-- App.jsx
    |   `-- index.js
    |-- server/                       # Express backend
    |   |-- config/                   # Database, Cloudinary, and Razorpay config
    |   |-- controllers/              # Route controllers
    |   |-- mail/templates/           # Email templates
    |   |-- middleware/               # Auth middleware
    |   |-- models/                   # Mongoose models
    |   |-- routes/                   # API routes
    |   |-- utils/                    # Backend utilities
    |   |-- index.js
    |   |-- package.json
    |   `-- README.md
    |-- build/                        # Production frontend build output
    `-- node_modules/                 # Installed dependencies
```

## 🚀 Features
- 🔐 **User Authentication & Authorization**  
  - Secure sign-up and login using **JWT (JSON Web Tokens)**.  
  - Personalized dashboards for **students** and **instructors**.  
- 📚 **Course Management**  
  - Instructors can **create, upload, and manage** courses.  
  - Role-based system (**Student / Instructor**) for efficient content handling.  
- 🎥 **Media Uploads**  
  - Integrated with **Cloudinary** for storing and managing high-quality images and videos.  
- ⚡ **Backend APIs**  
  - Built with **Node.js** and **Express.js**.  
  - Handles users, courses, and progress tracking.  
- 🗄️ **Database**  
  - **MongoDB** for managing user data, courses, and progress.

## Run Locally

From the project folder:

```bash
cd studynotion-edtech-project-main
npm install
npm run dev
```

- `npm start` runs the React frontend
- `npm run server` runs the backend from the `server` folder
- `npm run dev` starts both frontend and backend together

## Notes

- The main application code is inside `studynotion-edtech-project-main`, not at the repository root.
- `build/` and `node_modules/` are generated directories and are included above only to reflect the current structure present in this project folder.
