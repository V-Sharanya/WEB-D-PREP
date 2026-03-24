# 🔹 1. HTML BOILERPLATE (MANDATORY STRUCTURE)

Every HTML file should follow this structure:

```html
<!DOCTYPE html>
<html lang="en">
<head>
  <meta charset="UTF-8">
  <meta name="viewport" content="width=device-width, initial-scale=1.0">
  <title>My Page</title>
</head>
<body>
</body>
</html>
```

### Key Points:

* `<!DOCTYPE html>` → tells browser HTML5
* `lang="en"` → improves accessibility + SEO
* `meta viewport` → required for responsive design

---

# 🔹 2. SEMANTIC HTML (STRUCTURE LIKE A PRO)

Instead of random `<div>`, use meaningful structure:

```html
<header></header>
<nav></nav>

<main>
  <section>
    <article></article>
  </section>

  <aside></aside>
</main>

<footer></footer>
```

### Important Differences:

* `section` → grouping content
* `article` → independent content (blog, post)
* `aside` → sidebar

---

# 🔹 3. ACCESSIBILITY (a11y)

Make your website usable for everyone.

---

## ✔ Labels for Inputs

```html
<label for="email">Email</label>
<input id="email" type="email">
```

---

## ✔ Alt Text for Images

```html
<img src="image.jpg" alt="Profile picture">
```

---

## ✔ ARIA Attributes

```html
<button aria-label="Close menu">X</button>
```

---

## ✔ Best Practices

* Use semantic tags
* Ensure keyboard navigation
* Avoid using only color to convey meaning

---

# 🔹 4. FORMS — ADVANCED USAGE

---

## ✔ Input Types

```html
<input type="text">
<input type="email">
<input type="password">
<input type="number">
<input type="date">
<input type="file">
```

---

## ✔ Validation Attributes

```html
<input type="email" required>
<input type="text" pattern="[A-Za-z]+">
```

* `required` → must fill
* `pattern` → regex validation

---

## ✔ Textarea

```html
<textarea placeholder="Enter message"></textarea>
```

---

# 🔹 5. META TAGS (SEO BASICS)

```html
<meta name="description" content="Portfolio website">
<meta name="keywords" content="HTML, CSS, JavaScript">
<meta name="author" content="Sharanya">
```

👉 Helps:

* Search engines
* Page ranking

---

# 🔹 6. BLOCK vs INLINE vs INLINE-BLOCK

---

## ✔ Block Elements

* Take full width
* Example: `<div>`, `<p>`, `<section>`

---

## ✔ Inline Elements

* Take only content width
* Example: `<span>`, `<a>`, `<b>`

---

## ✔ Inline-Block

* Behaves like inline + can set width/height

---

# 🔹 7. IMAGE BEST PRACTICES

```html
<img src="img.jpg" alt="Description" width="200">
```

### Important:

* Always add `alt`
* Optimize image size (performance)
* Use correct formats (`jpg`, `png`, `webp`)

---

# 🔹 8. TABLES 

```html
<table border="1">
  <tr>
    <th>Name</th>
    <th>Age</th>
  </tr>
  <tr>
    <td>Sharanya</td>
    <td>20</td>
  </tr>
</table>
```

---

## ✔ Structure:

* `<table>` → container
* `<tr>` → row
* `<th>` → header
* `<td>` → data

---

# 🔹 9. HTML ENTITIES

Used for special characters:

```html
&lt;   <!-- < -->
&gt;   <!-- > -->
&nbsp; <!-- space -->
&copy; <!-- © -->
```

