<div align="center">

# ✖️ QuickMultiply

### Multiply any numbers — instantly, in the cloud.

[![Python](https://img.shields.io/badge/Python-3.10+-3776AB?style=for-the-badge&logo=python&logoColor=white)](https://python.org)
[![Flask](https://img.shields.io/badge/Flask-2.x-000000?style=for-the-badge&logo=flask&logoColor=white)](https://flask.palletsprojects.com)
[![Docker](https://img.shields.io/badge/Docker-Containerized-2496ED?style=for-the-badge&logo=docker&logoColor=white)](https://docker.com)
[![Render](https://img.shields.io/badge/Deployed_on-Render-46E3B7?style=for-the-badge&logo=render&logoColor=white)](https://quickmultiply.onrender.com)
[![License](https://img.shields.io/badge/License-MIT-green?style=for-the-badge)](LICENSE)

<br/>

> A production-ready Flask web application containerized with Docker and deployed live on Render.  
> Built to demonstrate modern backend development — RESTful architecture, containerization, cloud deployment, and clean UI design.

<br/>

🔗 **[Live Demo → quickmultiply.onrender.com](https://quickmultiply.onrender.com)**

</div>

---

## 📌 Table of Contents

- [About the Project](#-about-the-project)
- [Live Demo](#-live-demo)
- [Features](#-features)
- [Tech Stack](#-tech-stack)
- [How It Works](#-how-it-works)
- [Project Structure](#-project-structure)
- [Getting Started](#-getting-started)
- [Docker Usage](#-docker-usage)
- [Deployment](#-deployment-on-render)
- [Contributing](#-contributing)
- [License](#-license)

---

## 🎯 About the Project

**QuickMultiply** is a lightweight, production-grade Flask web app that lets users multiply any set of numbers by entering them as a comma-separated list. While the functionality is intentionally simple, the engineering behind it is not — this project is built to showcase a complete, real-world backend development workflow:

- ✅ RESTful web app with Flask
- ✅ Containerized with Docker for environment consistency
- ✅ Version-controlled with Git and hosted on GitHub
- ✅ Deployed to the cloud via Render with zero manual server setup

---

## 🚀 Live Demo

> **[https://quickmultiply.onrender.com](https://quickmultiply.onrender.com)**

Enter numbers like `2, 3, 4` and get the result `24` instantly.

---

## ✨ Features

- ➕ Multiply any quantity of numbers from a single input field
- 🔢 Handles both integers and floating-point numbers seamlessly
- ⚠️ Graceful error handling for invalid inputs
- 📱 Fully responsive — works on mobile, tablet, and desktop
- 🎨 Clean gradient UI with smooth hover animations
- 🐳 Docker-ready for consistent local and production environments
- ☁️ Live and publicly accessible via Render cloud deployment

---

## 🛠️ Tech Stack

| Layer | Tool |
|---|---|
| **Language** | Python 3.10+ |
| **Web Framework** | Flask |
| **Frontend** | HTML5, CSS3 (inline via `render_template_string`) |
| **Containerisation** | Docker |
| **Cloud Deployment** | Render |
| **Version Control** | Git & GitHub |

---

## 🧠 How It Works

```
User enters:  "2, 3, 4"
                  │
                  ▼
         POST /  (Flask route)
                  │
                  ▼
     Split string by comma → ["2", "3", "4"]
                  │
                  ▼
     Convert to float list → [2.0, 3.0, 4.0]
                  │
                  ▼
     Multiply iteratively  → 2 × 3 × 4 = 24
                  │
                  ▼
     If result is whole number → display as int
                  │
                  ▼
         Render result on page: "Result = 24"
```

Input validation catches non-numeric values and empty inputs, returning a user-friendly error message without crashing the app.

---

## 📂 Project Structure

```
QuickMultiply/
│
├── 🐍 app.py              # Flask app — routes, logic, and HTML template
├── 📋 requirements.txt    # Python dependencies (Flask)
├── 🐳 Dockerfile          # Container build instructions
└── 📄 README.md           # Project documentation
```

---

## ⚙️ Getting Started

### Prerequisites

- Python 3.10+
- pip
- Docker *(optional, for containerized run)*

### 1. Clone the repository

```bash
git clone https://github.com/prithvicoder1/QuickMultiply.git
cd QuickMultiply
```

### 2. Install dependencies

```bash
pip install -r requirements.txt
```

### 3. Run the app locally

```bash
python app.py
```

Open your browser at **http://localhost:5001**

---

## 🐳 Docker Usage

Run the app inside a Docker container — no Python installation needed on your machine.

### Build the image

```bash
docker build -t quickmultiply .
```

### Run the container

```bash
docker run -p 5001:5001 quickmultiply
```

Open your browser at **http://localhost:5001**

---

## ☁️ Deployment on Render

This app is deployed live on **[Render](https://render.com)** using the Docker runtime.

**To deploy your own instance:**

1. Push your code to GitHub
2. Go to [render.com](https://render.com) and create a **New Web Service**
3. Connect your GitHub repository
4. Set the environment to **Docker**
5. Render auto-detects the `Dockerfile` and builds & deploys automatically

Every push to `main` triggers a fresh deployment — zero manual steps.

---

## 🤝 Contributing

Contributions are welcome!

1. Fork the repository
2. Create your branch: `git checkout -b feature/your-feature`
3. Commit your changes: `git commit -m 'Add your feature'`
4. Push to the branch: `git push origin feature/your-feature`
5. Open a Pull Request

---

## 📄 License

Distributed under the MIT License. See [LICENSE](LICENSE) for details.

---

<div align="center">

Made with ❤️ by [Prithvi](https://github.com/prithvicoder1)

⭐ Found this useful? Give it a star — it means a lot!

</div>
