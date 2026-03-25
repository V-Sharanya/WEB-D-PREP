# 📘 CSS3 + Tailwind 

## 🔹 1. CSS Box Model (VERY IMPORTANT)

```
Content → Padding → Border → Margin
```

```css
div {
  width: 200px;
  padding: 20px;
  border: 5px solid black;
  margin: 10px;
}
```

```css
box-sizing: border-box;
```

✔ Prevents layout breaking (used in all real projects)

---

## 🔹 2. Display Types (Expand your knowledge)


```css
display: block;
display: inline;
display: inline-block;
display: none;
```

👉 Key difference:

* `block` → takes full width
* `inline` → no width/height
* `inline-block` → best of both

---

## 🔹 3. Positioning 

```css
position: static;   /* default */
position: relative;
position: absolute;
position: fixed;
position: sticky;
```

👉 Important:

```css
top, left, right, bottom
z-index
```

---

## 🔹 4. Flexbox 

### Container properties:

```css
display: flex;
flex-direction: row | column;
justify-content: center | space-between | space-around;
align-items: center;
gap: 10px;
```

### Item properties:

```css
flex: 1;
align-self: center;
order: 1;
```

👉 Use for:

* Navbar
* Cards
* Centering elements

---

## 🔹 5. CSS Grid 

```css
display: grid;
grid-template-columns: repeat(3, 1fr);
grid-template-rows: auto;
gap: 10px;
```

### Placement:

```css
grid-column: span 2;
grid-row: span 2;
```

👉 Use for:

* Full layouts (dashboard, pages)

---

## 🔹 6. Responsive Design (IMPORTANT)

### Media Queries:

```css
@media (max-width: 768px) {
  body {
    background: red;
  }
}
```

👉 Common breakpoints:

* 480px → mobile
* 768px → tablet
* 1024px → laptop

---

## 🔹 7. Units 

```css
px      /* fixed */
%       /* relative */
em      /* parent-based */
rem     /* root-based */
vh/vw   /* viewport */
```

👉 MOST IMPORTANT:

* `rem` for fonts
* `vh/vw` for layouts

---

## 🔹 8. CSS Variables (Modern CSS)

```css
:root {
  --main-color: blue;
}

h1 {
  color: var(--main-color);
}
```

---

## 🔹 9. Transitions 

```css
transition: all 0.3s ease;
```

```css
button:hover {
  background: black;
  color: white;
}
```

---

## 🔹 10. Animations (CSS3)

```css
@keyframes slide {
  from { transform: translateX(0); }
  to { transform: translateX(100px); }
}

div {
  animation: slide 1s infinite;
}
```

---

## 🔹 11. Transform 

```css
transform: scale(1.2);
transform: rotate(45deg);
transform: translateX(50px);
```

---

## 🔹 12. Object Fit (for images)

```css
img {
  width: 100%;
  height: 200px;
  object-fit: cover;
}
```

---

## 🔹 13. Cursor & Visibility

```css
cursor: pointer;
visibility: hidden;
```

---

# 🎨 Tailwind CSS 

## 🔹 1. Utility First Concept

```html
<div class="bg-blue-500 text-white p-4 rounded">
```

---

## 🔹 2. Flex in Tailwind

```html
<div class="flex justify-center items-center">
```

---

## 🔹 3. Grid in Tailwind

```html
<div class="grid grid-cols-3 gap-4">
```

---

## 🔹 4. Responsive Tailwind

```html
<div class="text-sm md:text-lg lg:text-2xl">
```

---

## 🔹 5. Spacing

```html
p-4   m-2   mt-5   px-6
```

---

## 🔹 6. Colors

```html
bg-red-500
text-blue-700
```

---

## 🔹 7. Hover / Effects

```html
hover:bg-black hover:text-white
```

---

## 🔹 8. Important Tailwind Concepts 

* `container`
* `max-w-*`
* `shadow-*`
* `rounded-*`
* `flex-wrap`
* `overflow-hidden`
* `z-*`

---
🔥 What Tailwind Reset Does

It removes browser default styles like:

❌ Before (browser default styles)
<ul> → bullets
<h1> → big bold text
<a> → blue + underline
<table> → borders
<body> → margins

🧠 Key Concept (VERY IMPORTANT)

👉 Tailwind assumes:

“You will style EVERYTHING yourself”

So it removes all default styling.
---
