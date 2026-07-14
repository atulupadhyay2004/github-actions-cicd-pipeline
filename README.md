# 🚀 GitHub Actions CI/CD Pipeline

[![GitHub repo size](https://img.shields.io/github/repo-size/atulupadhyay2004/github-actions-cicd-pipeline)](https://github.com/atulupadhyay2004/github-actions-cicd-pipeline)
[![GitHub stars](https://img.shields.io/github/stars/atulupadhyay2004/github-actions-cicd-pipeline?style=social)](https://github.com/atulupadhyay2004/github-actions-cicd-pipeline/stargazers)

> A production-grade 5-stage CI/CD pipeline built with **GitHub Actions** featuring automated testing, Docker build, health check validation, and simulated deployment — all triggered on every push to the `main` branch.

---

## 📋 Table of Contents
- [About The Project](#-about-the-project)
- [Features](#-features)
- [Tech Stack](#-tech-stack)
- [System Architecture](#-system-architecture)
- [CI/CD Workflow](#-cicd-workflow)
- [Pipeline Stages](#-pipeline-stages)
- [Getting Started](#-getting-started)
  - [Prerequisites](#prerequisites)
  - [Installation](#installation)
  - [Running Locally](#running-locally)
  - [Triggering the Pipeline](#triggering-the-pipeline)
- [Environment Variables](#-environment-variables)
- [Contributing](#-contributing)
- [License](#-license)
- [Contact](#-contact)

---

## 📖 About The Project

This project demonstrates a **complete CI/CD pipeline** using **GitHub Actions** for a Node.js application. The pipeline automates the entire software delivery lifecycle:

- **Code is pulled** from the repository on every push to `main`
- **Dependencies are installed** with caching for faster builds
- **Tests are executed** to catch regressions early
- **Health checks** validate the application is running correctly
- **Versioning** is automated using GitHub's run number
- **Deployment** is simulated (ready to be extended to AWS, Azure, or GCP)

The pipeline follows industry best practices with **job dependencies**, **output sharing**, and **fail-fast** behavior.

---

## ✨ Features

- ✅ **5-stage pipeline** — Build → Test → Health Check → Deploy
- ✅ **Automated versioning** — `1.0.<run_number>` format
- ✅ **Dependency caching** — Faster builds with `actions/cache`
- ✅ **Health check validation** — Ensures the app is healthy before deployment
- ✅ **Job dependencies** — Stages run in sequence with `needs`
- ✅ **Output sharing** — Version number passed from build to deploy
- ✅ **Simulated deployment** — Ready to be replaced with real deployment logic
- ✅ **Zero-touch automation** — Triggered on every push to `main`

---

## 🛠 Tech Stack

| Category | Technology |
|----------|------------|
| **CI/CD Platform** | GitHub Actions |
| **Application** | Node.js (v20) |
| **Testing** | npm test |
| **Caching** | actions/cache |
| **Versioning** | GitHub run_number |
| **Runtime** | Node.js HTTP server |

---


---

