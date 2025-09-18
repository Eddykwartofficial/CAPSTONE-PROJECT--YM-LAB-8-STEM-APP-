# CAPSTONE PROJECT "YM LAB 8 STEM APP'
CAPSTONE PROJECT

# YM Lab 8 STEM Lab React App

A full-featured **STEM Education Lab website** built with **React (Vite)**, **Tailwind CSS**, **Framer Motion**, and **json-server** for a mock backend.

The app includes pages for **Home, Gallery, Programs, Projects & Awards, About, Donate, Login, Signup**, and integrates **state management with React Context**, **local storage authentication**, and **API fetching**.

---

## 📂 Project Structure

src/
├── App.jsx
├── main.jsx
├── context/
│ └── AppContext.jsx
├── components/
│ ├── Header.jsx
│ ├── Footer.jsx
│ ├── Container.jsx
│ └── Card.jsx
├── pages/
│ ├── HomePage.jsx
│ ├── GalleryPage.jsx
│ ├── ProgramsPage.jsx
│ ├── ProjectsAwardsPage.jsx
│ ├── AboutPage.jsx
│ ├── DonatePage.jsx
│ ├── LoginPage.jsx
│ ├── SignupPage.jsx
│ └── NotFound.jsx
└── services/
└── api.js


---

## ⚙️ Setup Instructions

### 1. Clone and install
```bash
git clone https://github.com/yourusername/stem-lab-app.git
cd stem-lab-app
npm install

2. Install dependencies
npm install react-router-dom axios framer-motion
npm install -D tailwindcss postcss autoprefixer
npx tailwindcss init -p

3. Configure Tailwind

In tailwind.config.js update content paths:

export default {
  content: ["./index.html", "./src/**/*.{js,jsx}"],
  theme: { extend: {} },
  plugins: [],
}


In src/index.css add:

@tailwind base;
@tailwind components;
@tailwind utilities;

4. Mock API with json-server

Create db.json at project root:

{
  "programs": [
    { "id": 1, "title": "Robotics Basics", "description": "Intro to building robots" }
  ],
  "projects": [
    { "id": 1, "title": "Drone Project", "year": 2023, "award": "Innovation Award" }
  ]
}


Run server:

npx json-server --watch db.json --port 4000

5. Start app
npm run dev

🚀 Features

HomePage — overview and highlights

GalleryPage — image showcase with hover animations

ProgramsPage — list of courses with add new course form (requires auth)

Projects & AwardsPage — achievements since 2022

DonatePage — bank & mobile money donate options

Login/Signup — localStorage authentication

Framer Motion — smooth animations & transitions

🛠️ Tech Stack

React (Vite) — fast dev environment

Tailwind CSS — styling framework

Framer Motion — animations

React Router — routing

Context API + Reducer — state management

Axios — API requests

json-server — mock REST API

🤝 Contributing

Fork the project

Create a feature branch (git checkout -b feature/new-feature)

Commit changes (git commit -m 'Add new feature')

Push to branch (git push origin feature/new-feature)

Open a Pull Request

📜 License

This project is licensed under the MIT License.
