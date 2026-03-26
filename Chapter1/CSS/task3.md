
---

# 📄 **CHALLENGE: Stripe Pricing Section Clone**

---

## 🧾 **Title**

**Recreate Stripe Pricing UI using Tailwind CSS**

---

## 🎯 **Objective**

Master:

* Card layouts (real-world)
* Grid + Flex combination
* UI hierarchy
* Advanced styling (gradients, shadows)

---

## ⏱️ **Duration**

**1.5 Hours (Strict)**

---

# 🏗️ **Task Breakdown (STEP-BY-STEP)**

---

## 🔹 1. Top Heading

### 🎯 Build:

```
Pricing built for
businesses of all sizes
```

### Requirements:

```html
text-4xl font-bold text-gray-800
```

👉 Center or left aligned (your choice)

---

## 🔹 2. Pricing Cards Section (CORE)

You have **2 main cards**:

---

## 🟦 LEFT CARD (Standard)

### Layout:

* White card
* Rounded
* Shadow

```html
bg-white p-6 rounded-xl shadow-lg
```

---

### Inside structure:

#### Left side:

* Title: Standard
* Description
* Button

#### Right side:

* 2% (India)
* 3% (International)

👉 Use:

```html
grid grid-cols-2
```

---

---

## 🟪 RIGHT CARD (Custom)

### Style:

```html
bg-blue-900 text-white p-6 rounded-xl shadow-lg
```

---

### Inside:

* Title: Custom
* Description
* Button
* 3 stacked boxes:

```html
flex flex-col gap-2
```

Each box:

```html
bg-blue-800 p-3 rounded
```

---

---

## 🔹 3. Background Gradient (ADVANCED 🔥)

This is what makes UI look premium.

### Add behind cards:

```html
bg-gradient-to-r from-purple-500 via-pink-500 to-orange-400
```

👉 Place it in a wrapper div

---

---

## 🔹 4. Toggle Tabs (Small UI Element)

```
Standard pricing | Custom pricing | FAQs
```

### Style:

```html
flex gap-4 bg-white p-2 rounded-full shadow-md
```

---

---

## 🔹 5. Features Section (BOTTOM GRID)

### Layout:

```html
grid grid-cols-1 md:grid-cols-2 lg:grid-cols-4 gap-6
```

Each feature:

* Icon (optional)
* Title
* Bullet points

---

---

# 📱 **Responsive Requirements**

| Screen  | Behavior       |
| ------- | -------------- |
| Mobile  | Stack cards    |
| Tablet  | 2 columns      |
| Desktop | Same as design |

---

---

# 🚫 **Constraints**

❌ No fixed widths (`vw`, `px`)
❌ No inline CSS
❌ No float
❌ No copying code

✅ Only Tailwind
✅ Clean spacing
✅ Proper layout system

---

# 🧠 **What This Tests**

* Can you **break UI into components?**
* Can you combine **grid + flex correctly?**
* Can you build **real product UI (not just styled HTML)?**

---

# 🔥 HINTS (Important)

### 1. Cards container:

```html
flex flex-col md:flex-row gap-6
```

---

### 2. Buttons:

```html
bg-blue-500 text-white px-4 py-2 rounded-full
```

---

### 3. Spacing consistency:

```html
p-6 gap-4 mt-4
```

---

# 📊 **Evaluation Criteria**

| Area             | Marks |
| ---------------- | ----- |
| Layout accuracy  | 25    |
| Tailwind usage   | 25    |
| Visual hierarchy | 20    |
| Responsiveness   | 20    |
| Polish           | 10    |

---

# 🚀 Strategy (VERY IMPORTANT)

Do NOT try everything at once.

### Step order:

1. Heading
2. Cards (no styling first)
3. Add styling
4. Add gradient
5. Add features

---

