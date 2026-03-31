# 🧪 8. Practice Tasks (Progressive 🚀)

## 🟢 Beginner

1. Show:

   * User name
   * Email

```javascript
li.innerText = user.name + " - " + user.email;
```

---

2. Clear previous data before loading again

```javascript
userList.innerHTML = "";
```

---

## 🟡 Intermediate

3. Add **Loading text**

👉 Before fetch:

```javascript
userList.innerHTML = "Loading...";
```

👉 After data:

```javascript
userList.innerHTML = "";
```

---

4. Handle errors properly

```javascript
try {
  // fetch
} catch(err) {
  userList.innerHTML = "Failed to load users";
}
```

---

## 🔴 Advanced (Mini Project Level)

5. Add **Delete button for each user**

👉 Each `<li>` should have:

* Name
* Delete button

---

6. Show:

* Name
* Email
* City
 
---

7. Convert list into **cards UI**

---

8. Add search filter:

* Input box
* Filter users by name

---