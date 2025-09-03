Remote Work Tracker
1. Introduction
Welcome to the Remote Work Tracker project! This is a comprehensive, full-stack application designed for organizations to understand and analyze remote work patterns in a secure, private, and efficient manner. The system is composed of three distinct services:

A lightweight desktop daemon to track activity.

A robust backend server for data processing and storage.

A modern web dashboard for data visualization.

This repository, remote-work-tracker, serves as the central hub for all project documentation and links the three core application repositories together using Git Submodules.

2. Repository Structure: A Multi-Repo Setup
This project uses a multi-repo architecture managed with Git Submodules. This means the code for each of the three main services lives in its own dedicated repository, while this parent repository acts as an aggregator.

This approach keeps the codebase for each service clean, independent, and easier to manage.

The Core Repositories
Repository

Description

📍 remote-work-tracker (You are here)

The main repository. Contains all project documentation and links to the service repositories below.

💻 remote-work-tracker-daemon

Contains the Python code for the cross-platform client-side daemon that runs on an employee's computer.

🗄️ remote-work-tracker-backend

Contains the FastAPI backend server responsible for data ingestion, processing, and serving the API.

📊 remote-work-tracker-frontend

Contains the React.js single-page application for the user-facing dashboard.

3. How to Work With This Project
Because this project uses Git Submodules, you need to use a special clone command to get all the code at once.

Cloning the Repository
To clone this repository and all the code for the daemon, backend, and frontend, run the following command:

git clone --recurse-submodules [https://github.com/Ashish-Ram0906/remote-work-tracker.git](https://github.com/Ashish-Ram0906/remote-work-tracker.git)

This command will:

Clone the main remote-work-tracker repository.

Automatically look at the .gitmodules file.

Clone the daemon, backend, and frontend repositories into the correct subfolders (client-daemon/, backend-server/, frontend-dashboard/).

Pulling Updates
To pull the latest changes for the main project AND all the submodules, you need to run two commands:

# First, pull changes for the main repository
git pull

# Then, pull the latest changes for all the submodules
git submodule update --remote --merge

4. Project Documentation
All detailed planning and technical documentation for this project is stored in this main repository.

System Architecture: A high-level visual overview of the system.

User Flows: Diagrams detailing the journey for Employees and Admins.

Employee Flow Document: A detailed breakdown of the employee experience.

Employer & Admin Flow Document: A detailed breakdown of the administrative experience.

Technology & Implementation Guide: The complete technical guide for developers.

Project Structure Guide: A guide to the file structure of each service.
