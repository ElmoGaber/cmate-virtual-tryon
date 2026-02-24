# CMate Virtual Try-On

![License](https://img.shields.io/badge/License-MIT-yellow.svg)
![Python](https://img.shields.io/badge/Python-3.10%2B-blue)
![Docker](https://img.shields.io/badge/Docker-Ready-blue)
![HTML5](https://img.shields.io/badge/HTML5-Ready-orange)

**An AI-powered virtual clothing try-on system** that lets users upload their photo and instantly see how any garment looks on them — no changing room needed.

---

## ✨ Features

- **Real-time Virtual Try-On**: Upload a person photo + clothing image and get photorealistic results in seconds.
- **Web-Based Interface**: Clean, responsive UI built with HTML, CSS, and JavaScript.
- **Docker Ready**: One-command deployment with full environment isolation.
- **High-Quality Output**: Powered by state-of-the-art computer vision and generative models.
- **Multi-Platform Support**: Works on desktop, tablet, and mobile browsers.
- **Easy Integration**: REST API endpoints for easy connection with e-commerce platforms.
- **Batch Processing**: Try multiple outfits at once.

---

## 🛠 Tech Stack

- **Backend**: Python 3.10+
- **Framework**: FastAPI / Flask (modular structure in `/src`)
- **AI Models**: Virtual Try-On (VITON-HD style) + Pose Estimation + GAN-based rendering
- **Frontend**: HTML5 + Tailwind CSS + vanilla JS
- **Containerization**: Docker + Dockerfile
- **Dependencies**: Managed via `requirements.txt` and `setup.py`
- **Documentation**: Full docs in `/docs` folder

---

## 🚀 Quick Start

### Using Docker (Recommended)

```bash
# Clone the repo
git clone https://github.com/ElmoGaber/cmate-virtual-tryon.git
cd cmate-virtual-tryon
```
# Build and run
```
docker build -t cmate-virtual-tryon .
docker run -p 8000:8000 cmate-virtual-tryon
Open your browser → http://localhost:8000
Local Installation
```
```Bash# Clone
git clone https://github.com/ElmoGaber/cmate-virtual-tryon.git
cd cmate-virtual-tryon
```

# Create virtual environment
```
python -m venv venv
source venv/bin/activate    # Windows: venv\Scripts\activate
```

# Install dependencies
```
pip install -r requirements.txt
pip install -e .
```

# Run the app
```
python src/main.py
```

📸 Screenshots
(Add your screenshots here in the /docs/images folder and they will appear automatically)
<img src="docs/images/demo1.png" alt="Demo 1">
<img src="docs/images/demo2.png" alt="Demo 2">

📖 API Documentation
Full Swagger UI available at /docs when the server is running.
Key endpoints:
```
POST /tryon → Main try-on endpoint
POST /upload/person → Upload person photo
POST /upload/cloth → Upload clothing image
GET /health → Health check
```
```
📁 Project Structure
textcmate-virtual-tryon/
├── src/                 # Main source code
├── docs/                # Documentation & images
├── .idea/               # IDE settings
├── .gitattributes
├── .gitignore
├── Dockerfile
├── LICENSE
├── README.md
├── requirements.txt
├── setup.py
└── ...
```



📄 License
This project is licensed under the MIT License — see the LICENSE file for details.

🙏 Acknowledgments

Inspired by cutting-edge research in virtual try-on (VITON, CP-VTON, etc.)
Thanks to the open-source community for all the amazing computer vision tools
Special thanks to everyone who helped test the early versions
