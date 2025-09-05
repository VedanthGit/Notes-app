# 📒 Notes-App (MERN Stack)

A full-stack **Notes Management Application** built with the **MERN stack (MongoDB, Express, React, Node.js)**. Users can **create, update, delete, and pin notes** to organize their tasks effectively. Authentication ensures that each user’s notes remain private and secure.

## 🚀 Features
- 🔐 User Authentication (Signup/Login with JWT)  
- 📝 Create Notes with title & content  
- ✏️ Edit Notes easily  
- ❌ Delete Notes permanently  
- 📌 Pin Important Notes for quick access  
- 🔍 Search Notes by title/content  
- 🎨 Responsive UI with Tailwind CSS  

## 🛠️ Tech Stack
**Frontend:** React.js, Vite, React Router DOM, Tailwind CSS, Axios  
**Backend:** Node.js, Express.js, MongoDB, JWT Authentication, Mongoose  
**API Testing:** Postman  
**Version Control:** Git & GitHub  

## ⚙️ Installation & Setup

Follow these steps to run the project locally:

---

### 🔹 Frontend Setup (React + Vite + Tailwind)

#### 1. Navigate to the frontend folder
cd frontend

#### 2. Create a Vite React project
npm create vite@latest notes-app  
Select options:  
Framework: React  
Variant: JavaScript

#### 3. Move into the project folder, install dependencies, and start the dev server
cd notes-app
npm install
npm run dev

#### 4. Now stop the server (Ctrl + C) and create the folder structure inside src/:
src/  
├── assets/  
├── components/  
├── pages/  
└── utils/  

#### 5. Install Tailwind CSS (follow Vite setup guide):

#### 6. Install Tailwind and required dependencies
npm install -D tailwindcss postcss autoprefixer
npx tailwindcss init -p

#### 7. Install React Router DOM:
npm install react-router-dom

## Folder structure for frontend:
frontend/  
├── notes-app/  
│   ├── node_modules/  
│   ├── public/  
│   ├── src/  
│   │   ├── assets/  
│   │   │   └── (static files like images, icons etc.)  
│   │   ├── components/  
│   │   │   └── (reusable UI components)  
│   │   ├── pages/  
│   │   │   └── (page-level components like Home, Login, Register, etc.)  
│   │   ├── utils/  
│   │   │   └── (helper functions, axiosInstance, constants.js, etc.)  
│   │   ├── App.jsx  
│   │   ├── main.jsx  
│   │   └── index.css  
│   ├── package.json  
│   ├── vite.config.js  
│   └── tailwind.config.js  
___
### 🔹 Backend Setup (Node + Express + MongoDB)
#### 1. Go to a new terminal while running the frontend server and head to backend folder 
cd backend (mine is Notes-app/backend)

#### 2. Initialize backend project
npm init -y

#### 3. Install dependencies
npm install express mongoose jsonwebtoken dotenv cors nodemon

#### 4. Create index.js in the backend folder and set up basic Express server (http://localhost:8000).

#### 5. Create a .env file:
Create a .env file:

ACCESS_TOKEN_SECRET=your_generated_secret_key


#### Generate secret key:

node -e "console.log(require('crypto').randomBytes(64).toString('hex'))"

#### 6. Create config.json and add your MongoDB connection string.
#### 7. Create utilities.js for JWT helper functions.

## Folder structure for backend:
backend/  
├── index.js  
├── config.json  
├── utilities.js  
├── models/  
│   ├── user.model.js  
│   └── note.model.js  
└── .env  

### 🔹 API Integration & Utilities
#### Test backend routes with Postman (Add, Edit, Delete, Pin Notes, Get All Notes, Get User).

#### Install Axios in frontend:

npm install axios

#### Create constants.js in frontend:

export const BASE_URL = 'http://localhost:8000';

#### Create axiosInstance.js utility for requests.

### 🔹 Running the Project
#### Start backend server
cd backend  
npm start

#### Start frontend server
cd frontend/notes-app  
npm run dev


### ⚠️ Note: Both servers must run at the same time.

* If using WiFi, add your current IP address in MongoDB Atlas.

* If using mobile broadband/hotspot, set MongoDB access to 0.0.0.0/0 to avoid frequent network access errors (IP keeps changing).

## Open browser at:

http://localhost:5173

# 🤝 Contributing

Pull requests are welcome. For major changes, please open an issue first to discuss what you would like to change.

# 📜 License

This project is licensed under the MIT License.
