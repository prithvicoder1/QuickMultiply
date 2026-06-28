<div align="center">

<!-- Animated wave header -->
<img width="100%" src="https://capsule-render.vercel.app/api?type=waving&color=gradient&customColorList=6,11,20&height=180&section=header&text=QuickMultiply&fontSize=62&fontColor=fff&animation=twinkling&fontAlignY=32&desc=Multiply%20any%20numbers%20%E2%80%94%20instantly,%20in%20the%20cloud.&descAlignY=55&descSize=18"/>

<!-- Typing animation -->
<a href="https://quickmultiply.onrender.com">
  <img src="https://readme-typing-svg.demolab.com?font=Fira+Code&weight=600&size=22&pause=1000&color=6C63FF&center=true&vCenter=true&width=600&lines=Production-Ready+Flask+App+%F0%9F%90%8D;Containerized+with+Docker+%F0%9F%90%B3;Deployed+Live+on+Render+%E2%98%81%EF%B8%8F;Clean+UI+%2B+RESTful+Architecture+%E2%9A%A1" alt="Typing SVG" />
</a>

<br/><br/>

<!-- Badges row 1 -->
[![Python](https://img.shields.io/badge/Python-3.10+-3776AB?style=for-the-badge&logo=python&logoColor=white)](https://python.org)
[![Flask](https://img.shields.io/badge/Flask-000000?style=for-the-badge&logo=flask&logoColor=white)](https://flask.palletsprojects.com)
[![Docker](https://img.shields.io/badge/Docker-2496ED?style=for-the-badge&logo=docker&logoColor=white)](https://docker.com)
[![Render](https://img.shields.io/badge/Render-46E3B7?style=for-the-badge&logo=render&logoColor=white)](https://quickmultiply.onrender.com)
[![MIT License](https://img.shields.io/badge/License-MIT-green?style=for-the-badge)](LICENSE)

<!-- Badges row 2 -->
[![GitHub stars](https://img.shields.io/github/stars/prithvicoder1/QuickMultiply?style=social)](https://github.com/prithvicoder1/QuickMultiply/stargazers)
[![GitHub forks](https://img.shields.io/github/forks/prithvicoder1/QuickMultiply?style=social)](https://github.com/prithvicoder1/QuickMultiply/network/members)
[![GitHub last commit](https://img.shields.io/github/last-commit/prithvicoder1/QuickMultiply?style=flat-square&color=7957d5)](https://github.com/prithvicoder1/QuickMultiply/commits/main)

<br/>

### 🔗 [**Try it Live → quickmultiply.onrender.com**](https://quickmultiply.onrender.com)

</div>

<br/>

<!-- Animated snake divider -->
<img src="https://raw.githubusercontent.com/andreasbm/readme/master/assets/lines/rainbow.png" width="100%"/>

<br/>

## 🧠 What is QuickMultiply?

<img align="right" width="300" src="https://user-images.githubusercontent.com/74038190/229223263-cf2e4b07-2615-4f87-9c38-e37600f8381a.gif"/>

**QuickMultiply** is a lightweight yet **production-grade** Flask web application that multiplies any set of numbers entered as a comma-separated list — and returns the result instantly.

But the real story isn't the math. It's the **full engineering pipeline** behind it:

- 🐍 Clean Flask REST endpoint with input validation
- 🐳 Containerized with Docker for zero-friction deployment
- ☁️ Live on Render — auto-deploys on every `git push`
- 🎨 Gradient UI with smooth hover animations
- 📱 Fully responsive across all screen sizes

<br clear="right"/>

<br/>

<img src="https://raw.githubusercontent.com/andreasbm/readme/master/assets/lines/colored.png" width="100%"/>

## ✨ Features

<div align="center">

| 🔢 Feature | 💬 Description |
|:---:|:---|
| **Multi-number input** | Enter any count of numbers separated by commas |
| **Float support** | Handles decimals like `1.5, 2.5, 4` seamlessly |
| **Smart output** | Displays whole numbers as integers, not floats |
| **Error handling** | Friendly messages for invalid or empty inputs |
| **Responsive UI** | Works beautifully on mobile, tablet, and desktop |
| **Dockerized** | Run anywhere with one `docker run` command |
| **Cloud deployed** | Live 24/7 on Render with zero manual ops |

</div>

<br/>

<img src="https://raw.githubusercontent.com/andreasbm/readme/master/assets/lines/colored.png" width="100%"/>

## 🛠️ Tech Stack

<div align="center">

<img src="https://skillicons.dev/icons?i=python,flask,docker,html,css,git,github&theme=dark" />

<br/><br/>

| Layer | Tool | Purpose |
|:---:|:---:|:---|
| **Backend** | ![Python](https://img.shields.io/badge/-Python-3776AB?logo=python&logoColor=white&style=flat-square) Flask | REST route, logic, template rendering |
| **Frontend** | ![HTML5](https://img.shields.io/badge/-HTML5-E34F26?logo=html5&logoColor=white&style=flat-square) ![CSS3](https://img.shields.io/badge/-CSS3-1572B6?logo=css3&logoColor=white&style=flat-square) | Inline via `render_template_string` |
| **Container** | ![Docker](https://img.shields.io/badge/-Docker-2496ED?logo=docker&logoColor=white&style=flat-square) | Environment consistency |
| **Deployment** | ![Render](https://img.shields.io/badge/-Render-46E3B7?logo=render&logoColor=white&style=flat-square) | Cloud hosting, auto-deploy |
| **Version Control** | ![GitHub](https://img.shields.io/badge/-GitHub-181717?logo=github&logoColor=white&style=flat-square) | Source code & CI/CD trigger |

</div>

<br/>

<img src="https://raw.githubusercontent.com/andreasbm/readme/master/assets/lines/colored.png" width="100%"/>

## 🔄 How It Works

```
┌─────────────────────────────────────────────────────┐
│                                                     │
│   User enters:  "2, 3, 4"  →  clicks Multiply      │
│                                                     │
└──────────────────────┬──────────────────────────────┘
                       │  HTTP POST /
                       ▼
┌─────────────────────────────────────────────────────┐
│              Flask Route Handler                    │
│                                                     │
│   1. Split by comma  →  ["2", "3", "4"]            │
│   2. Convert to float  →  [2.0, 3.0, 4.0]         │
│   3. Multiply iteratively  →  2 × 3 × 4 = 24.0    │
│   4. Whole number check  →  display as 24          │
│                                                     │
└──────────────────────┬──────────────────────────────┘
                       │
                       ▼
┌─────────────────────────────────────────────────────┐
│                                                     │
│        ✅  Result = 24  rendered on page            │
│                                                     │
└─────────────────────────────────────────────────────┘
```

> Invalid or empty input? The app catches it gracefully and shows a user-friendly error — no crashes, no stack traces.

<br/>

<img src="https://raw.githubusercontent.com/andreasbm/readme/master/assets/lines/colored.png" width="100%"/>

## 📂 Project Structure

```
📦 QuickMultiply/
│
├── 🐍  app.py               ← Flask app: routes, logic & HTML template
├── 📋  requirements.txt     ← Python dependencies (Flask)
├── 🐳  Dockerfile           ← Container build instructions
└── 📄  README.md            ← You are here!
```

<br/>

<img src="https://raw.githubusercontent.com/andreasbm/readme/master/assets/lines/colored.png" width="100%"/>

## ⚙️ Getting Started

### 🖥️ Run Locally

```bash
# 1. Clone the repo
git clone https://github.com/prithvicoder1/QuickMultiply.git
cd QuickMultiply

# 2. Install dependencies
pip install -r requirements.txt

# 3. Start the server
python app.py
```

> Open **http://localhost:5001** in your browser 🚀

---

### 🐳 Run with Docker

```bash
# Build the image
docker build -t quickmultiply .

# Run the container
docker run -p 5001:5001 quickmultiply
```

> Open **http://localhost:5001** — same result, zero Python setup needed.

<br/>

<img src="https://raw.githubusercontent.com/andreasbm/readme/master/assets/lines/colored.png" width="100%"/>

## ☁️ Deploy on Render

<div align="center">

```
GitHub Repo  ──push──▶  Render detects Dockerfile
                                    │
                                    ▼
                         Auto-build & deploy
                                    │
                                    ▼
                    🌐 Live at quickmultiply.onrender.com
```

</div>

**Steps to deploy your own:**

1. Push code to GitHub
2. Go to [render.com](https://render.com) → **New Web Service**
3. Connect your GitHub repo
4. Runtime: **Docker**
5. Click **Deploy** — done ✅

Every `git push` to `main` triggers a fresh deployment automatically.

<br/>

<img src="https://raw.githubusercontent.com/andreasbm/readme/master/assets/lines/colored.png" width="100%"/>

## 🤝 Contributing

```bash
# Fork → Clone → Branch → Commit → Push → PR
git checkout -b feature/your-feature
git commit -m "✨ Add your feature"
git push origin feature/your-feature
```

Then open a Pull Request on GitHub — all contributions are welcome!

<br/>

<img src="https://raw.githubusercontent.com/andreasbm/readme/master/assets/lines/colored.png" width="100%"/>

## 📄 License

Distributed under the **MIT License**. See [`LICENSE`](LICENSE) for details.

<br/>

<!-- Animated wave footer -->
<div align="center">

<img src="https://raw.githubusercontent.com/andreasbm/readme/master/assets/lines/rainbow.png" width="100%"/>

<!-- Visitor counter -->
![Visitor Count](https://profile-counter.glitch.me/prithvicoder1-QuickMultiply/count.svg)

<br/>

### Made with ❤️ by [Prithvi](https://github.com/prithvicoder1)

<img width="100%" src="https://capsule-render.vercel.app/api?type=waving&color=gradient&customColorList=6,11,20&height=120&section=footer"/>

</div>
