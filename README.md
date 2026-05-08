# 🎓 Greenfield Academy — School Website

A clean, responsive school website built with pure **HTML**, **CSS**, and **JavaScript** — no frameworks, no dependencies, just one single file. Features a fully working contact form powered by **FormSubmit**.

![HTML5](https://img.shields.io/badge/HTML5-E34F26?style=flat&logo=html5&logoColor=white)
![CSS3](https://img.shields.io/badge/CSS3-1572B6?style=flat&logo=css3&logoColor=white)
![JavaScript](https://img.shields.io/badge/JavaScript-F7DF1E?style=flat&logo=javascript&logoColor=black)
![FormSubmit](https://img.shields.io/badge/FormSubmit-Integrated-22543d?style=flat)
![Responsive](https://img.shields.io/badge/Responsive-Yes-0d2145?style=flat)

🌐 **Live Demo:** [akshkumar2.github.io/School-Website-using-GitHub-Copilot](https://akshkumar2.github.io/School-Website-using-GitHub-Copilot/)

---

## 📸 Preview

| Section | Description |
|---|---|
| 🏠 Hero | Full-screen banner with school tagline and CTA buttons |
| 🏫 About | School values, history, and mission |
| 📚 Courses | 6 course cards with hover effects |
| 📬 Contact | Real working form that sends emails via FormSubmit |

---

## ✨ Features

- **Single-file project** — everything lives in `school_website.html`
- **Fully responsive** — mobile-friendly layout with a hamburger navigation menu
- **Real contact form** — emails are delivered via [FormSubmit](https://formsubmit.co), no backend needed
- **No CAPTCHA** — disabled for a smooth user experience
- **Auto redirect after submit** — user is sent back to the live site after sending a message
- **Smooth scroll navigation** — clicking nav links scrolls to the correct section
- **Welcome alert** — interactive JS feature on the "Get Started" button
- **Hover effects** — on buttons, nav links, and course cards
- **Well-commented code** — beginner-friendly comments throughout HTML, CSS, and JS
- **No external dependencies** — only Google Fonts loaded from CDN

---

## 🗂️ Sections

| # | Section | What's Inside |
|---|---|---|
| 1 | **Header / Nav** | Fixed navbar, school logo, nav links, mobile hamburger toggle |
| 2 | **Home (Hero)** | Welcome badge, headline, description, CTA buttons, stats card |
| 3 | **About** | School story, 25+ years badge, values list with icons |
| 4 | **Courses** | 6 cards — Science, Mathematics, Arts, PE, Languages, Coding & Robotics |
| 5 | **Contact** | Address, phone, email + real form that sends to your inbox |
| 6 | **Footer** | Copyright line |

---

## 🛠️ Tech Stack

| Technology | Usage |
|---|---|
| **HTML5** | Semantic page structure |
| **CSS3** | Styling, Grid/Flexbox layout, animations, responsive breakpoints |
| **Vanilla JavaScript** | Mobile menu toggle, welcome alert |
| **FormSubmit** | Backend-free email delivery for the contact form |
| **Google Fonts** | Playfair Display (headings) + DM Sans (body text) |

---

## 🚀 Getting Started

No build tools or installation needed.

**Option 1 — Open directly in browser**
```bash
# Clone the repository
git clone https://github.com/akshkumar2/School-Website-using-GitHub-Copilot.git

# Open the file
cd School-Website-using-GitHub-Copilot
open school_website.html       # macOS
start school_website.html      # Windows
xdg-open school_website.html   # Linux
```

**Option 2 — Use Live Server (VS Code)**
1. Install the [Live Server extension](https://marketplace.visualstudio.com/items?itemName=ritwickdey.LiveServer) in VS Code
2. Right-click `school_website.html` → **Open with Live Server**

**Option 3 — Visit the live site**
> [akshkumar2.github.io/School-Website-using-GitHub-Copilot](https://akshkumar2.github.io/School-Website-using-GitHub-Copilot/)

---

## 📁 Project Structure

```
School-Website-using-GitHub-Copilot/
│
├── school_website.html     # Complete website (HTML + CSS + JS in one file)
└── README.md               # Project documentation
```

---

## 📬 Contact Form — How It Works

The contact form uses **[FormSubmit](https://formsubmit.co)** — a free service that delivers form submissions directly to your email with zero backend code.

```html
<form
  action="https://formsubmit.co/your@email.com"
  method="POST"
>
  <input type="hidden" name="_captcha" value="false">
  <input type="hidden" name="_subject" value="New Message From School Website">
  <input type="hidden" name="_next" value="https://your-site-url.com">
  ...
</form>
```

| Hidden Field | Purpose |
|---|---|
| `_captcha` | Set to `false` to disable CAPTCHA |
| `_subject` | Custom subject line for received emails |
| `_next` | Redirect URL shown to user after submission |

> ⚠️ **First-time setup:** FormSubmit will send a **one-time confirmation email** to the address in the `action` URL. You must click the confirmation link before submissions start arriving in your inbox.

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
| School name & logo | `<div class="nav-logo">` in `<header>` |
| Hero headline & text | `<h1 class="hero-title">` in `#home` |
| Course cards | `.course-card` divs in `#courses` |
| Contact details | `.info-items` in `#contact` |
| Form recipient email | `action="https://formsubmit.co/YOUR_EMAIL"` |
| Redirect URL after submit | `<input name="_next" value="YOUR_URL">` |
| Color theme | `:root` CSS variables at the top of `<style>` |
| Fonts | Google Fonts `<link>` in `<head>` |

---

## 📄 License

This project is open-source and available under the [MIT License](LICENSE).

---

## 🙋 Author

**Aksh Kumar** — CSE (AI/ML) student at Lovely Professional University  
Built as a beginner-friendly web development project.

> ⭐ If you found this useful, consider giving the repo a star!
