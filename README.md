# Knowvus - Knowledge-as-a-Service

## Traffic Info

![GitHub stars](https://img.shields.io/github/stars/MAKaminski/pickled-kimchi)
![GitHub watchers](https://img.shields.io/github/watchers/MAKaminski/pickled-kimchi)
![GitHub forks](https://img.shields.io/github/forks/MAKaminski/pickled-kimchi)
![GitHub contributors](https://img.shields.io/github/contributors/MAKaminski/pickled-kimchi)
![GitHub all releases](https://img.shields.io/github/downloads/MAKaminski/pickled-kimchi/total)
![GitHub release date](https://img.shields.io/github/release-date/MAKaminski/pickled-kimchi)
![GitHub last commit](https://img.shields.io/github/last-commit/MAKaminski/pickled-kimchi)

## Repo
![GitHub repo size](https://img.shields.io/github/repo-size/MAKaminski/pickled-kimchi)
![GitHub code size](https://img.shields.io/github/languages/code-size/MAKaminski/pickled-kimchi)
![GitHub language count](https://img.shields.io/github/languages/count/MAKaminski/pickled-kimchi)
![GitHub top language](https://img.shields.io/github/languages/top/MAKaminski/pickled-kimchi)
![Coverage](https://img.shields.io/codecov/c/github/MAKaminski/pickled-kimchi)
![GitHub license](https://img.shields.io/github/license/MAKaminski/pickled-kimchi)

## Issues
![GitHub issues](https://img.shields.io/github/issues/MAKaminski/pickled-kimchi)
![GitHub closed issues](https://img.shields.io/github/issues-closed/MAKaminski/pickled-kimchi)
![GitHub pull requests](https://img.shields.io/github/issues-pr/MAKaminski/pickled-kimchi)
![GitHub closed pull requests](https://img.shields.io/github/issues-pr-closed/MAKaminski/pickled-kimchi)

# Duke - Module of Knowa 🥬🫙🌶️
**Data Validation**
[] ORM Models
[] Pydantic Models
**Interface**
[] Website Endpoints
[] AI Interface

# Value Proposition
Anytime the organization generates new data useful to a users current task, they will be presented with the information.

# Summary
> 1) **AI-Driven Utilization:** Dynamically re-arranges user schedules to adhere to providing the highest Company Value defined as unit/value time given company objectives
> 2) **Passive Data Harvest:** Enterprise-wide data/communications are analyzed, and saved to a knowledgebase, and relationships are automatically inferred and associated with topics.
> 3)  **Company-Wide CI/CD:** Integration starts at the idea/research/content phase and ends at the Analytics/reporting phase so every idea that is implemented is tracked and can be measured for ROI.

# NOTES
1) Providing live-coaching to:
      a) Assist the user in completing tasks they are curretly working on by constantly evaluating:
      i) Current goals
      ii) Recent Progress
      iii) Ideal Next Step(s)
      iv) Presented in User's Learning Style

# CI/CD Build Status

![CI - Main](https://github.com/MAKaminski/pickled-kimchi/actions/workflows/CI.yaml/badge.svg?branch=main)

![CI - Dev](https://github.com/MAKaminski/pickled-kimchi/actions/workflows/CI.yaml/badge.svg?branch=dev)

### Main Branch

#### Python 3.10 and Node.js 14.x
![CI for Python 3.10 and Node.js 14.x](https://img.shields.io/github/actions/workflow/status/MAKaminski/pickled-kimchi/ci.yml?branch=main&label=Python%203.10%20Node%2014.x&logo=github&style=flat-square)

#### Python 3.11 and Node.js 18.x
![CI for Python 3.11 and Node.js 18.x](https://img.shields.io/github/actions/workflow/status/MAKaminski/pickled-kimchi/ci.yml?branch=main&label=Python%203.11%20Node%2018.x&logo=github&style=flat-square)

### Dev Branch

#### Python 3.10 and Node.js 14.x
![CI for Python 3.10 and Node.js 14.x](https://img.shields.io/github/actions/workflow/status/MAKaminski/pickled-kimchi/ci.yml?branch=dev&label=Python%203.10%20Node%2014.x&logo=github&style=flat-square)

#### Python 3.11 and Node.js 18.x
![CI for Python 3.11 and Node.js 18.x](https://img.shields.io/github/actions/workflow/status/MAKaminski/pickled-kimchi/ci.yml?branch=dev&label=Python%203.11%20Node%2018.x&logo=github&style=flat-square)

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
# System Architecture

1) **UI:**              Provides the front-end interface for user commands and system interaction.
2) **Server:**          The central hub for managing and routing system operations, including resource allocation and job management.
3) **Database:**        Handles data CRUD operations and interfaces with the Database and VectorDatabase for data-related tasks.
4) **Vector Database:** Handles data CRUD operations and interfaces with VectorDatabase for data-related tasks. | <ADD MILVUS> 
5) **GPT:**             Houses Agents that perform jobs <UPDATE GPT TO AGENT>
6) **KnodeGraph:**      Contains visualization of VectorDB Knowledge and Task Data <ADD Knodegraph>

# UPDATE BELOW HERE
<img width="1920" alt="Screenshot 2024-04-06 at 3 18 48 PM" src="https://github.com/MAKaminski/Swarm/assets/19610881/b3b6f928-c8f1-4834-b812-4465c58c0dc5">

------------------------------------------------------------------------------------------------------------------------------
# ERD

<img width="1920" alt="Screenshot 2024-04-06 at 3 18 37 PM" src="https://github.com/MAKaminski/Swarm/assets/19610881/255e16c2-dde0-4924-b05d-dde170778234">

------------------------------------------------------------------------------------------------------------------------------
# Credentials
**OpenAPI**
```
API_KEY = "sk-proj-iKqzqPBbXsrfCiJqv8WiT3BlbkFJGNxxNmtGIkujFn8iipsp"
```
**PostgresDB**
```
PROD_CREDS = {
            dbname=postgres,
            user=postgres,
            host=localhost,
            port=5432,
            password=None}
```
------------------------------------------------------------------------------------------------------------------------------
# Packages

# LANGUAGE
```
-- LIBRARY                 | PACKAGES                                     | DESCRIPTION
```
# REACT
```
-- react                   | React, useState, useEffect, useCallback      | UI Functionaltiy
-- react-dom/client        | ReactDOM                                     | Client Routing
-- react-router-dom        | BrowserRouter as Router, Route, Link, Routes | Server Routing
```
# SERVER
```
-- fastapi                 | FastAPI, HTTPException, Depends | fastapi    | FastAPI framework and necessary modules (*Depends Controls Session Requirements)
-- fastapi.logger          | logger                                       | FastAPI logger for server logging
-- fastapi.middleware.cors | CORSMiddleware                               | CORS middleware for handling cross-origin requests
-- fastapi.responses       | RedirectResponse                             | FastAPI response for redirecting requests
-- pydantic                | BaseModel                                    | Pydantic BaseModel for data validation and serialization
```
# POSTGRES
```
-- psycopg2                                                               | DB Connection
-- sqlalchemy.exc          | IntegrityErrory                              | SQLAlchemy exception for integrity errors
```
# LOGGING
```
-- logging                                                                | Standard logging module
-- datetime                | datetime                                     | Datetime module for handling date and time
-- traceback                                                              | Detailed Logging
-- pprint                  | pprint                                       | Enhanced Terminal Printing
-- functools                                                              | Wrapper Support
```
# LLM
```
-- openai                  | OpenAI                                       | GPT Responses
```
------------------------------------------------------------------------------------------------------------------------------
# RUN
package.json.js commands:
1) build: css
2) start-server
3) start-webserver
4) build
5) test
6) eject
7) install

# Launch Postgres
1) Docker
2) Postgres Connection
   
# Launch Milvus
1) Docker
2) Milvus Connection

------------------------------------------------------------------------------------------------------------------------------
# Contact Information
For inquiries or contributions, please contact Michael Kaminski at MKaminski1337@Gmail.com.

------------------------------------------------------------------------------------------------------------------------------
# FUTURE FEATURES

1) Milvus - VectorDB - Requires 4GB Docker + 8GB Milvus - Configure New Machine to Run Vector DB
   a) Inference
   b) KnowdeGraph*
   [ ] Selection Visualization

      1) Reduce font size of history box - feel good win
      2) Allow user to upload profile avatar and display it in top right - feel good win
      5) Allow task to be "selectable" - provide overview of information in "Selection Component" and "Objective Component"

*Aixtraction*
[Features]
```
[ ] Frequency
[ ] Core Dataset
```
*KnowdeGraph*
```
[ ] Selection Visualization
[ ] Oauth
[ ] 64GB Server for -- SETUP LOGGING TO MONITOR USAGE
    [ ] Available [20GB]
    [ ] OS [8GB]
    [ ] Milvus [16GB]
    [ ] Postgres [16GB]
    [ ] Docker [4GB]
    [ ] GPU Enabled - Check if CUDA or other Hardware Acceleration
    [ ] Web Server <Cloudflare?>
    [ ] FastAPI Server [Where does this run? Cloudflare?]
```

------------------------------------------------------------------------------------------------------------------------------
# <ADD LIBRARIES>
# LOGGING
```
-- schedule                                                               | CRON Timer
-- psutil                                                                 | System Usage
```
------------------------------------------------------------------------------------------------------------------------------
