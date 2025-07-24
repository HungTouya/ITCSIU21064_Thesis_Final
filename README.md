# ITCSIU21064_Thesis_Final — Personalized Meal Planning and Cooking Assistance for Diabetic Users
<img width="1918" height="872" alt="Home" src="https://github.com/user-attachments/assets/4aaa19d5-0e84-49f3-9b55-e67c31a1260f" />

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

Visit the app in your browser at: [http://localhost:3000](http://localhost:3000)

> ✅ **Important:**
> If the app opens on a screen that is **not the login page**, please click the **"Logout"** button to return to the login screen.
> From there, you can **create a new account or log in** using Firebase Authentication.


