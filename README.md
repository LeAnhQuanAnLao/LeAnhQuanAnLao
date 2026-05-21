<div align="center">

<img src="https://readme-typing-svg.demolab.com?font=Fira+Code&size=24&duration=3200&pause=900&color=38B2AC&center=true&vCenter=true&width=620&lines=Hi%2C+I'm+Le+Anh+Quan;Full-Stack+Engineer+%E2%80%94+Backend-First;Laravel+%2B+Python+%2B+Industrial+AI;I+ship+real-time+systems+that+touch+real+factories" alt="Typing banner" />

### 🏭 Engineering Resilient Systems · Synchronizing Hardware with Real-Time Data

<a href="mailto:leanhquan.work@email.com"><img src="https://img.shields.io/badge/Email-D14836?style=for-the-badge&logo=gmail&logoColor=white" /></a>
<a href="https://github.com/LeAnhQuanAnLao"><img src="https://img.shields.io/badge/GitHub-181717?style=for-the-badge&logo=github&logoColor=white" /></a>
<img src="https://img.shields.io/badge/Location-Ho_Chi_Minh_City%2C_VN-0A66C2?style=for-the-badge&logo=googlemaps&logoColor=white" />
<img src="https://img.shields.io/badge/Open_to-Technical_Challenges-2EA44F?style=for-the-badge" />

</div>

---

## 👨‍💻 About Me

I'm a **Full-Stack Engineer with a Backend bias**, building mission-critical systems where the database, the production line, and the camera on the warehouse door all have to agree on the same source of truth — in real time.

My day-to-day is **Laravel + Python**, but my real job is *closing the gap between digital state and physical operations*: synchronizing live machine telemetry, debt-code / pre-night carry-over logic, AI-driven QR/vision pipelines, and stored-procedure-heavy ERP workflows. I treat the database as a first-class citizen, run my own **bare-metal Linux & Windows servers** (no WSL), and keep my Python strictly **PEP 8** and my Laravel code in clean, predictable design patterns.

What I care about:

- **Correctness under load** — production lines don't tolerate "eventually consistent."
- **Lean abstractions** — Pythonic, idiomatic, no over-engineered ceremony.
- **Real ownership** — I deploy what I build; the server, the cron, the SMTP relay, all of it.

---

## 🛠️ Core Expertise

<table>
<tr>
<td valign="top" width="50%">

#### 🔧 Backend
![PHP](https://img.shields.io/badge/PHP-777BB4?style=flat-square&logo=php&logoColor=white)
![Laravel](https://img.shields.io/badge/Laravel_11%2F12-FF2D20?style=flat-square&logo=laravel&logoColor=white)
![Python](https://img.shields.io/badge/Python_3.11-3776AB?style=flat-square&logo=python&logoColor=white)
![Django](https://img.shields.io/badge/Django_5.2-092E20?style=flat-square&logo=django&logoColor=white)
![Flask](https://img.shields.io/badge/Flask-000000?style=flat-square&logo=flask&logoColor=white)
![Node.js](https://img.shields.io/badge/Node.js-339933?style=flat-square&logo=node.js&logoColor=white)
![Express](https://img.shields.io/badge/Express-000000?style=flat-square&logo=express&logoColor=white)

#### 🎨 Frontend
![React](https://img.shields.io/badge/React_18-20232A?style=flat-square&logo=react&logoColor=61DAFB)
![JavaScript](https://img.shields.io/badge/JavaScript-F7DF1E?style=flat-square&logo=javascript&logoColor=black)
![TailwindCSS](https://img.shields.io/badge/Tailwind-38B2AC?style=flat-square&logo=tailwindcss&logoColor=white)
![Mantine](https://img.shields.io/badge/Mantine-339AF0?style=flat-square&logo=mantine&logoColor=white)
![Blade](https://img.shields.io/badge/Blade-F05340?style=flat-square&logo=laravel&logoColor=white)

</td>
<td valign="top" width="50%">

#### 🗄️ Data & Architecture
![SQL Server](https://img.shields.io/badge/SQL_Server-CC2927?style=flat-square&logo=microsoftsqlserver&logoColor=white)
![MySQL](https://img.shields.io/badge/MySQL-4479A1?style=flat-square&logo=mysql&logoColor=white)
![SQLite](https://img.shields.io/badge/SQLite-003B57?style=flat-square&logo=sqlite&logoColor=white)
![Eloquent](https://img.shields.io/badge/Eloquent_ORM-FF2D20?style=flat-square&logo=laravel&logoColor=white)
![SQLAlchemy](https://img.shields.io/badge/SQLAlchemy-D71F00?style=flat-square&logo=python&logoColor=white)

> *Stored-procedure orchestration · cross-DB linked queries · Base36 ID encoding · MARS pyodbc tuning*

#### ⚙️ Infrastructure & AI
![Linux](https://img.shields.io/badge/Linux_Bare--Metal-FCC624?style=flat-square&logo=linux&logoColor=black)
![Windows](https://img.shields.io/badge/Windows_Server-0078D6?style=flat-square&logo=windows&logoColor=white)
![PM2](https://img.shields.io/badge/PM2-2B037A?style=flat-square&logo=pm2&logoColor=white)
![Docker](https://img.shields.io/badge/Docker-2496ED?style=flat-square&logo=docker&logoColor=white)
![NVIDIA](https://img.shields.io/badge/CUDA_12.1-76B900?style=flat-square&logo=nvidia&logoColor=white)
![Gemini](https://img.shields.io/badge/Gemini_API-8E75B2?style=flat-square&logo=google&logoColor=white)
![YOLO](https://img.shields.io/badge/YOLOv8-00FFFF?style=flat-square&logo=yolo&logoColor=black)
![OpenCV](https://img.shields.io/badge/OpenCV-5C3EE8?style=flat-square&logo=opencv&logoColor=white)

</td>
</tr>
</table>

---

## 🚀 Featured Projects

### 🎯 Smart Trolley Vision — Industrial CV + Active Learning
> *Python · Flask-SocketIO · YOLOv8 · OpenCV · pyzbar · PyTorch (CUDA 12.1) · React · SQL Server*

An end-to-end computer-vision platform that watches warehouse doors via **RTSP**, detects arriving trolleys with a **YOLOv8** truck/vehicle detector, and decodes their QR codes through a **six-pass adaptive pipeline** (CLAHE → Otsu → unsharp mask → multi-scale → `cv2.QRCodeDetector` fallback) — then updates trolley `status` and `location` in SQL Server and streams events live to a React dashboard.

- 🧠 **Built a 4-state inbound-door state machine** with QR-triggered short-circuiting, 3 s / 10 s cooldowns, and a "burst proxy" mode that runs at ~3 FPS bursts to keep CPU low on GPU-less hosts.
- 🔁 **Active-learning loop in production**: captured frames stream into a YOLO dataset, retraining runs **out-of-process** so the eventlet event loop never blocks during inference.
- ⚡ **Singleton `SmoothCameraStream`** per camera serves both MJPEG to the UI and raw frames to the detector from a single `cv2.VideoCapture`, with auto-reconnect and offline placeholder frames.
- 🐳 Dockerized with **NVIDIA GPU passthrough**, ODBC Driver 17, and a 2 GB `shm_size` tuned for PyTorch DataLoader workers.

---

### 🤖 PIWEB / FOS — Factory Operation System Hub with Gemini AI
> *Node.js · Express · React 18 · Mantine · recharts · Google Gemini · MSSQL*

The single pane of glass for an entire manufacturing site — a **bento-grid React SPA** that aggregates every internal subsystem (IMS, IMPAS, MMS, SMS, RTSS, TOS, PQAS, ODIS, …) and ships an **AI-powered production analytics dashboard** backed by Google **Gemini**.

- 📊 **Real-time KPI engine**: Express server calls `USP_P4801QA50_DYRZ` against MSSQL `PT_REAL`, aggregates into daily / by-work-center / by-item-group / under-achieved buckets, and feeds Mantine + recharts visualizations.
- 🌐 **Trilingual AI insight** (Vietnamese / English / Korean): builds a markdown context summary and pipes it through Gemini for explanation + interactive follow-up Q&A.
- 🏭 **Designed for the shop floor**: kiosk auto-reload, fullscreen rotation mode, glassmorphism UI, MSSQL connection pool tuned for long-running requests (60 s timeout, pool max 10).

---

### 🚚 ODIS — Multi-Plant Delivery Operation System
> *Laravel 11 · PHP 8.2 · maatwebsite/excel · PHPMailer · MSSQL (4 connections) · SQLite*

Production-grade delivery / Car-Trans monitoring across **two factories**, with the kind of business logic that ERP vendors quietly farm out — *Pre-Code*, *Debt-Code*, and *PreNight* carry-over from day-shift to night-shift, per-plant cutoff times, and weekday-aware auto-mail.

- 🧮 **Custom shift-carry-over engine**: merges `CodeBu` (debt) + `CodeNeo` (pre-delivered) + `PreNight` (day→night surplus) on a composite `AssyCode|Location` key to compute true completion percent.
- 📧 **Self-driving auto-mail pipeline**: an every-minute Artisan command (`report:auto-send`) evaluates per-plant interval / cutoff / weekday whitelist rules, generates an XLSX via PhpSpreadsheet, and ships it through PHPMailer (Gmail App-Password validated, log-mode fallback).
- 🗂️ **Four-database orchestration**: `sqlsrv`, `sqlsrv_soms`, `sqlsrv_tmdn`, plus local SQLite for settings — each routed correctly through Eloquent connection bindings.
- 🔧 Console commands use `ReflectionClass` to reuse private controller helpers — pragmatic code reuse without breaking encapsulation in the HTTP layer.

---

### 📱 IMPASS — Mobile QR + OCR Workflow for Injection Molding
> *Laravel 12 · Blade · Vite 5 · Tailwind 4 · MSSQL stored procedures · TMES auth*

A web **and** mobile platform that lets operators on the injection-molding floor scan a trolley QR, OCR a printed setpoint sheet, and write production conditions back to the ERP — all driven by a single multi-function stored procedure (`sp_CONDITION_WEBSITE_DYRZ`) dispatched on a `@Fun` parameter.

- 🔐 **Cross-database authentication** against a separate **TMES** SQL Server using `PWDCOMPARE`, fronted by a rate-limited `MobileAuthController` with a graceful demo-mode fallback when the TMES driver is unreachable.
- 📐 **Excel-driven dynamic layouts**: per-plant `.xlsx` templates are parsed with PhpSpreadsheet, merged cells are translated into HTML `colSpan` / `rowSpan`, so the input grid changes *without* a deploy.
- 🏭 **Multi-plant context middleware** (`PlantSelectionMiddleware`) resolves the active plant from request → cookie → session and shares it with every Blade view via the service container.

---

<details>
<summary><b>📦 Other notable builds — TMES, TOPS, ERP Inventory, SIMS, IT Manager</b></summary>

<br />

- **TMES Dashboard** — Django 5.2 + Tailwind real-time production-line monitor for "Door Line A"; merges two SQL Server stored procedures and an inline shift-aware aggregation into a 12-column KPI board, deployed via PM2.
- **TOPS — Truck Operation System** — PHP web dashboard for two-plant truck IO traffic, JSON/XML payloads through the `sp_H_CAR_IO_INFO_DYRZ_*` SP family, XLSX export with PhpSpreadsheet.
- **ERP Inventory (Project_ERP)** — Django reporting layer over `PT_REAL`; heavy BOM-tree rebuild job using direct **pyodbc with MARS_Connection** + aggressive `cursor.nextset()` draining to avoid TDS stalls.
- **SIMS — Smart Inventory Management** — Flask Application Factory with multiple Blueprints, QR-code workflows, Waitress on port 9001, optional pyOpenSSL HTTPS, Werkzeug-hashed accounts.
- **IT Manager** — Laravel 11 IT asset / license tracker with **tri-lingual (vi / en / ko)** UI, dynamic device-attribute search via EAV joins, and `maatwebsite/excel` reporting.

</details>

---

## 📈 GitHub Stats

<div align="center">


<img src="https://github-readme-activity-graph.vercel.app/graph?username=LeAnhQuanAnLao&theme=tokyo-night&hide_border=true&area=true" width="98%" alt="Contribution graph" />

</div>

---

## 📫 Let's Connect

<div align="center">

If you're working on **industrial automation, real-time data pipelines, or AI-on-the-edge** — or you just want to talk database schema design over coffee — my inbox is open.

<a href="mailto:leanhquan.work@email.com"><img src="https://img.shields.io/badge/Send_a_Message-D14836?style=for-the-badge&logo=gmail&logoColor=white" /></a>
<a href="https://github.com/LeAnhQuanAnLao"><img src="https://img.shields.io/badge/Follow_on_GitHub-181717?style=for-the-badge&logo=github&logoColor=white" /></a>

<sub><i>"Code is the contract; the database is the source of truth; the production line is the judge."</i></sub>

</div>
