# Contributing to OpenResume

First off, thank you for considering contributing to OpenResume! It's people like you that make OpenResume such a great tool for everyone. We welcome contributions of all sizes, from fixing typos to adding new features.

This document provides a set of guidelines and steps to help you contribute to this project.

## 🚀 Getting Started

### 1. Fork and Clone
1. Fork the repository on GitHub by clicking the **Fork** button in the top right corner.
2. Clone your fork locally:
   ```bash
   git clone https://github.com/YOUR-USERNAME/open-resume.git
   cd open-resume
   ```
3. Add the original repository as an upstream remote to keep your fork synced:
   ```bash
   git remote add upstream https://github.com/xitanggg/open-resume.git
   ```

### 2. Install Dependencies
Make sure you have [Node.js](https://nodejs.org/) installed. Then run:
```bash
npm install
```

### 3. Create a Branch
Always create a new branch for your work:
```bash
git checkout -b my-new-feature
```
Use descriptive branch names (e.g., `fix/header-typo`, `feature/dark-mode`, `docs/update-readme`).

## 💻 Development Workflow

Start the Next.js development server:
```bash
npm run dev
```
Open [http://localhost:3000](http://localhost:3000) in your browser. The app will automatically reload if you change any of the source files.

### Code Style & Linting
We use ESLint and Prettier to maintain code quality. Before submitting your code, please run:
```bash
npm run lint
```
Fix any linting errors that pop up!

### Testing
We use Jest for unit testing. To run the tests:
```bash
npm test
```
If you are adding a new feature or utility, please consider adding a test for it! For CI environments, use `npm run test:ci`.

## 📁 Project Structure Refresher
- `src/app/`: Contains the Next.js App Router pages (`/`, `/resume-builder`, `/resume-parser`, etc.).
- `src/app/components/`: Reusable React components (UI, Form, Resume preview).
- `src/app/lib/`: Utility functions, Redux slices (`redux/`), and the PDF parsing logic.
- `public/`: Static assets like images and fonts.

## 📬 Submitting a Pull Request (PR)

1. **Commit your changes**: Make sure your commit messages are clear and descriptive.
   ```bash
   git add .
   git commit -m "Add dark mode toggle button to TopNavBar"
   ```
2. **Sync with upstream**: Before pushing, pull the latest changes from the `main` branch of the original repo:
   ```bash
   git fetch upstream
   git rebase upstream/main
   ```
3. **Push to your fork**:
   ```bash
   git push origin my-new-feature
   ```
4. **Open a Pull Request**: Go to the original OpenResume repository on GitHub. You should see a prompt to open a PR from your recently pushed branch.
5. **Describe your changes**: Explain what you fixed or added clearly so maintainers can review it easily.

## 🤔 Need Help?
If you're stuck, feel free to open an issue and ask questions. We are happy to help beginners get started!

Happy coding! 🎉
