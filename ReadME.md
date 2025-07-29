# 🧾 Complete Guide: Connecting Your Local Git Repository to GitHub

This guide explains how to:
- Create or use a local Git repository  
- Link it to a GitHub remote repository  
- Push your code from local to remote (GitHub)

---

## 🔧 Prerequisites
Before running the commands below, make sure:
- Git is installed on your computer.
- You have a GitHub account.
- You’ve created a GitHub repository (e.g., `https://github.com/Itsharshitgoat/first-repo.git`)

---

## 🗂️ 1. Navigate to your project folder

```bash
cd Desktop
cd first-repo
```

---

## 🌱 2. Initialize a local Git repository

```bash
git init
```
_Sets up Git tracking in your folder. Only needs to be done once per project._

---

## 📝 3. Create a file to commit (optional but needed for first push)

```bash
echo "# first-repo" > README.md
```
_Creates a basic README.md file for testing the push._

---

## 📥 4. Stage your files for commit

```bash
git add .
```
_Adds all current files to the staging area._

---

## 📦 5. Make your first commit

```bash
git commit -m "Initial commit"
```
_Saves the current state of the project with a message._

---

## 🌳 6. Rename default branch to main

```bash
git branch -M main
```
_Renames the default branch from master to main._

---

## 🌍 7. Add the GitHub remote

```bash
git remote add india https://github.com/Itsharshitgoat/first-repo.git
```
_Links your local repo to the GitHub remote._

If it already exists, remove and re-add:

```bash
git remote remove india
git remote add india https://github.com/Itsharshitgoat/first-repo.git
```

---

## 🚀 8. Push code to GitHub

```bash
git push -u india main
```
_Pushes the main branch and sets up tracking with the remote._

---

## 🔎 9. Check remote setup (optional)

```bash
git remote -v
```
_Confirms the correct connection to GitHub._

---

## 🔄 Daily workflow (after initial setup)

```bash
git add .
git commit -m "Your message"
git push
```

---

## ✅ Summary of Commands

```bash
cd Desktop
cd first-repo
git init
echo "# first-repo" > README.md
git add .
git commit -m "Initial commit"
git branch -M main
git remote add india https://github.com/Itsharshitgoat/first-repo.git
git push -u india main
```
