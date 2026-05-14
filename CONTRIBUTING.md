# Contributing to Auto-Fill-Tool

First off, thank you for considering contributing to Auto-Fill-Tool! 
We welcome contributions of all sizes, from fixing typos to adding new features.

## 🚀 Getting Started

### 1. Fork and Clone

1. Fork the repository on GitHub by clicking the **Fork** button.
2. Clone your fork locally:
```bash
   git clone https://github.com/YOUR-USERNAME/Auto-Fill-Tool.git
   cd Auto-Fill-Tool
```
3. Add upstream remote:
```bash
   git remote add upstream https://github.com/sunilkumar2170/Auto-Fill-Tool.git
```

### 2. Install Dependencies
```bash
npm install
```

### 3. Create a Branch
```bash
git checkout -b my-new-feature
```
Use descriptive names (e.g., `fix/header-typo`, `feature/dark-mode`, `docs/update-readme`).

## 💻 Development Workflow

```bash
npm run dev
```
Open http://localhost:3000 in your browser.

### Linting
```bash
npm run lint
```

### Testing
```bash
npm test
```

## 📁 Project Structure

- `src/app/` — Next.js pages
- `src/app/components/` — Reusable React components
- `src/app/lib/` — Utility functions, Redux slices
- `public/` — Static assets

## 📬 Submitting a Pull Request

1. Commit your changes:
```bash
   git add .
   git commit -m "feat: add dark mode toggle"
```
2. Sync with upstream:
```bash
   git fetch upstream
   git rebase upstream/main
```
3. Push to your fork:
```bash
   git push origin my-new-feature
```
4. Open a PR on: https://github.com/sunilkumar2170/Auto-Fill-Tool

5. **Describe your PR clearly:**
   - What did you fix or add?
   - Attach screenshots (before & after)
   - Mention the issue number (e.g., Closes #17)

## 🤔 Need Help?

Open an issue and ask — we are happy to help!

Happy coding! 🎉
