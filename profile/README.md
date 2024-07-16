## Welcome to the team 🙌

<!--

**Here are some ideas to get you started:**

🙋‍♀️ A short introduction - what is your organization all about?
👀 Contribution guidelines - how do team members dive in?
👩‍💻 Useful resources - where do you keep your docs? Is there anything else the team should know?
🍪 Fun facts - what is your team's favorite snack?
🧙 Remember, you can do mighty things with the power of [Markdown](https://docs.github.com/github/writing-on-github/getting-started-with-writing-and-formatting-on-github/basic-writing-and-formatting-syntax)
-->

------------------------------------------------------------------------------------------------------------------------------
# Directory Structure

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
env/                            :::Environment Variables
.gitignore                      :::Git Ignore File
docker-compose.yml              :::Docker Compose Configuration
README.md                       :::Readme File
requirements.txt                :::Python Requirements File
```

------------------------------------------------------------------------------------------------------------------------------
# v1.0 Goal

Allow user to:
[ADD USE CASES AS CI/CD ARE TIED TO IT]

------------------------------------------------------------------------------------------------------------------------------
