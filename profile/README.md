## Welcome to the team 🙌

🙋‍♀️ **INTRODUCTION**
Knowvus is a Knowledge-as-a-Service tool that aims to deliver information to users.

Knowvus completes this via real-time data ingestion, and AI analysis.

👀 **CONTRIBUTION GUIDELINES**

TBD

👩‍💻 **RESOURCES**

- [Lucid](https://lucid.app/lucidchart/27a4f1ab-1925-4b57-b286-d59169d5385b/edit?invitationId=inv_c172e4c8-e0a9-4258-a836-6ee22863362c&page=qAbGdBw9_a6I#) - Architecture Diagrams
- [Digital Ocean](https://DigitalOcean.com)       - Infrastructure-as-a-Service (Compute, Storage [RAM, SSD, CPU, GPU, NPU]
- [Cloud Flare](https://Cloudflare.com)           - Hosting
- [Github](https://Github.com/Knowvus.com)        -  Codebase + CI/CD
- [Docker](https://Docker.com)                    -  Containerization  Deployment

## COMPONENTS

**INFRASTRUCTURE**

- [Duke](https://github.com/Knowvus/Duke) - Server

**FEATURES**
- [Tassadar](https://github.com/Knowvus/Tassadar) - Knowledge Framework
- [Fenix](https://github.com/Knowvus/Fenix) - Frame Processing, Semantic Process & Vector Embedding
- [Overmind](https://github.com/Knowvus/Overmind) - Modal Recorder

**STORAGE**
- [Kerrigan](https://github.com/Knowvus/Kerrigan) - Postgres
- [Zeratul](https://github.com/Knowvus/Zeratul) - Milvus

**OBSERVABILITY**
- [Artanis](https://github.com/Knowvus/Artanis) - Observability

# DIRECTORY STRUCTURE (Template)
```
app/                            :::Top-Level Directory
├── .vscode/                    :::VSCode Configuration Files
├── build/                      :::Build Output Directory
├── node_modules/               :::Node.js Modules Directory
├── public/                     :::Public Static Files
├── src/                        :::Source Code Directory
│  ├── .github/                 :::GitHub Configuration
│  │  ├── workflows/            :::GitHub Actions Workflows
│  │  │  └── python-app.yml     :::Python App Workflow Configuration
│  ├── backend/                 :::Backend Functionality
│  │  ├── __init__.py           :::Backend Initialization
│  │  ├── Database.py           :::Database Management
│  │  ├── GPT.py                :::GPT Model Integration
│  │  └── Server.py             :::Backend Server Configuration
│  ├── config/                  :::Configuration Files
│  │  ├── logo.svg              :::Application Logo
│  │  ├── postcss.config.js     :::PostCSS Configuration
│  │  ├── reportWebVitals.js    :::Web Vitals Reporting
│  │  ├── setupTests.js         :::Test Setup Configuration
│  │  ├── tailwind.config.js    :::Tailwind CSS Configuration
│  │  └── tailwind.css          :::Tailwind CSS File
│  ├── pages/                   :::Application Pages
│  │  ├── css/                  :::Page Specific CSS Files
│  │  ├── Chat.js               :::Chat Page Component
│  │  ├── ChatModal.js          :::Chat Modal Component
│  │  ├── Dashboard.js          :::Dashboard Page Component
│  │  ├── Misc.js               :::Miscellaneous Page Component
│  │  ├── Nodegraph.js          :::Node Graph Page Component
```
<!--
│  │  ├── Objective.js          :::Objective Page Component
│  │  ├── Profile.js            :::Profile Page Component
│  │  ├── Selection.js          :::Selection Page Component
│  │  └── Tasks.js              :::Tasks Page Component
│  ├── tests/                   :::Test Files Directory
│  ├── __init__.py              :::Initialization File for src
│  ├── App.css                  :::Main App CSS
│  ├── App.js                   :::Main App Component
│  ├── index.css                :::Main Index CSS
│  └── index.js                 :::Main Index JavaScript
├── package-lock.json           :::Package Lock File
├── package.json                :::Package Configuration File
.gitignore                      :::Git Ignore File
README.md                       :::Readme File

-->
------------------------------------------------------------------------------------------------------------------------------
# v1.0 Goal

Allow user to:
[ADD USE CASES AS CI/CD ARE TIED TO IT]
------------------------------------------------------------------------------------------------------------------------------
