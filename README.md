<div align="center">

# 🤖 Auto-Fill Tool
### AI Resume Analyzer & Job Matcher

**Stop copy-pasting. Start applying smarter.**

[![GSSoC 2026](https://img.shields.io/badge/GSSoC-2026-orange?style=for-the-badge&logo=github)](https://gssoc.girlscript.tech/)
[![Open Source](https://img.shields.io/badge/Open%20Source-%E2%9D%A4-red?style=for-the-badge)](https://github.com/sunilkumar2170/Auto-Fill-Tool)
[![Contributions Welcome](https://img.shields.io/badge/Contributions-Welcome-brightgreen?style=for-the-badge)](CONTRIBUTING.md)
</div>

---

## 📌 What Is This?

**Auto-Fill Tool** is an open-source AI assistant that reads your resume, understands job descriptions, and matches them intelligently — so you spend less time copy-pasting and more time interviewing.

It combines a **resume analyzer**, a **job description parser**, and an **auto-fill engine** into a single, privacy-respecting tool that runs locally in your browser.

> **Built for GSSoC '26** — This project is actively accepting contributions from students and first-time open-source contributors. All skill levels welcome.

---

## 🎬 Demo

**Resume Builder in action:**

![Resume Builder Demo](https://i.ibb.co/jzcrrt8/resume-builder-demo-optimize.gif)

**Resume Parser in action:**

![Resume Parser Demo](https://i.ibb.co/JvSVwNk/resume-parser-demo-optimize.gif)

---

## ✨ Core Features

| Feature | What It Does |
|---|---|
| 🔄 **Real-Time Preview** | Resume PDF updates instantly as you type — no refresh needed. |
| 🎨 **ATS-Friendly Design** | Output follows U.S. resume best practices and is tested against platforms like Greenhouse and Lever. Fonts, margins, and bullet points are handled automatically. |
| 🔒 **100% Local Processing** | No sign-up. No server calls. Your data never leaves your browser. The app even works offline. |
| 📥 **Import Existing Resume** | Drop in your current PDF and the tool extracts your data instantly, ready for editing. |
| ✅ **Proven Track Record** | Users have landed roles at Google, Meta, Dropbox, and more. Hiring managers have noted its clean formatting. |
| 🤖 **AI Job Matching** | Paste a job description and the tool highlights keyword gaps between your resume and the role. |
| ✍️ **Auto-Fill Engine** | Automatically populates form fields across job applications using your parsed resume data. |

---

## 🔍 Resume Parser

The built-in resume parser lets you test how well any ATS (Applicant Tracking System) can read your resume.

Upload a PDF → get a structured breakdown of what the parser extracts. If important fields are missing, you'll know exactly what to fix.

📖 Read the full [Parser Algorithm Deep Dive](https://open-resume.com/resume-parser) to understand how it works under the hood.

---

## 🗂️ Project Structure

The project is built with **Next.js 13** and follows its standard conventions. All source code lives in `src/app`.

| Page Route | Code Path | Purpose |
|---|---|---|
| `/` | `/page.tsx` | Landing page — hero section, demo, testimonials |
| `/resume-import` | `/resume-import/page.tsx` | Upload and parse an existing resume PDF (`ResumeDropzone`) |
| `/resume-builder` | `/resume-builder/page.tsx` | Build and download your resume (`ResumeForm` + `Resume`) |
| `/resume-parser` | `/resume-parser/page.tsx` | Test ATS readability using `parseResumeFromPdf` |

---

## 🛠️ Tech Stack

| Layer | Technology | Why |
|---|---|---|
| **Language** | [TypeScript](https://github.com/microsoft/TypeScript) | Catches type errors at compile time, not at runtime. |
| **UI Library** | [React](https://github.com/facebook/react) | Component-based architecture keeps the UI modular and reusable. |
| **State Management** | [Redux Toolkit](https://github.com/reduxjs/redux-toolkit) | Manages the complex, nested resume state without boilerplate. |
| **CSS Framework** | [Tailwind CSS](https://github.com/tailwindlabs/tailwindcss) | Utility-first styling keeps everything in one file — no context switching. |
| **Web Framework** | [Next.js 13](https://github.com/vercel/next.js) | Static site generation + file-based routing out of the box. |
| **PDF Reader** | [PDF.js](https://github.com/mozilla/pdf.js) | Powers the resume parser's first step: reading raw PDF content. |
| **PDF Renderer** | [React-pdf](https://github.com/diegomura/react-pdf) | Generates the downloadable resume PDF from React components. |

---

## ⚙️ Local Development

### Prerequisites

Before you start, make sure you have the following installed:

| Tool | Version | Check |
|---|---|---|
| **Node.js** | v18 or higher | `node -v` |
| **npm** | v8 or higher | `npm -v` |
| **Git** | any recent version | `git --version` |

> **Windows users:** Use [Git Bash](https://git-scm.com/downloads) or [WSL2](https://learn.microsoft.com/en-us/windows/wsl/install) to run the commands below.

---

### Method 1 — npm (Recommended)

```bash
# 1. Clone the repository
git clone https://github.com/sunilkumar2170/Auto-Fill-Tool.git

# 2. Move into the project directory
cd Auto-Fill-Tool

# 3. Install dependencies
npm install

# 4. Start the development server
npm run dev
```

Then open [http://localhost:3000](http://localhost:3000) in your browser.

---

### Method 2 — Docker

```bash
# 1. Clone the repository
git clone https://github.com/sunilkumar2170/Auto-Fill-Tool.git

# 2. Move into the project directory
cd Auto-Fill-Tool

# 3. Build the Docker image
docker build -t auto-fill-tool .

# 4. Run the container
docker run -p 3000:3000 auto-fill-tool
```

Then open [http://localhost:3000](http://localhost:3000) in your browser.

---

## 🤝 Contributing (GSSoC '26 — Start Here)

We welcome contributors of all experience levels. Whether it's your first pull request or your fiftieth, here's how to get involved:

**1. Fork the repository** using the "Fork" button at the top right of this page.

**2. Clone your fork locally:**
```bash
git clone https://github.com/<your-username>/Auto-Fill-Tool.git
cd Auto-Fill-Tool
```

**3. Create a feature branch:**
```bash
git checkout -b feat/your-feature-name
```

**4. Make your changes, then commit:**
```bash
git add .
git commit -m "feat: describe what you changed"
```

**5. Push and open a Pull Request:**
```bash
git push origin feat/your-feature-name
```

Then open a PR against the `main` branch of `sunilkumar2170/Auto-Fill-Tool`.

> **GSSoC participants:** Tag your PR with the `GSSoC-2026` label and link it to the relevant issue. Check the [Issues tab](https://github.com/sunilkumar2170/Auto-Fill-Tool/issues) for `good first issue` and `help wanted` tags — those are the best starting points.

---

## 📋 Contribution Guidelines

- Follow the existing code style (TypeScript + Tailwind conventions).
- Write clear, descriptive commit messages (`feat:`, `fix:`, `docs:`, `refactor:`).
- Test your changes locally before submitting a PR.
- Keep PRs focused — one feature or fix per PR.
- If you're unsure about scope, open an issue first to discuss.

---

## 🐛 Reporting Issues

Found a bug or have a feature request? [Open an issue](https://github.com/sunilkumar2170/Auto-Fill-Tool/issues/new) and include:

- A clear description of the problem or idea
- Steps to reproduce (for bugs)
- Your OS, browser, and Node.js version
- Screenshots or screen recordings if relevant

---

## 📄 License

This project is licensed under the [AGPL-3.0](LICENSE) — free to use, modify, and distribute.

---

<div align="center">

Made with ❤️ for the open-source community · GSSoC 2026

**[⭐ Star this repo](https://github.com/sunilkumar2170/Auto-Fill-Tool)** if you find it useful — it helps more contributors discover the project.

</div>
