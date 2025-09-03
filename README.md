# Remote Work Tracker

## 1. Introduction  
Welcome to the **Remote Work Tracker** project!  
This is a comprehensive, full-stack application designed for organizations to understand and analyze remote work patterns in a secure, private, and efficient manner.  

The system is composed of three distinct services:  
1. A lightweight desktop daemon to track activity.  
2. A robust backend server for data processing and storage.  
3. A modern web dashboard for data visualization.  

This repository, **remote-work-tracker**, serves as the central hub for all project documentation and links the three core application repositories together using **Git Submodules**.  

---

## 2. Repository Structure: A Multi-Repo Setup  
This project uses a **multi-repo architecture** managed with Git Submodules.  
The code for each of the three main services lives in its own dedicated repository, while this parent repository acts as an aggregator.  

This approach keeps the codebase for each service clean, independent, and easier to manage.  

### Core Repositories  

| Repository | Description |
|------------|-------------|
| 📍 **remote-work-tracker** (You are here) | The main repository. Contains all project documentation and links to the service repositories below. |
| 💻 **remote-work-tracker-daemon** | Contains the Python code for the cross-platform client-side daemon that runs on an employee's computer. |
| 🗄 **remote-work-tracker-backend** | Contains the FastAPI backend server responsible for data ingestion, processing, and serving the API. |
| 📊 **remote-work-tracker-frontend** | Contains the React.js single-page application for the user-facing dashboard. |

Repositories:  
- [Daemon Repository](https://github.com/Ashish-Ram0906/remote-work-tracker-daemon)  
- [Backend Repository](https://github.com/Ashish-Ram0906/remote-work-tracker-backend)  
- [Frontend Repository](https://github.com/Ashish-Ram0906/remote-work-tracker-frontend)  

---

## 3. How to Work With This Project  

### Cloning the Repository  
Because this project uses Git Submodules, you need to use a special clone command to get all the code at once:  

```bash
git clone --recurse-submodules https://github.com/Ashish-Ram0906/remote-work-tracker.git
