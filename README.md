<div align="center">

# Hey there, I'm Anurag Dubey 👋

### Full-Stack Developer · System Builder · Problem Solver

[![Portfolio](https://img.shields.io/badge/🌐_Portfolio-Visit-4F46E5?style=for-the-badge)](https://portfolio-iamanu26.vercel.app/)
[![LeetCode](https://img.shields.io/badge/LeetCode-320+_Problems-FFA116?style=for-the-badge&logo=leetcode&logoColor=white)](https://leetcode.com/u/iamanu26_/)
[![LinkedIn](https://img.shields.io/badge/LinkedIn-Connect-0A66C2?style=for-the-badge&logo=linkedin&logoColor=white)](https://linkedin.com)

</div>

---

I build **real-world, scalable systems** — real-time platforms, backend architectures, authentication systems, and AI-assisted decision engines.

My focus is **end-to-end ownership**: designing, building, deploying, and clearly explaining systems from first principles.

---

## 🛠️ Tech Stack

<div align="center">

**Languages**

![JavaScript](https://img.shields.io/badge/JavaScript-F7DF1E?style=flat-square&logo=javascript&logoColor=black)
![Python](https://img.shields.io/badge/Python-3776AB?style=flat-square&logo=python&logoColor=white)
![C++](https://img.shields.io/badge/C++-00599C?style=flat-square&logo=cplusplus&logoColor=white)

**Frontend**

![HTML5](https://img.shields.io/badge/HTML5-E34F26?style=flat-square&logo=html5&logoColor=white)
![CSS3](https://img.shields.io/badge/CSS3-1572B6?style=flat-square&logo=css3&logoColor=white)
![React](https://img.shields.io/badge/React-61DAFB?style=flat-square&logo=react&logoColor=black)

**Backend**

![Node.js](https://img.shields.io/badge/Node.js-339933?style=flat-square&logo=nodedotjs&logoColor=white)
![Express](https://img.shields.io/badge/Express-000000?style=flat-square&logo=express&logoColor=white)
![Flask](https://img.shields.io/badge/Flask-000000?style=flat-square&logo=flask&logoColor=white)
![FastAPI](https://img.shields.io/badge/FastAPI-009688?style=flat-square&logo=fastapi&logoColor=white)
![Socket.IO](https://img.shields.io/badge/Socket.IO-010101?style=flat-square&logo=socketdotio&logoColor=white)

**Databases & Cloud**

![MongoDB](https://img.shields.io/badge/MongoDB-47A248?style=flat-square&logo=mongodb&logoColor=white)
![SQL Server](https://img.shields.io/badge/SQL_Server-CC2927?style=flat-square&logo=microsoftsqlserver&logoColor=white)
![Vercel](https://img.shields.io/badge/Vercel-000000?style=flat-square&logo=vercel&logoColor=white)
![Render](https://img.shields.io/badge/Render-46E3B7?style=flat-square&logo=render&logoColor=black)

**AI / ML**

![PyTorch](https://img.shields.io/badge/PyTorch-EE4C2C?style=flat-square&logo=pytorch&logoColor=white)
![Stable Baselines3](https://img.shields.io/badge/Stable--Baselines3-PPO-8B5CF6?style=flat-square)
![Gymnasium](https://img.shields.io/badge/Gymnasium-RL_Env-0081A7?style=flat-square)
![Groq](https://img.shields.io/badge/Groq-LLaMA_3.1-F54E00?style=flat-square)

</div>

---


## 📊 GitHub Stats

<div align="center">

<img src="https://github-readme-stats.vercel.app/api?username=iamanu26&show_icons=true&theme=tokyonight&hide_border=true&count_private=true" height="165" />
<img src="https://github-readme-streak-stats.herokuapp.com/?user=iamanu26&theme=tokyonight&hide_border=true" height="165" />

<br/>

<img src="https://github-readme-stats.vercel.app/api/top-langs/?username=iamanu26&layout=compact&theme=tokyonight&hide_border=true" height="140" />

</div>

---

## 🚀 Featured Projects

### 🚆 ChanakyanRail — AI-Powered Railway Digital Twin

> *"The master strategist doesn't react to chaos — he prevents it."*
> ChanakyanRail is a real-time digital twin of a railway network, where a Reinforcement Learning agent acts as the strategic mind — continuously analyzing 10 live trains and issuing intelligent speed & routing advisories to prevent collisions and eliminate delays before they cascade.

[![Live Demo](https://img.shields.io/badge/Live_Demo-000000?style=flat-square&logo=vercel)](https://railway-simulation.vercel.app)
[![Backend](https://img.shields.io/badge/Backend-Render-46E3B7?style=flat-square&logo=render&logoColor=black)](https://railway-simulation.onrender.com)
[![AI Engine](https://img.shields.io/badge/AI_Engine-Render-46E3B7?style=flat-square&logo=render&logoColor=black)](https://railway-ai-brain.onrender.com)

**What makes it interesting:**
- 🧠 **Custom RL Environment** — built a `RailwayEnv` class from scratch following the Gymnasium API standard, with a carefully tuned reward function: `+100` for route completion, `+10` per segment, `-200` for collision, and micro-penalties per timestep to keep trains moving efficiently
- 🤖 **PPO Agent trained for 500K timesteps** on Google Colab (free GPU) — the AI learned emergent strategies to balance speed vs. safety across all 10 trains simultaneously using a `MultiDiscrete` action space (HOLD / SLOW / NORMAL / FAST / REROUTE)
- 🔄 **Real-time multi-user sync** via Socket.IO Rooms (<50ms latency) — Station Masters see the global map; Loco Pilots receive only their targeted data packets
- 🗺️ **SVG-based live simulation** — trains are animated along `<path>` elements using `getPointAtLength()`, not a game engine — pure DOM + SVG
- 📡 **Decoupled microservices architecture** — frontend (Vercel) → Node.js orchestrator (Render) → Flask AI brain (Render), communicating over REST + WebSockets
- 🚨 Emergency stop interrupts that propagate instantly to the control center

`Vanilla JS` `SVG` `Node.js` `Socket.IO` `Python` `Flask` `PyTorch` `Stable-Baselines3` `Gymnasium` `Vercel` `Render`

---

### 🎙️ MockHire AI — AI-Powered Mock Interview Platform

> A full-stack voice-driven interview simulator that conducts real Technical & HR interviews using AI, scores your performance, and includes a LeetCode-style DSA practice module.

**What makes it interesting:**
- 🗣️ **Full voice interview loop** — AI speaks questions via speech synthesis, listens to spoken answers via Web Speech API, and asks intelligent follow-ups in real time — no typing required
- 📊 **AI performance reports** — after each session, generates a detailed scorecard across Communication, Confidence, Technical Skills, Grammar & Overall with written strength/weakness analysis
- 💻 **DSA Practice Module** — AI generates 3 fresh problems (Easy / Medium / Hard) per session; users submit solutions in Python, C++, Java, or JavaScript and get AI feedback on correctness + time/space complexity
- 🔐 **JWT auth + per-user history** — sessions are isolated, scores always reflect the current interview only
- 🛠️ **Engineering depth** — solved shared agent state bugs, built a custom JSON parser to handle LLaMA's inconsistent output formats (markdown fences, `"7/10"` strings), and engineered strict scoring prompts with server-side caps to prevent inflated scores

`React (Vite)` `FastAPI` `Python` `SQLAlchemy` `SQLite` `JWT` `LLaMA 3.1` `Groq API` `Web Speech API`

---

### 🏢 Prominix Limited — IT Solutions Platform *(Frontend)*

> Built the complete frontend for a startup-style IT services platform — public-facing website and a secure internal developer dashboard.

**What makes it interesting:**
- ⚡ Architected with **React + Vite** for fast load times and optimized bundle size
- 🧭 Multi-page navigation built with **React Router** for a seamless SPA experience
- 🎨 Fully custom UI with polished CSS — designed to connect cleanly with an ASP.NET Core + SQL Server backend

`React (Vite)` `React Router` `Bootstrap` `Custom CSS`

---

### 📺 YouTube Backend System

> A production-grade backend replicating core features of a video streaming platform — built for scale and security.

**What makes it interesting:**
- 🔐 Dual-token auth with **JWT Access + Refresh Tokens** and secure session management
- ☁️ **Cloudinary** integration for video and image asset management
- 🏗️ Clean, RESTful API design modeled after real-world streaming architecture

`Node.js` `Express.js` `MongoDB` `JWT` `Cloudinary` `REST APIs`

---

## 🏆 Achievements

| 🏅 Achievement | Details |
|---|---|
| 💻 **LeetCode** | 320+ DSA problems solved · [iamanu26_](https://leetcode.com/u/iamanu26_/) |
| 🏛️ **Best Parliamentary Award** | GLBMUN |
| 🏆 **Smart India Hackathon 2025** | Participant |
| ⚽ **Secretary**, Sports Club | GL Bajaj Institute · 2025–26 |
| 🎨 **Design & Creative Lead**, Sports Club | GL Bajaj Institute · 2024–25 |

---

<div align="center">

**Thanks for stopping by — feel free to explore my work or reach out!**

[![Portfolio](https://img.shields.io/badge/🌐_portfolio--iamanu26.vercel.app-4F46E5?style=for-the-badge)](https://portfolio-iamanu26.vercel.app/)

</div>
