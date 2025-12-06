# DevOps CI/CD Demo — GitHub Actions (JS + Python + Load Test)

This repository demonstrates a complete **multi-language CI/CD pipeline** using **GitHub Actions**, including:

- ✔ JavaScript Unit Tests (Jest)
- ✔ Code Coverage Reporting
- ✔ Static Website Deployment to GitHub Pages
- ✔ Python-based Monitoring Script
- ✔ k6 Load Testing
- ✔ Student Participation (Real-Time Traffic Observation)

---

##  Project Structure
```
my-cicd-demo/
├── index.html
├── sum.js
├── sum.test.js
├── monitor.py
├── loadtest.js
├── package.json
├── requirements.txt
└── .github/workflows/deploy.yml
```

---

## Instructions

- After creating the repository > Go to repository settings > pages > choose Source: Github Actions.  [This allows your workflow to deploy automatically]
- Then, you can clone this repository > Makes any desired changes > commit & push.
- Incase you want to perform this entire task from scratch > There's a script.py in this repository that will help you to setup the required directory structure in your local env > Tweak changes to the files > Push and observe


---

##  CI: Tests + Coverage

Runs automatically on every push:

- Executes Jest unit tests
- Generates `coverage/` report
- Uploads coverage as GitHub artifact

---

##  CD: Deployment

The site deploys automatically to **GitHub Pages** after tests pass.

URL example:

https://USERNAME.github.io/REPO/


---

## Monitoring (Python)

After deployment, a Python script checks:

- Response latency
- Status code
- Content size
- Timestamp

Results output to:

metrics.json


You can download the artifact and see metrics.

---

## Load Testing (k6)

A lightweight load test runs automatically:

- 20 virtual users
- 20 seconds duration
- Hitting live GitHub Pages site

---

## 🛠 Tech Used

- GitHub Actions
- GitHub Pages
- Jest (Tests + Coverage)
- Python (Monitoring)
- k6 (Load Testing)

