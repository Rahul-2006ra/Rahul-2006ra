<div align="center">

# Rahul R

**Software Developer · Information Science Engineering Student**

*Building systems that solve real problems — from disaster-response AI to computer vision game controllers.*

[![LinkedIn](https://img.shields.io/badge/LinkedIn-0077B5?style=for-the-badge&logo=linkedin&logoColor=white)](https://www.linkedin.com/in/rahul-r-737137338/)
[![GitHub](https://img.shields.io/badge/GitHub-181717?style=for-the-badge&logo=github&logoColor=white)](https://github.com/Rahul-2006ra)
[![Email](https://img.shields.io/badge/Email-D14836?style=for-the-badge&logo=gmail&logoColor=white)](mailto:rahulrkudlur@gmail.com)
[![EventSphere Live](https://img.shields.io/badge/Live_Demo-EventSphere-22c55e?style=for-the-badge&logo=vercel&logoColor=white)](https://event-sphere-flame.vercel.app)

</div>

---

## About Me

I'm an Information Science Engineering student who builds end-to-end software systems — not just prototypes. My projects span disaster-management AI (SIH 2026), forensic video intelligence, real-time event platforms, and computer vision game controllers. I work across the full stack: FastAPI and Node.js backends, React/TypeScript frontends, PostgreSQL and SQLite databases, and AI integration with Gemini, YOLOv8, and CLIP.

I approach engineering with an emphasis on honesty and traceability: every claim in my software is backed by verifiable data, every feature is tested, and every limitation is documented. I also enjoy applied mathematics — finding elegant shortcuts in patterns that appear complex.

Currently deepening my knowledge of distributed systems and computer vision.

---

## Tech Stack

**Languages**

![Python](https://img.shields.io/badge/Python-3776AB?style=flat-square&logo=python&logoColor=white)
![JavaScript](https://img.shields.io/badge/JavaScript-F7DF1E?style=flat-square&logo=javascript&logoColor=black)
![TypeScript](https://img.shields.io/badge/TypeScript-3178C6?style=flat-square&logo=typescript&logoColor=white)
![Java](https://img.shields.io/badge/Java-ED8B00?style=flat-square&logo=openjdk&logoColor=white)
![C](https://img.shields.io/badge/C-00599C?style=flat-square&logo=c&logoColor=white)
![HTML5](https://img.shields.io/badge/HTML5-E34F26?style=flat-square&logo=html5&logoColor=white)
![CSS3](https://img.shields.io/badge/CSS3-1572B6?style=flat-square&logo=css3&logoColor=white)

**Backend & APIs**

![FastAPI](https://img.shields.io/badge/FastAPI-009688?style=flat-square&logo=fastapi&logoColor=white)
![Node.js](https://img.shields.io/badge/Node.js-339933?style=flat-square&logo=nodedotjs&logoColor=white)
![Express.js](https://img.shields.io/badge/Express.js-000000?style=flat-square&logo=express&logoColor=white)
![Flask](https://img.shields.io/badge/Flask-000000?style=flat-square&logo=flask&logoColor=white)
![Socket.IO](https://img.shields.io/badge/Socket.IO-010101?style=flat-square&logo=socketdotio&logoColor=white)

**Frontend**

![React](https://img.shields.io/badge/React-20232A?style=flat-square&logo=react&logoColor=61DAFB)
![Vite](https://img.shields.io/badge/Vite-646CFF?style=flat-square&logo=vite&logoColor=white)
![Tailwind CSS](https://img.shields.io/badge/Tailwind_CSS-38B2AC?style=flat-square&logo=tailwind-css&logoColor=white)

**Databases**

![PostgreSQL](https://img.shields.io/badge/PostgreSQL-316192?style=flat-square&logo=postgresql&logoColor=white)
![SQLite](https://img.shields.io/badge/SQLite-07405E?style=flat-square&logo=sqlite&logoColor=white)
![Prisma](https://img.shields.io/badge/Prisma-2D3748?style=flat-square&logo=prisma&logoColor=white)

**AI & Computer Vision**

![OpenCV](https://img.shields.io/badge/OpenCV-5C3EE8?style=flat-square&logo=opencv&logoColor=white)
![MediaPipe](https://img.shields.io/badge/MediaPipe-0097A7?style=flat-square&logo=google&logoColor=white)
![YOLOv8](https://img.shields.io/badge/YOLOv8-00FFFF?style=flat-square&logo=yolo&logoColor=black)
![Gemini AI](https://img.shields.io/badge/Gemini_AI-4285F4?style=flat-square&logo=google&logoColor=white)
![Qdrant](https://img.shields.io/badge/Qdrant-DC382D?style=flat-square&logo=redis&logoColor=white)

**DevOps & Tools**

![Docker](https://img.shields.io/badge/Docker-2496ED?style=flat-square&logo=docker&logoColor=white)
![Git](https://img.shields.io/badge/Git-F05032?style=flat-square&logo=git&logoColor=white)
![Linux](https://img.shields.io/badge/Linux-FCC624?style=flat-square&logo=linux&logoColor=black)
![VS Code](https://img.shields.io/badge/VS_Code-007ACC?style=flat-square&logo=visualstudiocode&logoColor=white)
![Pytest](https://img.shields.io/badge/Pytest-0A9EDC?style=flat-square&logo=pytest&logoColor=white)
![FFmpeg](https://img.shields.io/badge/FFmpeg-007808?style=flat-square&logo=ffmpeg&logoColor=white)
![Nginx](https://img.shields.io/badge/Nginx-009639?style=flat-square&logo=nginx&logoColor=white)

---

## Featured Projects

### 🌩️ SkySafe AI — Disaster Alert Intelligence Platform

> SIH 2026 · Problem SIH26068 (Weather + Disaster Management)

Turns government CAP 1.2 weather alerts (NDMA SACHET / IMD) into verified, multilingual, citizen-ready voice and SMS actions — with a live command center for officials.

**The engineering challenge:** LLMs hallucinate. In disaster communication, a wrong wind speed or evacuate direction can cost lives. SkySafe solves this with a zero-hallucination pipeline: every fact gets a stable ID from a deterministically built FactSheet. The LLM may only *select* and *rephrase* those facts — never invent new ones. A grounding validator checks every numeral, date, place, and severity word in the output against the original feed. Any mismatch triggers a retry, then a template fallback that operates with no LLM at all.

**Key features:**
- CAP 1.2 XML feed ingestion (real NDMA SACHET + IMD feeds in live mode)
- FactSheet → ActionPlan → LLM → Grounding Validator → Template Fallback pipeline
- Claim Ledger: every citizen message shows a ✅ badge proving what was verified and from where
- Citizen Progressive Web App with offline support
- Command center with risk-score-based resource allocation optimizer
- Multilingual broadcast (text, voice, SMS/WhatsApp via Twilio)
- Docker Compose deployment; 308 backend tests pass with no API key

**Stack:** Python · FastAPI · TypeScript · Next.js · SQLite/Postgres · Docker · Gemini AI · Open-Meteo · Twilio  
📁 [Rahul-2006ra/SkySafe-AI](https://github.com/Rahul-2006ra/SkySafe-AI)

---

### 🎥 CamTrace Intelligence — Multi-Vendor DVR/NVR Forensic Platform

> SIH 2026 · Problem SIH26150 · Team Phoenix (Rahul R — full-stack engineering & forensic pipeline)

A functional local forensic workflow for investigators who receive CCTV evidence from different DVR/NVR brands with inconsistent formats, clock drift, and potential deleted footage.

**The engineering challenge:** Real DVR forensics is messy — vendors use different index formats (JSON, XML, binary, CSV), cameras drift in time, and deleted recordings may be partially recoverable from FAT images. CamTrace implements a real FAT16 directory parser that reads deleted file entries directly from disk images, normalizes timestamps with signed clock-correction records, and runs each recovered clip through a YOLOv8+ByteTrack+CLIP pipeline for semantic search.

**Key features:**
- Case-based evidence intake with MD5+SHA-256 hash verification
- Real FAT16 deleted file recovery from controlled forensic disk images
- AI-assisted search: describe a scene in plain language, retrieve matching clips
- Chain-of-custody audit log with hash-chained events
- PDF report generation from case state (findings, hashes, selected clips, limitations)
- 39 backend tests · 3 Playwright browser workflow tests · production build validated

**Stack:** Python · FastAPI · React · TypeScript · Vite · YOLOv8 · CLIP · Qdrant · FFmpeg · SQLite · Docker · Playwright  
📁 [Rahul-2006ra/SIH26150-Prototype](https://github.com/Rahul-2006ra/SIH26150-Prototype)

---

### 🎟️ EventSphere — Real-Time AI Event Management Platform

A production-deployed event management platform with live ticketing, Razorpay payments, QR check-in, and Gemini-powered AI features.

**The engineering challenge:** Coordinating a live check-in at an event with hundreds of attendees requires real-time synchronization across multiple organizer dashboards simultaneously. EventSphere uses Socket.IO with scoped rooms — each event has its own room, each organizer dashboard subscribes independently — so a QR scan instantly updates the attendee count, check-in feed, and revenue chart for all connected clients without polling.

**Key features:**
- JWT auth with role-based access (Organizer / Attendee)
- Razorpay payment flow with server-side signature verification
- QR code generation and scan-to-check-in validation
- Live Socket.IO: attendee counts, check-ins, dashboard updates, notifications
- Gemini AI: event description generator, schedule builder, personalized recommendations
- Node.js + Express + Prisma backend · Flask AI microservice · Nginx reverse proxy
- PM2 process management · AWS EC2 deployment ready

**Stack:** Node.js · Express · Prisma · PostgreSQL · Socket.IO · Python · Flask · Gemini AI · Razorpay · Nginx · HTML/CSS/JS  
📁 [Rahul-2006ra/EventSphere](https://github.com/Rahul-2006ra/EventSphere) · 🌐 [Live Demo](https://event-sphere-flame.vercel.app)

---

### 🖐️ Hand Gesture Controller — Touchless Game Input via Computer Vision

Controls keyboard-based games (Temple Run, Subway Surfers) using real-time hand gesture recognition from a standard webcam — no controller, no keyboard.

**The engineering challenge:** Detecting a "swipe" from raw landmark coordinates is harder than it looks. Single-frame position is too noisy; fingertips jitter constantly. Instead, the system tracks the *palm center* (average of wrist and middle-finger-base landmarks, two stable points) over a 0.35s rolling buffer. A swipe fires when displacement exceeds a tunable threshold *and* velocity clears a minimum — which means slow drifts don't trigger, only intentional movements do. A 0.45s cooldown after each keypress prevents one gesture from cascading into five.

**Key features:**
- 21-landmark hand detection with MediaPipe Hands
- Velocity-threshold swipe detection with rolling buffer (configurable in `config.py`)
- Input routing via `pydirectinput` for OS-level keystrokes
- Modular architecture: hand tracker, gesture detector, input controller are independent files
- Includes test suite (`test_gesture_detector.py`) and tuning guide

**Stack:** Python · OpenCV · MediaPipe · PyDirectInput  
📁 [Rahul-2006ra/Hand-Gesture-Temple-Run-Name](https://github.com/Rahul-2006ra/Hand-Gesture-Temple-Run-Name)

---

### 🔢 10-Number Math Hack — Fast Consecutive Sum Trick

A personal mathematical discovery: any 10 consecutive numbers can be summed instantly as `(average of the two middle numbers) × 10` — no step-by-step addition.

This works because consecutive integers form an arithmetic progression where every pair equidistant from the center sums to the same value. The two middle numbers' average equals the series mean, and multiplying by 10 applies that mean to all terms simultaneously.

📁 [Rahul-2006ra/10---Numbers-Math-Hack-Trick-](https://github.com/Rahul-2006ra/10---Numbers-Math-Hack-Trick-)

---

## Also Worth Exploring

| Project | Description |
|---|---|
| [Ravanger-Subway-Escape](https://github.com/Rahul-2006ra/Ravanger-Subway-Escape) | AI bot using graph algorithms and strategic pathfinding — built for an AI × Maths Hackathon |
| [AI-Resume-Analyzer](https://github.com/Rahul-2006ra/AI-Resume-Analyzer) | ATS score optimizer with keyword detection and improvement recommendations |
| [Eco-Track-Carbon-Footprint-Analyzer](https://github.com/Rahul-2006ra/Eco-Track-Carbon-Footprint-Analyzer) | Daily carbon footprint calculator with actionable reduction tips |
| [Smart-Disaster-Alert-And-Safety-Recomandation](https://github.com/Rahul-2006ra/Smart-Disaster-Alert-And-Safety-Recomandation) | Web app for real-time disaster type detection and safety guidance |

---

## GitHub Activity

<div align="center">

[![Rahul's GitHub Stats](https://github-readme-stats.vercel.app/api?username=Rahul-2006ra&show_icons=true&theme=github_dark&hide_border=true&include_all_commits=true&count_private=false)](https://github.com/Rahul-2006ra)

[![Top Languages](https://github-readme-stats.vercel.app/api/top-langs/?username=Rahul-2006ra&layout=compact&theme=github_dark&hide_border=true&langs_count=8)](https://github.com/Rahul-2006ra)

*Stats powered by [github-readme-stats](https://github.com/anuradhkumar26/github-readme-stats) — if widgets are unavailable, visit the [profile directly](https://github.com/Rahul-2006ra).*

</div>

---

## Connect

I'm open to internship opportunities, collaborations, and technical conversations.

| Platform | Link |
|---|---|
| 💼 LinkedIn | [linkedin.com/in/rahul-r-737137338](https://www.linkedin.com/in/rahul-r-737137338/) |
| 📧 Email | [rahulrkudlur@gmail.com](mailto:rahulrkudlur@gmail.com) |
| 💻 GitHub | [github.com/Rahul-2006ra](https://github.com/Rahul-2006ra) |

---

<div align="center">

*I build things that are honest about what they do — and clear about what they don't.*

</div>
