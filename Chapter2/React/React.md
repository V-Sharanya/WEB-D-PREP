
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

# ⚛️ React Basics & Vite Conventions

## 📌 Returning Elements in React

In React, a component must return **only one parent element**.

### ❌ Invalid

```jsx
return (
  <h1>Hello</h1>
  <p>World</p>
);
```

### ✅ Valid (using a wrapper)

```jsx
return (
  <div>
    <h1>Hello</h1>
    <p>World</p>
  </div>
);
```

### ✅ Valid (using Fragment)

```jsx
return (
  <>
    <h1>Hello</h1>
    <p>World</p>
  </>
);
```

👉 **Why Fragment (`<> </>`) ?**

* Avoids unnecessary `<div>` in DOM
* Keeps code clean and optimized

---

## ⚡ Vite + React Naming Conventions

When using Vite with React, follow these rules:

### 1. File Naming

* Use `.jsx` for React components

```
App.jsx
Header.jsx
```

### 2. Component Naming

* Component functions must start with a **capital letter**

### ❌ Wrong

```jsx
function header() {
  return <h1>Hello</h1>;
}
```

### ✅ Correct

```jsx
function Header() {
  return <h1>Hello</h1>;
}
```

👉 Reason:

* React treats lowercase as HTML tags
* Uppercase tells React it's a **custom component**

---

## 🧠 Additional Important Points

### 1. Always Import React (if needed)

In newer setups (like Vite + React 17+), you don’t need:

```jsx
import React from "react";
```

---

### 2. Use `export default`

```jsx
function App() {
  return <h1>Hello</h1>;
}

export default App;
```

---

### 3. Component Structure Best Practice

```jsx
import Header from "./Header";

function App() {
  return (
    <>
      <Header />
      <h1>Main App</h1>
    </>
  );
}

export default App;
```

---

### 4. Use `className` instead of `class`

```jsx
<div className="container"></div>
```

---

### 5. Self-closing Tags

```jsx
<input />
<img />
```

---

### 6. Props Example

```jsx
function Welcome(props) {
  return <h1>Hello {props.name}</h1>;
}
```

---

### 7. Folder Structure (Recommended)

```
src/
 ├── components/
 │    ├── Header.jsx
 │    └── Footer.jsx
 ├── App.jsx
 └── main.jsx
```

---

