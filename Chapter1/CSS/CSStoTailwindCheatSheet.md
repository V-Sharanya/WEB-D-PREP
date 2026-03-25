
---

# 📘 1. CSS → Tailwind Conversion Cheat Sheet

---

## 🔹 Layout & Display

| CSS                     | Tailwind       |
| ----------------------- | -------------- |
| `display: flex`         | `flex`         |
| `display: grid`         | `grid`         |
| `display: block`        | `block`        |
| `display: inline-block` | `inline-block` |
| `display: none`         | `hidden`       |

---

## 🔹 Flexbox

| CSS                              | Tailwind                         |
| -------------------------------- | -------------------------------- |
| `justify-content: center`        | `justify-center`                 |
| `justify-content: space-between` | `justify-between`                |
| `align-items: center`            | `items-center`                   |
| `flex-direction: column`         | `flex-col`                       |
| `gap: 10px`                      | `gap-2` (≈8px), `gap-3`, `gap-4` |

---

## 🔹 Grid

| CSS                                    | Tailwind      |
| -------------------------------------- | ------------- |
| `grid-template-columns: repeat(3,1fr)` | `grid-cols-3` |
| `gap: 20px`                            | `gap-5`       |
| `grid-column: span 2`                  | `col-span-2`  |

---

## 🔹 Spacing (VERY IMPORTANT)

| CSS                 | Tailwind |
| ------------------- | -------- |
| `margin: 10px`      | `m-2`    |
| `margin-top: 20px`  | `mt-5`   |
| `padding: 16px`     | `p-4`    |
| `padding-left: 8px` | `pl-2`   |

👉 Scale:

* `1 = 4px`
* `2 = 8px`
* `4 = 16px`

---

## 🔹 Width & Height

| CSS             | Tailwind    |
| --------------- | ----------- |
| `width: 100%`   | `w-full`    |
| `width: 50%`    | `w-1/2`     |
| `height: 100vh` | `h-screen`  |
| `height: 200px` | `h-[200px]` |

---

## 🔹 Typography

| CSS                  | Tailwind      |
| -------------------- | ------------- |
| `font-size: 1rem`    | `text-base`   |
| `font-size: 24px`    | `text-xl`     |
| `font-weight: bold`  | `font-bold`   |
| `text-align: center` | `text-center` |
| `font-family: serif` | `font-serif`  |

---

## 🔹 Colors

| CSS                  | Tailwind          |
| -------------------- | ----------------- |
| `color: red`         | `text-red-500`    |
| `background: blue`   | `bg-blue-500`     |
| `border-color: gray` | `border-gray-300` |

---

## 🔹 Borders

| CSS                   | Tailwind       |
| --------------------- | -------------- |
| `border: 1px solid`   | `border`       |
| `border-radius: 10px` | `rounded-lg`   |
| `border-radius: 50%`  | `rounded-full` |

---

## 🔹 Shadows

| CSS          | Tailwind                 |
| ------------ | ------------------------ |
| `box-shadow` | `shadow-md`, `shadow-lg` |

---

## 🔹 Position

| CSS                  | Tailwind   |
| -------------------- | ---------- |
| `position: relative` | `relative` |
| `position: absolute` | `absolute` |
| `top: 0`             | `top-0`    |
| `z-index: 10`        | `z-10`     |

---

## 🔹 Overflow

| CSS                | Tailwind          |
| ------------------ | ----------------- |
| `overflow: hidden` | `overflow-hidden` |
| `overflow-x: auto` | `overflow-x-auto` |

---

## 🔹 Effects

| CSS                     | Tailwind          |
| ----------------------- | ----------------- |
| `transition: all 0.3s`  | `transition`      |
| `transform: scale(1.1)` | `hover:scale-110` |
| `opacity: 0.5`          | `opacity-50`      |

---

## 🔹 Responsive Design

| CSS                         | Tailwind |
| --------------------------- | -------- |
| `@media (min-width:768px)`  | `md:`    |
| `@media (min-width:1024px)` | `lg:`    |

Example:

```html
<div class="text-sm md:text-lg lg:text-xl">
```

---

## 🔹 Hover / States

| CSS      | Tailwind |
| -------- | -------- |
| `:hover` | `hover:` |
| `:focus` | `focus:` |

```html
<button class="hover:bg-blue-700">
```

---

## 🔹 Special Utilities

| Purpose          | Tailwind                                    |
| ---------------- | ------------------------------------------- |
| Center div       | `flex justify-center items-center`          |
| Full page center | `h-screen flex items-center justify-center` |
| Hide on mobile   | `hidden md:block`                           |

---


## Font Sizes

text-xs: 0.75rem (12px)
text-sm: 0.875rem (14px)
text-base: 1rem (16px) — Default
text-lg: 1.125rem (18px)
text-xl: 1.25rem (20px)
text-2xl: 1.5rem (24px)
text-3xl: 1.875rem (30px)
text-4xl: 2.25rem (36px)
text-5xl: 3rem (48px)
text-6xl: 3.75rem (60px)
text-7xl: 4.5rem (72px)
text-8xl: 6rem (96px)
text-9xl: 8rem (128px) 

---