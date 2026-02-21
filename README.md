# Static Website Deployment using GitHub Actions 🚀

## 📌 Project Overview

This project demonstrates how to deploy a static HTML website using GitHub Actions and GitHub Pages.

Whenever code is pushed to the `main` branch, GitHub Actions automatically deploys the website.

---

## 🌍 Live Website

https://YOUR_USERNAME.github.io/YOUR_REPOSITORY_NAME/

---

## 📁 Project Structure

```
static-git-actions/
│
├── index.html
├── images/
│     └── myphoto.jpg
│
└── .github/
    └── workflows/
        └── deploy.yml
```

---

## ⚙️ Technologies Used

- HTML
- Git
- GitHub
- GitHub Actions
- GitHub Pages

---

## 🔄 How Deployment Works

1. Developer pushes code to the `main` branch.
2. GitHub Actions workflow is triggered.
3. The workflow:
   - Checks out the repository
   - Configures GitHub Pages
   - Uploads the website files
   - Deploys the site
4. Website becomes live automatically.

---

## 🤖 GitHub Actions Workflow

The deployment workflow file is located at:

```
.github/workflows/deploy.yml
```

It triggers on every push to the `main` branch.

---

## 🚀 Setup Steps (How To Recreate This Project)

### Step 1: Create Repository

Create a new repository on GitHub.

### Step 2: Add Website Files

Add `index.html` in the root folder.

### Step 3: Create GitHub Actions Workflow

Create:

```
.github/workflows/deploy.yml
```

Add deployment configuration.

### Step 4: Enable GitHub Pages

Go to:

Settings → Pages

Select:

Source → GitHub Actions

### Step 5: Push Code

```
git add .
git commit -m "Initial setup"
git push origin main
```

GitHub Actions will automatically deploy the website.

---

## 🎯 Key Learning Outcomes

- Understanding CI/CD basics
- Writing GitHub Actions workflow
- Deploying static sites automatically
- Managing repository structure
- Debugging deployment issues

---

## 📸 Features

- Full-screen background image
- Automatic deployment
- Clean folder structure

---

## 🧠 What I Learned

- GitHub Pages requires `index.html` in root
- Folder structure is important
- GitHub Actions automates deployment
- Case sensitivity matters in Linux environments

---

## 📜 License

This project is for learning purposes.