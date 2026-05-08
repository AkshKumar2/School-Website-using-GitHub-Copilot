# 🎓 Greenfield Academy — School Website

A clean, responsive school website built with pure **HTML**, **CSS**, and **JavaScript** — no frameworks, no dependencies, just one single file.

![HTML5](https://img.shields.io/badge/HTML5-E34F26?style=flat&logo=html5&logoColor=white)
![CSS3](https://img.shields.io/badge/CSS3-1572B6?style=flat&logo=css3&logoColor=white)
![JavaScript](https://img.shields.io/badge/JavaScript-F7DF1E?style=flat&logo=javascript&logoColor=black)
![Responsive](https://img.shields.io/badge/Responsive-Yes-0d2145?style=flat)
![Single File](https://img.shields.io/badge/Single%20File-✓-f0a500?style=flat)

---

## 📸 Preview

| Section | Description |
|---|---|
| 🏠 Hero | Full-screen banner with school tagline and CTA buttons |
| 🏫 About | School values, history, and mission |
| 📚 Courses | 6 course cards with hover effects |
| 📬 Contact | Validated form with toast notification |

---

## ✨ Features

- **Single-file project** — everything lives in `school_website.html`
- **Fully responsive** — mobile-friendly layout with a hamburger navigation menu
- **Contact form validation** — checks for empty fields and validates email format using JavaScript
- **Toast notification** — success message slides in after form submission
- **Smooth scroll navigation** — clicking nav links scrolls to the correct section
- **Hover effects** — on buttons, nav links, and course cards
- **Well-commented code** — beginner-friendly comments throughout HTML, CSS, and JS
- **No external dependencies** — only Google Fonts is loaded (from CDN)

---

## 🗂️ Sections

| # | Section | What's Inside |
|---|---|---|
| 1 | **Header / Nav** | Fixed navbar, school logo, nav links, mobile hamburger toggle |
| 2 | **Home (Hero)** | Welcome badge, headline, description, CTA buttons, stats card |
| 3 | **About** | School story, 25+ years badge, values list with icons |
| 4 | **Courses** | 6 cards — Science, Mathematics, Arts, PE, Languages, Coding & Robotics |
| 5 | **Contact** | Address, phone, email info + validated contact form |
| 6 | **Footer** | Copyright line |

---

## 🛠️ Tech Stack

| Technology | Usage |
|---|---|
| **HTML5** | Semantic page structure |
| **CSS3** | Styling, layout (Grid/Flexbox), animations, responsive breakpoints |
| **Vanilla JavaScript** | Form validation, mobile menu toggle, toast notification |
| **Google Fonts** | Playfair Display (headings) + DM Sans (body text) |

---

## 🚀 Getting Started

No build tools or installation needed.

**Option 1 — Open directly in browser**
```bash
# Clone the repository
git clone https://github.com/your-username/greenfield-academy.git

# Open the file
cd greenfield-academy
open school_website.html       # macOS
start school_website.html      # Windows
xdg-open school_website.html   # Linux
```

**Option 2 — Use Live Server (VS Code)**
1. Install the [Live Server extension](https://marketplace.visualstudio.com/items?itemName=ritwickdey.LiveServer) in VS Code
2. Right-click `school_website.html` → **Open with Live Server**

That's it — no `npm install`, no build step. ✅

---

## 📁 Project Structure

```
greenfield-academy/
│
└── school_website.html     # Complete website (HTML + CSS + JS in one file)
└── README.md               # Project documentation
```

---

## 🎨 Color Palette

| Name | Hex | Usage |
|---|---|---|
| Navy | `#0d2145` | Primary background, headings |
| Blue | `#1a56db` | Accents, links, focus states |
| Gold | `#f0a500` | Highlights, CTA buttons |
| Sky | `#e8f0fe` | Light backgrounds, icon fills |
| White | `#ffffff` | Cards, sections |

---

## ⚙️ JavaScript Functionality

### 1. Mobile Navigation Toggle
```js
navToggle.addEventListener('click', function () {
  navLinks.classList.toggle('open');
});
```
Toggles the `.open` class on the nav list to show/hide links on mobile.

### 2. Welcome Alert (Interactive Feature)
```js
function showWelcome() {
  alert('🎓 Welcome to Greenfield Academy!...');
}
```
Triggered by the "Get Started" button in the hero section.

### 3. Form Validation
```js
function submitForm() {
  // Checks all fields are non-empty
  // Validates email with regex: /^[^\s@]+@[^\s@]+\.[^\s@]+$/
  // Shows inline error messages on invalid fields
}
```

### 4. Toast Notification
```js
function showToast() {
  toast.classList.add('show');        // Slide in
  setTimeout(() => toast.classList.remove('show'), 3500);  // Slide out
}
```

---

## 📱 Responsive Breakpoints

| Breakpoint | Layout Change |
|---|---|
| `> 768px` | Two-column grids for hero, about, contact; 3-column course grid |
| `≤ 768px` | All grids collapse to single column; hamburger menu appears |
| `≤ 480px` | Hero buttons stack vertically |

---

## 🔧 Customization Guide

| What to change | Where to find it |
|---|---|
| School name & logo | `<div class="nav-logo">` in the `<header>` |
| Hero headline & text | `<h1 class="hero-title">` in `#home` section |
| Course cards | `.course-card` `<div>`s in `#courses` section |
| Contact details | `.info-items` in `#contact` section |
| Color theme | `:root` CSS variables at the top of `<style>` |
| Fonts | Google Fonts `<link>` in `<head>` + `font-family` in `:root` |

---

## 📄 License

This project is open-source and available under the [MIT License](LICENSE).

---

## 🙋 Author

Made with 💙 as a beginner-friendly school project.  
Feel free to fork, customize, and use it for your own school or learning portfolio!

> ⭐ If you found this useful, consider giving the repo a star!
