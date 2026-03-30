
---

# 🚀 JavaScript Async Concepts + Fetch API (Practical Guide)

---

# 🌐 1. What is an API?

🔹 **API (Application Programming Interface)**
An API is a way for your frontend (JS) to **talk to a server** and get/send data.

👉 Think:

> “API = waiter between your app and the database”

### 🔸 Example API

```
https://jsonplaceholder.typicode.com/users
```

### 🔸 What it returns:

```json
[
  { "id": 1, "name": "Leanne Graham", "email": "..." }
]
```

📌 This is called a **REST API** → it gives data via URLs.

---

# 📦 2. Fetch API

🔹 Used to **request data from an API**

---

## 🔹 Basic Syntax (Promise-based)

```javascript
fetch("https://api.example.com/data")
  .then(response => response.json())
  .then(data => console.log(data))
  .catch(error => console.log(error));
```

---

## 🔹 Real Example

```javascript
fetch("https://jsonplaceholder.typicode.com/users")
  .then(res => res.json())
  .then(data => console.log(data));
```

---

## 🔹 Key Understanding

| Step            | What happens         |
| --------------- | -------------------- |
| fetch()         | Sends request        |
| response        | Raw response         |
| response.json() | Convert to JS object |
| data            | Usable data          |

---

# 🔁 3. Promises

🔹 A Promise represents **future result of async operation**

---

## 🔹 States

* **Pending** → waiting
* **Resolved** → success
* **Rejected** → error

---

## 🔹 Create Promise

```javascript
let promise = new Promise((resolve, reject) => {
  let success = true;

  if (success) resolve("Done!");
  else reject("Error!");
});
```

---

## 🔹 Use Promise

```javascript
promise
  .then(result => console.log(result))
  .catch(error => console.log(error));
```

---

# ⏳ 4. Async / Await (Important 🔥)

🔹 Cleaner way to write Promises

---

## 🔹 Syntax

```javascript
async function getData() {
  let response = await fetch("https://api.example.com/data");
  let data = await response.json();
  console.log(data);
}
```

---

## 🔹 With Error Handling (Best Practice)

```javascript
async function fetchUsers() {
  try {
    let res = await fetch("https://jsonplaceholder.typicode.com/users");
    let data = await res.json();
    console.log(data);
  } catch (err) {
    console.log("Error:", err);
  }
}
```

---

## 🔹 Flow (VERY IMPORTANT)

1. `await fetch()` → wait for response
2. `await res.json()` → convert data
3. Use data

👉 This is exactly what your project is doing

---

# 🔄 5. Connecting to Your Project

Your code:

```javascript
let response = await fetch("https://jsonplaceholder.typicode.com/users");
let data = await response.json();
```

Then:

```javascript
data.forEach(user => {
  let li = document.createElement('li');
  li.innerText = user.name;
  userList.appendChild(li);
});
```



---

# 🔍 6. Equality Operators

## = (Assignment)

```javascript
let x = 5;
```

## == (Loose Equality ❌)

```javascript
5 == "5" // true
```

## === (Strict Equality ✅)

```javascript
5 === "5" // false
```

👉 Rule:
**Always use `===`**

---

# 🧠 7. Mental Model (VERY IMPORTANT)

When working with APIs:

```
User clicks button
        ↓
JS sends request (fetch)
        ↓
Server sends response
        ↓
Convert response → JSON
        ↓
Loop through data
        ↓
Update UI (DOM)
```

---

# 🎯 9. Bonus: Types of API Requests

| Method | Use         |
| ------ | ----------- |
| GET    | Fetch data  |
| POST   | Send data   |
| PUT    | Update data |
| DELETE | Delete data |

---

