# 📄 **ASSIGNMENT: CSS + TAILWIND STYLING CHALLENGE**

---

## 🧾 **Title**

**Transform Semantic Blog Website into a Fully Styled Responsive UI using Tailwind + Flexbox + Grid**

---

## 🎯 **Objective**

To evaluate your ability to:

* Convert raw HTML into a **modern UI**
* Use **Flexbox & Grid properly**
* Apply **Tailwind utility classes effectively**
* Build **responsive layouts**
* Replace bad practices (like `float`) with modern CSS

---

## ⏱️ **Duration**

**2 Hours (Strict Time Limit)**

---

## ⚙️ **Instructions**

* Use your existing HTML file (no rewriting structure)
* You are allowed to:

  * Add classes
  * Slightly restructure layout (if needed)
* Use **Tailwind CSS only**

```html
<script src="https://cdn.tailwindcss.com"></script>
```

---

## 🚫 **Constraints (VERY STRICT)**

❌ No custom CSS file
❌ No inline CSS (`style=""`) → remove your `float` from aside
❌ No Bootstrap / other frameworks

✅ Only Tailwind classes
✅ Must use Flexbox + Grid

---

# 🏗️ **Task Breakdown (Based on YOUR HTML)**

---

## 🔹 **1. Header Styling**

Your current:

```html
<header>...</header>
```

### ✅ Convert into:

* Flex layout
* Space between logo & nav
* Add background + shadow

### 🎯 Requirements:

```html
flex justify-between items-center
```

### 💡 Expected:

* Sticky header (`sticky top-0`)
* Horizontal nav (no bullets)

---

## 🔹 **2. Sidebar Fix (IMPORTANT)**

Your current:

```html
aside style="float: left;"
```

👉 ❌ WRONG approach (old CSS)

### ✅ Convert into:

* Flex or Grid layout
* Sidebar + content side-by-side

### 🎯 Requirements:

* Sidebar width fixed
* Hidden on mobile

```html
hidden md:block
```

---

## 🔹 **3. Main Layout (CORE PART)**

Wrap `aside + section` inside:

```html
<div class="flex">
```

---

## 🔹 **4. Blog Articles Styling**

Each `<article>`:

### 🎯 Convert into cards:

```html
bg-white p-4 rounded-xl shadow-md mb-4
```

### Add:

* Proper spacing
* Image styling:

```html
w-full h-48 object-cover rounded-lg
```

### Bonus:

```html
hover:scale-105 transition
```

---

## 🔹 **5. Grid Layout for Articles**

Instead of stacking:

### 🎯 Use:

```html
grid grid-cols-1 md:grid-cols-2 gap-4
```

---

## 🔹 **6. Table Styling**

Your table is raw.

### 🎯 Convert:

```html
w-full bg-white rounded-xl shadow-md overflow-hidden
```

### Add:

```html
border-b p-2 text-left
```

### Wrap:

```html
overflow-x-auto
```

---

## 🔹 **7. Form Styling (IMPORTANT)**

### Inputs:

```html
w-full p-2 border rounded mb-2
```

### Button:

```html
bg-blue-500 text-white px-4 py-2 rounded hover:bg-blue-700
```

---

## 🔹 **8. Footer Styling**

### Add:

```html
text-center p-4 bg-white shadow-md mt-4
```

---

# 📱 **Responsive Requirements (MANDATORY)**

| Element  | Mobile   | Desktop      |
| -------- | -------- | ------------ |
| Sidebar  | Hidden   | Visible      |
| Articles | 1 column | 2 columns    |
| Layout   | Stacked  | Side-by-side |

---

# 🎨 **Design Guidelines**

Use:

* `bg-gray-100` → page background
* `shadow-md` → elevation
* `rounded-xl` → modern look
* `gap-4`, `p-4` → spacing

---

# 🧪 **Bonus (HIGHLY RECOMMENDED)**

* Highlight active nav:

```html
text-blue-500 font-semibold
```

* Add hover to links:

```html
hover:underline
```

* Add focus styles for inputs

---

# 📊 **Evaluation Criteria**

| Criteria            | Marks |
| ------------------- | ----- |
| Flexbox Usage       | 20    |
| Grid Usage          | 20    |
| Tailwind Efficiency | 20    |
| Responsiveness      | 20    |
| UI Quality          | 20    |

---

# 🧠 **Expected Outcome**

After this:

* Your project should look like a **real blog website**
* Not a plain HTML page

---
