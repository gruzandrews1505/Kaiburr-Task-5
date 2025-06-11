## Kaiburr Task 5 - DevOps CI/CD Pipeline

This project demonstrates a simple DevOps CI/CD setup using **GitHub Actions**. It includes a mock Node.js application and a workflow to automate installation, testing, and build steps.

---

##  Technologies Used

- GitHub Actions
- Node.js
- JavaScript
- Docker (included for containerization)
- npm scripts

---

## Project Structure

kaiburr-task-5-devops/
├── app/
│ ├── index.js # Entry point
│ └── package.json # Scripts: test, build
├── .github/
│ └── workflows/
│ └── ci.yml # CI/CD pipeline configuration
├── Dockerfile # Docker build config
├── README.md # Project overview
└── screenshots/
├── ui.png # Terminal output
└── code_screenshot.png # VS Code project view


---

##  CI/CD Pipeline

The GitHub Actions workflow runs on every `push` to the `main` branch and performs the following steps:

1. Checkout code  
2. Setup Node.js  
3. Install dependencies from `app/`  
4. Run mock tests  
5. Execute a simulated build

---

##  How to Run Locally

```bash
cd app
npm install
npm run test
npm run build


You should see:
"Running tests..."
"Building project..."
