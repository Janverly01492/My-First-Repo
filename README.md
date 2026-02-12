# 📝 Armada Git Workflow Guide

<p align="center">
    <a href="https://github.com/YOUR_USERNAME/organic-shop-tl/actions">
    </a>
    <a href="https://github.com/YOUR_USERNAME/organic-shop-tl">
</p>

---

# **📝 Armada Git Workflow Guide**
###### Made by
&nbsp;&nbsp;**Janverly Mhay O. Bacani**

---

## Description / Overview
This is a complete guide for contributing to the **Armada Organic Shop** project using Git and GitHub.  
Following this workflow ensures your changes are organized, your fork stays up-to-date, and pull requests are clean.  
It covers forking, cloning, syncing with the TL repository, working with `develop` and feature branches, and best practices for commits and pushes.

---

## Fork the Repository
- Go to the TL repository:  
  [https://github.com/Erudite098/organic-shop-tl](https://github.com/Erudite098/organic-shop-tl)  
- Click **Fork** → this creates a copy of the repository in your GitHub account.

---

##  Clone Your Fork Locally

git clone https://github.com/YOUR_USERNAME/organic-shop-tl.git
cd organic-shop-tl

## Set Up the TL Repository as Upstream
```bash
git remote add upstream https://github.com/Erudite098/organic-shop-tl.git
git fetch upstream
git remote -v  # Optional: check remotes
```
## Always Work on the Develop Branch

```bash 
git checkout develop
```


## Add Changes

```bash
git add <file-or-folder> # Stage specific files
git add . #Stage all changes
```
## Commit Changes

```bash
git commit - "Your commit message."
```

## Pushing the Changes

```bash
git push
```

## Keep your branch Up-to-Date

```bash
# If the TL repo has updates while you’re working:
git fetch upstream
git checkout develop
git pull upstream develop
git checkout feature/your-feature-name
git merge develop
# Resolve conflicts if any appear, then commit
```
