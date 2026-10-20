# Hi, I'm Maruf Aurnap 👋

Cornell undergrad building AI-powered tools for the real world. I work across machine learning and full-stack development, from training models to shipping the interfaces people actually use.

## Tech Stack

**Languages**
![Python](https://img.shields.io/badge/-Python-3776AB?style=flat-square&logo=python&logoColor=white)
![JavaScript](https://img.shields.io/badge/-JavaScript-F7DF1E?style=flat-square&logo=javascript&logoColor=black)
![TypeScript](https://img.shields.io/badge/-TypeScript-3178C6?style=flat-square&logo=typescript&logoColor=white)
![Swift](https://img.shields.io/badge/-Swift-F05138?style=flat-square&logo=swift&logoColor=white)
![C#](https://img.shields.io/badge/-C%23-512BD4?style=flat-square&logo=dotnet&logoColor=white)
![HTML5](https://img.shields.io/badge/-HTML5-E34F26?style=flat-square&logo=html5&logoColor=white)
![CSS3](https://img.shields.io/badge/-CSS3-1572B6?style=flat-square&logo=css3&logoColor=white)

**Frontend**
![React](https://img.shields.io/badge/-React-61DAFB?style=flat-square&logo=react&logoColor=black)
![Next.js](https://img.shields.io/badge/-Next.js-black?style=flat-square&logo=next.js&logoColor=white)
![Three.js](https://img.shields.io/badge/-Three.js-black?style=flat-square&logo=threedotjs&logoColor=white)

**Backend & Cloud**
![FastAPI](https://img.shields.io/badge/-FastAPI-009688?style=flat-square&logo=fastapi&logoColor=white)
![Firebase](https://img.shields.io/badge/-Firebase-FFCA28?style=flat-square&logo=firebase&logoColor=black)

**Mobile & AR**
![Unity](https://img.shields.io/badge/-Unity-black?style=flat-square&logo=unity&logoColor=white)
![ARKit](https://img.shields.io/badge/-ARKit%20%2F%20RoomPlan-000000?style=flat-square&logo=apple&logoColor=white)

**ML & AI**
![PyTorch](https://img.shields.io/badge/-PyTorch-EE4C2C?style=flat-square&logo=pytorch&logoColor=white)
![TensorFlow](https://img.shields.io/badge/-TensorFlow-FF6F00?style=flat-square&logo=tensorflow&logoColor=white)
![Scikit-Learn](https://img.shields.io/badge/-Scikit--Learn-F7931E?style=flat-square&logo=scikit-learn&logoColor=white)
![Hugging Face](https://img.shields.io/badge/-Hugging%20Face-FCC624?style=flat-square&logo=huggingface&logoColor=black)
![LangGraph](https://img.shields.io/badge/-LangGraph-1C3C3C?style=flat-square)
![Gemini](https://img.shields.io/badge/-Gemini-8E75B2?style=flat-square&logo=googlegemini&logoColor=white)

**Tools**
![Playwright](https://img.shields.io/badge/-Playwright-2EAD33?style=flat-square&logo=playwright&logoColor=white)
![axe-core](https://img.shields.io/badge/-axe--core-6E3FA3?style=flat-square)
![Git](https://img.shields.io/badge/-Git-F05032?style=flat-square&logo=git&logoColor=white)
![GitHub](https://img.shields.io/badge/-GitHub-black?style=flat-square&logo=github&logoColor=white)

## Projects

### [Gnarly](https://github.com/mukundgaur/gnarly)
*LiDAR indoor navigation for iPhone: scan a building, edit the map on the web, and navigate it in AR.*

- **Mapping:** A Swift app uses RoomPlan and ARKit to capture room geometry and an ARWorldMap, then turns walls, doors, and openings into a walkable visibility graph.
- **Navigation:** A Unity 6 iOS app relocalizes against the map and draws the route in the camera view. Routing handles multiple zones and floors, with elevator rides weighted as a walking-equivalent cost (A\* in Unity, Dijkstra on the web).
- **Haptics:** ARKit scene depth drives Taptic Engine cues for direction and obstacle proximity (closer means stronger).
- **Backend & editor:** A TypeScript publish API verifies Firebase auth, validates packages against a JSON schema, and switches map versions in a single Firestore transaction, so a failed upload never breaks the live map. A React + Three.js editor arranges zones, waypoints, and floors.

**Stack:** Swift · Unity · ARKit · RoomPlan · TypeScript · React · Three.js · Firebase

### [SecondSight](https://github.com/marnan4/SecondSight)
*An autonomous AI agent that audits live web apps, fixes accessibility violations, and opens verified GitHub pull requests.*

- Targets WCAG violations that affect ~95% of the top 1M websites.
- Multi-stage LLM agent pipeline (audit → map → code → verify → PR) that generates targeted fixes and validates each one with automated re-scans.
- Real-time dashboard that streams agent logs and produces minimal, reviewable diffs.

**Stack:** Python · LangGraph · Playwright · axe-core · Gemini · Next.js · FastAPI · Server-Sent Events

### [Predictive Gas Pump Maintenance](https://github.com/marnan4/Accenture-2C-Predictive-Maintenance-for-Oil-Gas-Pump-Operation)
*End-to-end ML lifecycle for predicting pump failures, built with a 7-member fellowship team.*

- Trained and compared Logistic Regression, Random Forest, Gradient Boosted Trees, MLP, and LSTM models on 720,000+ sensor records.
- Selected a regularized Logistic Regression model with 100% precision and recall, projecting a 50% reduction in unplanned downtime (~$1.3M saved over 100 days).
- Shipped a FastAPI demo that serves real-time failure predictions to a live pump monitoring dashboard.

**Stack:** Python · scikit-learn · PyTorch · FastAPI

### [Free-Scribe](https://github.com/marnan4/free-scribe)
*Multilingual transcription and translation that runs entirely in the browser.*

- Built with React, using Whisper (via Transformers.js) for transcription and NLLB-200 for translation across 200 languages.
- Runs inference client-side in Web Workers, so the UI never blocks and no audio leaves the device.

**Stack:** React · Whisper · NLLB-200 · Web Workers

### [Email Spam Detector](https://colab.research.google.com/drive/1gMOGZT8XWAj4hKewcOthNSVbQQwdscUW#scrollTo=1tGoIHEmdzGi)
*Fine-tuned BERT classifier that flags spam from raw email text.*

- Tokenized and preprocessed data with Hugging Face Transformers; built training, validation, and evaluation pipelines in PyTorch.
- Reached up to 98% across accuracy, precision, recall, and F1.

### Other
- [NASA React App](https://github.com/marnan4/nasa-react-app): React app showing NASA APOD data and imagery through NASA's APIs.
