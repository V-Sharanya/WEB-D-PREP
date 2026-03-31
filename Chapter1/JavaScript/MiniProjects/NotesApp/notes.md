
---

# 🚀 Final Mini Project (Better Version)

## 🔥 **Notes Explorer (API + UI + Filtering)**

👉 This combines:

* DOM
* Events
* State
* Filtering
* **Fetch API (IMPORTANT)**
* UI (Tailwind)

---

# 🎯 What You Will Build

A Notes Viewer that:

* Fetches notes from API
* Displays them as cards
* Allows search + filter
* Allows delete + highlight

---

# 🌐 API to Use

```text
https://jsonplaceholder.typicode.com/posts
```

---

# 🧠 API Data Looks Like

```js
{
  userId: 1,
  id: 1,
  title: "sunt aut facere",
  body: "quia et suscipit..."
}
```

---

# 🧩 Features (Final Structure)

---

## 🟢 1. Fetch Notes

👉 Button:

```html
<button id="loadNotes">Load Notes</button>
```

👉 Behavior:

* Fetch posts
* Store in array

---

## 🟡 2. Display Notes (Card UI)

Each card:

```text
Title
Body
[⭐] [❌]
```

---

## 🔵 3. Highlight Note

👉 Toggle highlight using:

```js
classList.toggle()
```

---

## 🔴 4. Delete Note

👉 Remove from UI (and optionally from array)

---

## 🟣 5. Search Notes

👉 Input:

```html
<input id="search">
```

👉 Filter by:

* title
* body

---

## 🟠 6. User Filter (Advanced 🔥)

👉 Add dropdown:

```html
<select id="userFilter">
  <option value="all">All</option>
  <option value="1">User 1</option>
  ...
</select>
```

👉 Filter by:

```js
post.userId
```

---

## ⚫ 7. Loading + Error State

👉 Before fetch:

```js
list.innerHTML = "Loading..."
```

👉 Error:

```js
"Failed to load"
```

---

# 🧠 Required State

```js
let allPosts = [];
```

---

# 🧠 Functions You Should Write

```js
fetchPosts()
displayPosts(posts)
filterPosts()
toggleHighlight(id)
deletePost(id)
```

---

# 🧠 Mental Model (CRITICAL)

```text
Fetch → Store → Filter → Display
```

---



