# Personal Portfolio

This site looks is inspired from [Mengjia Yan's MIT CSAIL Faculty Homepage](https://people.csail.mit.edu/mengjia/), customized for **Me ~ Dipesh Kharel**.

---

## 📁 Simple Code Structure

```text
MyWeb/
├── index.html                  # Main webpage with identical CSAIL sections & layout
├── css/
│   └── style.css               # Exact StartBootstrap Resume styles with MIT crimson (#910d22)
├── js/
│   └── main.js                 # Smooth scroll (jQuery Easing), mobile navbar, and scrollspy
└── Assets/
    ├── profile.JPG             # Your circular profile image in the sidebar
    ├── CV.pdf                  # Your Curriculum Vitae
    └── MIT-logo-black-gray.png # MIT bottom emblem logo
```

---

## Quick Start

### 1. View Locally
Simply double-click `index.html` to open it in Chrome, Firefox, or Edge.

Or run Python's built-in web server:
```bash
python3 -m http.server 8085
```
Then visit: `http://localhost:8085`

---

## Easy Modification Guide

The HTML file is organized cleanly with self-explanatory section IDs:

| Section ID | What it Contains |
| :--- | :--- |
| `#about` | Name, title, department, bio paragraphs, and social icons |
| `#news` | Recent announcements and collapsible `>> older news...` drawer |
| `#students` | Mentoring, tutoring, and student collaborations |
| `#teaching` | Teaching assistantships, courses, and instructors |
| `#publications` | Papers & projects with links to PDF, code, and BibTeX |
| `#awards` | Honors, class rankings, and academic awards |
| `#service` | Engineering experience and community service |

### Adding a Publication or Project
In `index.html`, locate `<section ... id="publications">` and add a new item:

```html
<li class="mb-3">
  <strong>Your Project or Paper Title</strong>;
  <u>Dipesh Kharel</u>, Co-Author Name.
  Conference or Journal, Year. <br>
  <a href="Assets/CV.pdf" target="_blank"><i class="fa-solid fa-file"></i> paper</a> &nbsp;
  <a href="https://github.com/..." target="_blank"><i class="fab fa-github"></i> code</a>
</li>
```

### Adding a News Item
In `index.html`, locate `<section ... id="news">` and insert a line:

```html
<li> 11/2026: Your announcement or milestone text. </li>
```

---

## Free Deployment to GitHub Pages

1. In your terminal inside `File Name`:
   ```bash
   git init
   git add .
   git commit -m "Initial academic homepage"
   ```
2. Create a GitHub repo named `<your-username>.github.io`.
3. Push your code:
   ```bash
   git remote add origin https://github.com/<your-username>/<your-username>.github.io.git
   git branch -M main
   git push -u origin main
   ```
Your website will immediately be accessible worldwide at:
`https://<your-username>.github.io/`
