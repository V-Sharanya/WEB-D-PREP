
---

# 📘 React Setup & Fundamentals Guide

## 🚀 1. Install Node.js using NVM

Follow these steps to install Node.js (recommended method using NVM):

```bash
# Download and install nvm
curl -o- https://raw.githubusercontent.com/nvm-sh/nvm/v0.40.4/install.sh | bash

# Load nvm (without restarting terminal)
\. "$HOME/.nvm/nvm.sh"

# Install Node.js (v24)
nvm install 24

# Verify Node.js version
node -v   # Expected: v24.14.1

# Verify npm version
npm -v    # Expected: 11.11.0
```

---

## 📖 2. React Documentation

* Official Docs: React → [https://react.dev/](https://react.dev/)

Use this as your **primary learning source**.

---

## 🧠 3. Background of React

* React was created at Meta (Facebook)
* Created by:
  ➤ Jordan Walke

### 👥 Core Contributors

* Andrew Clark
* Dan Abramov
* Jason Bonta
* Joe Savona
* Josh Story

---

## 💡 4. Why React Was Created

React was developed to solve issues like:

* **Phantom message problem in Facebook**
* Difficulty managing **real-time UI updates**
* Complex DOM manipulation

👉 Solution: **Efficient UI updates using Virtual DOM**

---

## ⚖️ 5. Library vs Framework

| Feature     | Library (React)      | Framework               |
| ----------- | -------------------- | ----------------------- |
| Control     | You control the flow | Framework controls flow |
| Flexibility | High                 | Less flexible           |
| Rules       | Minimal              | Strict rules            |
| Example     | React                | Angular, Django         |

👉 React is a **library**, not a framework.

---

## ⚙️ 6. Creating a React App

### 🔹 Method 1: Create React App (CRA)

```bash
npx create-react-app <app-name>
```

❌ Downsides:

* Slow
* Heavy (bulky setup)

### 🧹 Files You Can Delete (CRA)

Inside `src/`:

* `setupTests.js`
* `reportWebVitals.js`
* `logo.svg`
* `App.test.js`
* `App.css`
* `index.css`

---

### 🔹 Method 2: Vite (Recommended ⚡)

```bash
npm create vite@latest
```

✅ Advantages:

* Faster
* Lightweight
* Modern setup

### 🧹 Files You Can Delete (Vite)

* `assets/` (if not needed)
* All default CSS files

---

