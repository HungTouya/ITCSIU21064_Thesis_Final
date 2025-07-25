# ITCSIU21064_Thesis_Final — Personalized Meal Planning and Cooking Assistance for Diabetic Users
<img width="1918" height="872" alt="Home" src="https://github.com/user-attachments/assets/4aaa19d5-0e84-49f3-9b55-e67c31a1260f" />

## Thesis Goals and Objectives

This project develops a **web-based meal planning and cooking assistance platform** tailored for diabetic users. It offers expert-recommended and customizable meal plans supported by AI.

Users select their diabetes type in their profile. If they choose a meal unsuitable for their condition, the system provides a **warning message** with three options:
1. Proceed with the original meal
2. Choose a suitable alternative
3. Return to the menu

### Technologies Used:
- ReactJS
- Firebase (Firestore, Authentication, Storage)
- TailwindCSS
- Dialogflow (for AI chatbot)

### Key UI Features:
- Login & Health Quiz
- Personalized Homepage
- Expert & Custom Schedule Pages
- AI Chatbox for Meal Advice
- Warning Messages with Alternatives

## Download & Setup Instructions

Clone the project from the `main` branch:

```bash
git clone <your-repository-url>
cd ITCSIU21064_Thesis_Final
````

---

## Environment Requirements

Ensure the following software is installed:

* **Node.js** (version ≥ 16.x)
  Download it from: [https://nodejs.org/](https://nodejs.org/)

Check your installed versions:

```bash
node -v
npm -v
```

---

## ⚙️ Setup Steps

After navigating to the project folder, run the following commands:

```bash
# Step 1: Install all dependencies (automatically creates node_modules)
npm install

# Step 2: Install Firebase and React Router DOM
npm install firebase react-router-dom

# Step 3: Install TailwindCSS
npm install -D tailwindcss postcss autoprefixer
npx tailwindcss init -p
```

> Note: The `node_modules` folder is not included in the Git repository.
> Running `npm install` will automatically generate it based on `package.json`.

---

## TailwindCSS Configuration

Update the `tailwind.config.js` file as follows:

```js
module.exports = {
  content: [
    "./src/**/*.{js,jsx,ts,tsx}",
  ],
  theme: {
    extend: {},
  },
  plugins: [],
}
```

In `src/index.css` or `src/App.css`, make sure the following lines are included:

```css
@tailwind base;
@tailwind components;
@tailwind utilities;
```

---

## Running the Application

To start the development server:

```bash
npm start
```

> ✅ **Important:**
> If the app opens on a screen that is **not the login page**, please click the **"Logout"** button to return to the login screen.
> From there, you can **create a new account or log in** using Firebase Authentication.


