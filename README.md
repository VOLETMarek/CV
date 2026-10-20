# 👨🏻‍💻 My Curriculum Vitae 👨🏻‍💻

☀️ Welcome to my GitHub repository for my CV! ☀️

This repository contains my updated CV, which showcases my skills, experience, and qualifications. The CV is available <a href="https://cv-five-weld.vercel.app/html/online-version" target="_blank"> here </a> 👌

## ⚒︎ My process ⚒︎

<strong>Built with :</strong>
- VSC
- HTML
- CSS
- JS

No framework, no build step: just static files.

## 🗂️ Project structure 🗂️

```
html/
  online-version/index.html   → CV published online (dark mode toggle, no phone number)
  pdf-version/index.html      → CV used to generate the PDF (phone number, no toggle)
css/
  reset.css                   → CSS reset
  style.css                   → All styles, split by commented sections
js/
  theme.js                    → Dark mode toggle
images/                       → Profile picture and icons
```

⚠️ Both `index.html` files share the same content. Any change to the CV must be made in **both** files. The only differences are:
- the dark mode toggle (`<div class="btn">`) and the scripts, only in the online version
- the phone number, only in the PDF version

## 🚀 Run locally 🚀

Start a local server from the **root** of the repository (CSS, JS and images are loaded with relative paths):

```bash
python3 -m http.server 8000
```

Then open:
- http://localhost:8000/html/online-version/
- http://localhost:8000/html/pdf-version/

Refresh the page (F5) after each change. For automatic reload, use the VS Code "Live Server" extension or `npx live-server` instead.

## 🎨 CSS conventions 🎨

`css/style.css` is organized by commented sections (`Global`, `Header`, `Main section left`, `Main section right`, `Dark Mode`, `Responsive Section`, `Print Section`). Add every new rule to the matching section, using the existing class naming (`.main-section_list`, `.section-list_item`, ...).

## 📄 Generate the PDF 📄

1. Open http://localhost:8000/html/pdf-version/ in Chrome
2. Press `Ctrl + P` and choose "Save as PDF"
3. In "More settings", check **Background graphics**

The `Print Section` in `style.css` handles the rest: A4 format, no margins, two-column layout, one single page. If the CV ever goes over one page, tighten the content or the spacing in that section.

## 🌍 Deployment 🌍

The CV is hosted on Vercel and deployed from the `master` branch: push your changes to `master` and the online version is updated.

## 📪 Contact 📪

If you have any questions, comments, or would like to connect, you can reach me via email at [marek.volet@hotmail.fr].

Thank you for visiting my CV repository, see you soon ☺️👋
