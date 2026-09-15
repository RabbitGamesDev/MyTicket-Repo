# MyTicket

<div align="center">

[![GitHub license](https://img.shields.io/badge/license-MIT-blue.svg)](LICENSE)
[![GitHub stars](https://img.shields.io/github/stars/rabbitgamesdev/MyTicket?style=social)](https://github.com/rabbitgamesdev/MyTicket)
[![Status](https://img.shields.io/badge/status-active-success.svg)]()
[![Platform](https://img.shields.io/badge/platform-Web%20%7C%20PWA-informational)]()

*A lightweight, intelligent personal finance Web App and PWA designed to simplify receipt tracking, detect invisible financial leaks ("Fugas Invisibles"), and rescue family budgets—built entirely from real family needs.*

</div>

---

## 📖 The Story Behind MyTicket

MyTicket is the very first tool in an ongoing series of bespoke applications developed by **Ian (Rab / RB)** for himself and his family. The core mission of this series is clear: **to meaningfully improve the quality of life, save precious time, and maximize daily utility for home and family through custom-built software.**

### Why I Built It
It all started when I noticed a recurring pain point in my family's financial management: budgeting felt abstract, stressful, and disconnected from reality, while everyday expenses and invisible micro-purchases ("fugas hormiga") were silently draining resources. 

Instead of stepping in with abstract lectures or endless arguments about money, **I decided to intervene using code.** 

I sat down with my family, asked them about their deepest financial struggles, frustrations, and daily hurdles with money management, and distilled all those raw pain points into a single guiding sentence:

> *"We need to know where our money actually goes without tedious manual spreadsheets, understand what we can truly spend based on our real income after fixed bills, and spot hidden leaks before they derail our goals."*

Working relentlessly from that exact phrase, I designed and engineered **MyTicket**—a zero-friction, AI-powered receipt scanning web application built to put financial clarity back into everyone's hands.

---

## 🔍 What is MyTicket?

**MyTicket** is a mobile-first Progressive Web App (PWA) built with Vanilla JavaScript (ES6+), modern CSS, and local persistence. It works alongside an AI-powered backend (compatible with Cloudflare Workers and Groq API) to scan, extract, categorize, and analyze paper receipts or digital tickets instantly.

Unlike traditional corporate finance apps that require tedious account linking or heavy bank credentials, MyTicket focuses on **privacy, simplicity, and family context**:
- **Zero Bank Credential Risks:** No sensitive bank logins required. You capture receipts via camera or gallery upload.
- **Real Available Money ("Disponible Real"):** Automatically subtracts fixed monthly expenses (rent, utilities, services) from your total income, revealing your true spending power.
- **Invisible Leaks Radar ("Fugas Invisibles"):** Automatically classifies items into essential and non-essential expenses, highlighting money leaks.
- **Rescue Route ("Ruta de Rescate"):** Connects daily spending habits and micro-leaks directly to debt reduction milestones, showing how redirecting small savings can finish debt months ahead of schedule.
- **Personalized AI Coach:** Speaks directly to you using your custom nickname and contextual math instead of generic warnings.

---

## 📱 How It Works (App Architecture & Features)

1. **Personalized Onboarding (5 Steps):** Set up your custom nickname, income type (fixed salary, informal/freelance, business, or pension), monthly earnings, fixed monthly commitments, and active debt targets.
2. **Snap & Extract Workflow:** Take a photo of any receipt or upload an image. The app compresses the image locally, sends it securely to the AI backend for item-by-item extraction, and instantly displays essential vs. non-essential breakdowns.
3. **Interactive Dashboard:** Live visual progress bars of your spent vs. remaining real budget, quick stats, monthly trend charts, and smart contextual coaching alerts.
4. **History & CSV Export:** Filter past tickets by month, review itemized breakdowns, and export your data anytime as a clean CSV file.
5. **Configurable Backend:** Keep your API keys secure on a lightweight serverless backend (like a Cloudflare Worker) while running the frontend seamlessly on GitHub Pages or locally.

---

## 🛠️ Tech Stack

- **Frontend:** Vanilla HTML5, CSS3 (Modern Flexbox, CSS Variables, Animations), Mobile-First Responsive PWA Design.
- **Data & Persistence:** `localStorage` for fast, offline-capable local storage.
- **AI & OCR Integration:** Fetch API interacting with serverless backend endpoints (Cloudflare Workers + Groq LLM API for structured JSON extraction).
- **Hosting:** Optimized for instant deployment on **GitHub Pages**.

---

## 🚀 Getting Started & Deployment

### 1. Frontend Setup (GitHub Pages)
1. Clone or download this repository.
2. Upload the `index.html` file directly to your GitHub repository root.
3. Enable **GitHub Pages** in your repository settings (Branch: `main` or `master`, folder: `/root`).
4. Open your live GitHub Pages URL on your mobile phone or browser.

### 2. Configuring the Backend
To enable AI receipt scanning:
1. Set up your lightweight serverless backend (e.g., Cloudflare Worker) equipped with your Groq API key to handle the `/scan-ticket` endpoint.
2. Open MyTicket in your browser, tap the **Settings (⚙️)** gear icon in the top right, and paste your backend worker URL into the **Backend API URL** field.
3. Save changes, and you're ready to start scanning!

---

## 📜 License

Distributed under the MIT License. See `LICENSE` for more information.

<div align="center">
  <p>Built with ❤️ and code by <b>Ian (Rab / RB)</b> • RGS Labs™</p>
</div>
