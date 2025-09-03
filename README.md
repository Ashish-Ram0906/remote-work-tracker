# Remote Work Tracker

## 1. Introduction 
Welcome to the Remote Work Tracker project! This is a comprehensive, full-stack application designed for organizations to understand and analyze remote work patterns in a secure, private, and efficient manner.  

The system is composed of three distinct services:  
1. A lightweight desktop daemon to track activity.  
2. A robust backend server for data processing and storage.  
3. A modern web dashboard for data visualization.  

This repository, **remote-work-tracker**, serves as the central hub for all project documentation and links the three core application repositories together using **Git Submodules**.  

---

## 2. Repository Structure: A Poly-Repo Architecture  
This project uses a poly-repo architecture (also known as multi-repo) managed with Git Submodules. This means the code for each of the three main services lives in its own dedicated repository, while this parent repository acts as a central aggregator for documentation and project oversight.  

This approach keeps the codebase for each service clean, independent, and easier to manage.  

### The Core Repositories  

Repository | Description
-----------|------------
📍 remote-work-tracker (You are here) | The main repository. Contains all project documentation and links to the service repositories below.  
💻 remote-work-tracker-daemon | Contains the Python code for the cross-platform client-side daemon that runs on an employee's computer.  
🗄 remote-work-tracker-backend | Contains the FastAPI backend server responsible for data ingestion, processing, and serving the API.  
📊 remote-work-tracker-frontend | Contains the React.js single-page application for the user-facing dashboard.  

https://github.com/Ashish-Ram0906/remote-work-tracker-daemon  
https://github.com/Ashish-Ram0906/remote-work-tracker-backend  
https://github.com/Ashish-Ram0906/remote-work-tracker-frontend  

---

## 3. How to Work With This Project  

Because this project uses Git Submodules, you need to use a special clone command to get all the code at once.  

### Cloning the Repository  


git clone --recurse-submodules https://github.com/Ashish-Ram0906/remote-work-tracker.git
This command will:

Clone the main remote-work-tracker repository.

Automatically look at the .gitmodules file.

Clone the daemon, backend, and frontend repositories into the correct subfolders.

Pulling Updates
To pull the latest changes for the main project AND all the submodules, run:


# First, pull changes for the main repository
git pull  

# Then, pull the latest changes for all the submodules
git submodule update --remote --merge
4. Project Documentation
All detailed planning and technical documentation for this project is stored in this main repository, linked below for easy access.

Core Documents
Project Explanation: A detailed overview of the project's features and components.
https://docs.google.com/document/d/1g0VEnCadkxScmt1QZyg-uRjV1wtu1Cq_dXdsPxzGINQ/edit?usp=sharing

System Architecture Diagram: A high-level visual overview of the system.
https://drive.google.com/file/d/1rx1VdDqnzYRNzWlyG1SddtvJbnmhdv-1/view?usp=sharing

Technology Selection & Implementation Guide: The complete technical guide for developers.
https://docs.google.com/document/d/1WKHaeL2DnEiHNutbDdWYnkuYOBdBPNyRVPBlNVEqxdo/edit?usp=sharing

User & Project Management
Project Timeline (45-Day Roadmap): The detailed development schedule.
https://docs.google.com/document/d/1Znt264XKm2oUurxpdc85DfkTnlo7alDr3EqfhfIu8yo/edit?usp=sharing

User Flow Diagram: Visual diagrams for Employee and Admin journeys.
https://drive.google.com/file/d/1oZeQnVps65fLjP42RBqRx_MvFYY4oUsq/view?usp=sharing

Employee Flow Document: A detailed breakdown of the employee experience.
https://docs.google.com/document/d/1jctuIo9FlD-lL38PB-pdGbtgnxHtisutE4ducpwNA7M/edit?usp=sharing

Employer & Admin Flow Document: A detailed breakdown of the administrative experience.
https://docs.google.com/document/d/1j-x35K42Udql48C-18I18K2XBM4ty7lE0-SG--NI8_s/edit?usp=sharing

Project Structure Guide: A guide to the file structure of each service.
https://docs.google.com/document/d/1WNfCVM6hX4s68o1rLSBIn_wYm9hNGlAnMdnKdkrmSC8/edit?usp=sharing
