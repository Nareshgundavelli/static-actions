# 🚀 Static Website Deployment using GitHub Actions

## 📌 Project Overview

This project demonstrates how to deploy a static HTML website using **GitHub Actions** and **GitHub Pages**.

Whenever code is pushed to the `main` branch, GitHub Actions automatically builds and deploys the website.

This project helped me understand the fundamentals of CI/CD and repository-based deployment.

---

## 🌍 Live Website

```
https://YOUR_USERNAME.github.io/YOUR_REPOSITORY_NAME/
```

(Replace with your actual URL)

---

## 🛠 Technologies Used

- HTML5
- Git
- GitHub
- GitHub Actions
- GitHub Pages

---

## 📁 Project Structure

```
static-git-actions/
│
├── index.html
├── README.md
│
└── .github/
    └── workflows/
        └── deploy.yml
```

---

## 🔄 How Deployment Works

1. Developer pushes code to the `main` branch.
2. GitHub detects the push event.
3. GitHub Actions workflow is triggered.
4. The workflow:
   - Checks out the repository
   - Configures GitHub Pages
   - Uploads the website files
   - Deploys the site
5. Website becomes live automatically.

This process is called **CI/CD (Continuous Integration / Continuous Deployment).**

---

## 🤖 GitHub Actions Workflow

Workflow file location:

```
.github/workflows/deploy.yml
```

### Workflow Explanation

- `on: push` → Triggers workflow when code is pushed to `main`
- `actions/checkout` → Downloads repository code
- `actions/configure-pages` → Prepares GitHub Pages environment
- `actions/upload-pages-artifact` → Uploads website files
- `actions/deploy-pages` → Publishes website

---

## 🖼 Image Handling

The website uses an external image URL:

```html
<img src="IMAGE_URL_HERE">
```

### ⚠️ Note on External Image URLs

Using external image links may:
- Cause blurry images (if thumbnail)
- Break if source website blocks hotlinking
- Stop working if link expires

For production projects, it is recommended to:
- Store images inside the repository
- Or use a proper image hosting/CDN service

---

## 🚀 Setup Instructions (Step-by-Step)

### 1️⃣ Create Repository

Create a new repository on GitHub.

---

### 2️⃣ Add Website File

Create `index.html` in the root directory.

---

### 3️⃣ Create Workflow Directory

Create:

```
.github/workflows/
```

Inside it create:

```
deploy.yml
```

---

### 4️⃣ Add Deployment Workflow

Add GitHub Pages deployment configuration inside `deploy.yml`.

---

### 5️⃣ Enable GitHub Pages

Go to:

```
Settings → Pages
```

Under Source, select:

```
GitHub Actions
```

---

### 6️⃣ Push Code

```
git add .
git commit -m "Initial setup"
git push origin main
```

GitHub Actions will automatically deploy the site.

---

## 🎯 Key Learning Outcomes

- Understanding folder structure importance
- Writing GitHub Actions workflows
- Automating deployment with CI/CD
- Debugging 404 errors in GitHub Pages
- Understanding case sensitivity in Linux
- Difference between local vs external image hosting

---

## 🧠 Problems Faced & Solutions

### ❌ 404 Error
Cause:
- `index.html` was not in the root directory.

Solution:
- Moved `index.html` to root.

---

### ❌ Pages Configuration Error
Cause:
- GitHub Pages was not fully enabled.

Solution:
- Re-enabled Pages under Settings.

---

### ❌ Blurry Image
Cause:
- Used low-resolution Google thumbnail link.

Solution:
- Used proper high-resolution image URL.