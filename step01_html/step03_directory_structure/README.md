### Markdown Version:

```markdown
# HTML Links and Navigation Guide

This repository contains examples and explanations to help students understand how HTML links work and how to navigate between sections of a page or across multiple pages effectively.

## 🔗 Understanding HTML Links

HTML links (or **anchors**) are created using the `<a>` tag. Links are used to navigate between web pages, jump to specific sections of a page, or perform actions like opening an email client or making a call.

### 📌 Basic Syntax

```html
<a href="URL">Link Text</a>
```

### **Attributes in Links**

#### 1. `href` (Hypertext Reference)
- Specifies the URL or location the link points to.
- Can link to:
  - Another webpage: `href="https://example.com"`
  - A section of the same page: `href="#section-id"`
  - An email: `href="mailto:email@example.com"`
  - A phone number: `href="tel:+1234567890"`

#### 2. `target="_blank"`
- Opens the link in a **new tab or window**.
- Example:
  ```html
  <a href="https://example.com" target="_blank">Open in New Tab</a>
  ```

---

## 📧 `mailto` Links

- Used to open the user's default email client with a pre-filled email address.
- Example:
  ```html
  <a href="mailto:info@example.com">Email Us</a>
  ```
- You can also include additional parameters like subject or body:
  ```html
  <a href="mailto:info@example.com?subject=Hello&body=I%20am%20interested%20in...">Contact Us</a>
  ```

---

## ☎️ `tel` Links

- Used to make phone numbers clickable for calling.
- Example:
  ```html
  <a href="tel:+1234567890">Call Us</a>
  ```

---

## 🏷 Using `id` and `#` for Section Navigation

- The `id` attribute uniquely identifies an element on the page.
- You can create links that **jump to a specific section** using the `id` with `#`.

### Example:

```html
<!-- Section to jump to -->
<h2 id="about">About Us</h2>
<p>This is the About Us section.</p>

<!-- Link to the section -->
<a href="#about">Go to About Us</a>
```

- Clicking the link scrolls directly to the element with `id="about"`.

---

## 🌐 Navigating Between Pages

### **Relative Paths**
- Use `../` to navigate **up a folder**.
- Use folder and file names to navigate **within a structure**.

#### Folder Structure Example:

```
project/
├── index.html
├── about/
│   └── about.html
└── contact/
    └── contact.html
```

#### Linking Example:

- From `index.html` to `about.html`:
  ```html
  <a href="about/about.html">About Us</a>
  ```
- From `about.html` to `contact.html`:
  ```html
  <a href="../contact/contact.html">Contact Us</a>
  ```

---

## 🚀 One-Page Navigation Example

You can combine the above concepts to navigate sections on the same page.

```html
<!-- Navbar -->
<nav>
  <a href="#home">Home</a>
  <a href="#services">Services</a>
  <a href="#contact">Contact</a>
</nav>

<!-- Sections -->
<section id="home">
  <h1>Welcome to Our Website</h1>
</section>

<section id="services">
  <h2>Our Services</h2>
</section>

<section id="contact">
  <h2>Contact Us</h2>
</section>
```

Clicking the links will smoothly scroll to the corresponding sections.

---

## 🛠️ Key Concepts Recap

1. Use `<a href="URL">` to create links.
2. Add `target="_blank"` to open links in a new tab.
3. Use `mailto` for email links and `tel` for phone links.
4. Use `id` and `#` for jumping between sections on the same page.
5. Use `../` and relative paths for folder navigation.

Explore this repository to see practical examples of these concepts!

---

## 📂 Folder Structure

```
project/
├── index.html  (Main Page)
├── about/
│   └── about.html (About Us Page)
├── contact/
│   └── contact.html (Contact Page)
└── assets/
    └── styles.css (CSS Styles)
```

Happy Coding! 😊
