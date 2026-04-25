<p align="center">
  <img src="https://img.shields.io/badge/PromptWars-2026-blueviolet?style=for-the-badge&logo=lightning&logoColor=white" alt="PromptWars 2026"/>
  <img src="https://img.shields.io/badge/Built_With-Google_Antigravity-4285F4?style=for-the-badge&logo=google&logoColor=white" alt="Built with Google Antigravity"/>
  <img src="https://img.shields.io/badge/Powered_By-Gemini_AI-8E75B2?style=for-the-badge&logo=googlegemini&logoColor=white" alt="Powered by Gemini AI"/>
  <img src="https://img.shields.io/badge/Tests-10%2F10_Passed-00e5a0?style=for-the-badge&logo=checkmarx&logoColor=white" alt="Tests 10/10"/>
</p>

<h1 align="center">🗳️ VoteWise</h1>

<p align="center">
  <strong>Your AI-Powered Indian Election Process Assistant</strong><br/>
  <em>An interactive, accessible, and secure single-file web application that demystifies the Indian election process — built for the PromptWars 2026 Virtual Hackathon.</em>
</p>

<p align="center">
  <a href="#-features">Features</a> •
  <a href="#-screenshots">Screenshots</a> •
  <a href="#-tech-stack">Tech Stack</a> •
  <a href="#-google-services-integration">Google Services</a> •
  <a href="#-getting-started">Getting Started</a> •
  <a href="#-test-suite">Test Suite</a> •
  <a href="#-author">Author</a>
</p>

---

## 🎯 Problem Statement

Millions of eligible Indian voters skip elections simply because the process feels overwhelming — confusing EPIC card procedures, unclear EVM/VVPAT processes, and scattered information. **VoteWise** tackles this head-on by consolidating everything a voter needs into a single, intuitive, AI-powered interface focused on the **Indian electoral system**.

---

## ✨ Features

### 🏠 Dashboard Home
An at-a-glance overview of the Lok Sabha 2029 election cycle: key stats, current election phase, a voter turnout chart (Google Charts — India 2024 data), and an AI-generated election summary powered by Gemini.

### 📅 Interactive Election Timeline
A Google Charts-powered **Timeline visualization** mapping all 6 Indian election phases — from Model Code of Conduct through Counting & Results Declaration — with expandable detail cards showing real-time countdown badges (Completed / Active / Upcoming).

### 📋 Step-by-Step Voter Guide
A 6-step interactive stepper that walks users through the complete Indian voting journey:
1. **Check Voter Eligibility** — Age, citizenship, and constituency requirements
2. **Get Your EPIC Card (Voter ID)** — Apply free at nvsp.in or via BLO
3. **Find Your Polling Booth** — Via electoralsearch.eci.gov.in or Helpline 1950
4. **Carry Valid ID to Polling Booth** — EPIC or 12 ECI-approved alternatives
5. **Cast Your Vote Using EVM** — Blue button, green light + beep confirms
6. **Verify via VVPAT Slip** — 7-second paper confirmation

Users can mark steps as complete with persistent progress tracking. Includes an embedded **Google Maps** iframe showing the **Election Commission of India** headquarters in New Delhi with directions link.

### ⚖️ Know Your Rights
An accordion-based reference of **6 constitutionally protected Indian voter rights**, including Article 326, NOTA (Supreme Court 2013), Section 135B paid holiday, and PwD accessibility rights. Includes a dedicated **AI-powered Q&A input** — ask any rights-related question and get an instant, non-partisan answer from Gemini.

### 🤖 AI Election Assistant
A full conversational chatbot powered by **Google Gemini 2.0 Flash**:
- Context-aware system prompt with complete Indian election data (ECI, EVM, VVPAT, NOTA, EPIC)
- Quick-action suggestion chips for common questions
- Real-time typing indicator and streamed responses
- India-specific offline fallback responses (register, EPIC, EVM, NOTA, booth, results, rights)
- Input sanitization (XSS prevention) and 500-character validation
- Secure API key management via session-based Settings modal

### ❓ FAQ Section
A searchable library of **17 India-specific frequently asked questions** organized by category (Registration, Voting, Rights, Results), with a **Google Charts donut pie chart** showing question distribution. Real-time search filtering across all FAQ entries.

### ♿ Accessibility (WCAG 2.1)
- Skip-to-content navigation link
- Full ARIA roles, labels, live regions, and `aria-expanded` states
- Keyboard-navigable tab bar (Arrow keys + Enter/Space)
- Escape key to close modals
- Semantic HTML5 structure
- Visible focus indicators on all interactive elements

### 🔒 Security
- **Zero hardcoded API keys** — keys stored in `sessionStorage` only
- Password-masked API key input field
- HTML/XSS sanitization on all user inputs
- Content Security Policy (CSP) meta tag

### ⚡ Performance
- **Lazy chart loading** — Google Charts drawn only when their tab becomes visible, not all at once at startup
- Single-file architecture with no build tools or framework overhead

---

## 📸 Screenshots

> 🔄 **Screenshots coming soon** — take fresh screenshots of the India-content app by opening `index.html` in your browser and saving images to the `screenshots/` folder.

---

## 🛠️ Tech Stack

| Layer | Technology |
|---|---|
| **Frontend** | HTML5, CSS3, Vanilla JavaScript (single-file architecture) |
| **AI Engine** | Google Gemini 2.0 Flash (`generativelanguage.googleapis.com`) |
| **Charts** | Google Charts API (Timeline + Column + Pie/Donut charts) |
| **Maps** | Google Maps Embed API — Election Commission of India, New Delhi |
| **Typography** | Google Fonts — Inter (body) + Outfit (headings) |
| **Design** | Dark theme, glassmorphism, CSS custom properties, gradient accents |
| **Testing** | Built-in 10-point automated test suite |

---

## 🔗 Google Services Integration

VoteWise deeply integrates **4 Google Services**, all within a single HTML file:

| # | Service | Usage |
|---|---|---|
| 1 | **Google Gemini 2.0 Flash** | AI chatbot for election Q&A + AI-powered rights advisor + home page election summary |
| 2 | **Google Charts** | Timeline visualization (Lok Sabha phases), Column chart (voter turnout by age — India 2024), Donut pie chart (FAQ categories) |
| 3 | **Google Maps Embed** | Interactive map showing Election Commission of India headquarters in New Delhi |
| 4 | **Google Fonts** | Inter (400–700) for body text, Outfit (500–800) for headings |

---

## 🇮🇳 India Election Content

VoteWise is fully localized for the **Indian electoral system**:

| Feature | India-Specific Content |
|---|---|
| **Election Body** | Election Commission of India (ECI) — eci.gov.in |
| **Voter ID** | EPIC Card — apply free at nvsp.in |
| **Booth Search** | electoralsearch.eci.gov.in |
| **Voter Helpline** | 1950 |
| **Voting Technology** | EVM (Electronic Voting Machine) + VVPAT |
| **Special Feature** | NOTA (None of the Above) — Supreme Court 2013 |
| **Election Timeline** | 6 Lok Sabha 2029 phases |
| **Voter Rights** | Article 326, Section 135B RPA, PwD accessibility |
| **Maps** | Election Commission of India HQ, New Delhi |
| **Turnout Chart** | India 2024 Lok Sabha data (18–25: 58%, 60+: 69%) |
| **Violations** | Report via cVIGIL app or Voter Helpline 1950 |

---

## 🚀 Getting Started

### Prerequisites
- A modern web browser (Chrome, Edge, Firefox, Safari)
- A [Google Gemini API key](https://aistudio.google.com/app/apikey) (free tier works)

### Run Locally

```bash
# Clone the repository
git clone https://github.com/mogilishivaram/votewise.git
cd VoteWise

# Option 1: Open directly
# Simply open index.html in your browser

# Option 2: Local server (recommended)
npx -y http-server -p 3000 -c-1
# Visit → http://localhost:3000
```

### Configure API Key
1. Click the **⚙️ Settings** button in the top-right corner
2. Paste your Gemini API key
3. Click **Save** — the key is stored in `sessionStorage` (never persisted to disk)
4. Start chatting with the AI assistant!

---

## 🧪 Test Suite

VoteWise ships with a **built-in 10-point automated test suite** that runs on every page load. Tests validate the entire application stack:

| # | Test | What It Validates |
|---|---|---|
| 1 | **Tab Navigation** | 6 tabs + 6 panels + active state management |
| 2 | **Election Timeline** | 6 phase cards + Google Charts Timeline integration |
| 3 | **Step-by-Step Guide** | 6 steps + expand/collapse interactivity |
| 4 | **Voter Rights** | 6+ accordion items + accessible headers |
| 5 | **AI Assistant** | Chat input + send button + Gemini endpoint configured |
| 6 | **FAQ Section** | 10+ FAQs + real-time search filtering |
| 7 | **Google Services** | Charts API ✓ · Maps iframe ✓ · Gemini model ✓ |
| 8 | **Security** | No hardcoded keys · password field · XSS sanitization |
| 9 | **Accessibility** | Skip link · ARIA roles · labels · live regions · expanded states |
| 10 | **Input Validation** | Max-length enforcement · empty rejection · HTML stripping |

> **Result: ✅ 10/10 tests passed**

Click **🔄 Run Tests Again** in the floating test panel to re-run at any time.

---

## 📁 Project Structure

```
VoteWise/
├── index.html          # Complete single-file application (HTML + CSS + JS)
├── README.md           # This file
├── screenshots/        # App screenshots for documentation
│   ├── home.png
│   ├── timeline.png
│   ├── guide.png
│   ├── rights.png
│   ├── ai-help.png
│   └── faq.png
└── .gitignore
```

> **Single-file architecture**: The entire application — 3,150+ lines of HTML, CSS, and JavaScript — lives in one self-contained `index.html`. No build tools, no dependencies, no framework overhead. Just open and run.

---

## 🏆 Hackathon Compliance

| Requirement | Status |
|---|---|
| Single-file HTML application | ✅ |
| Google Gemini AI integration | ✅ |
| Google Charts (2+ chart types) | ✅ Timeline + Column + Donut Pie |
| Google Maps integration | ✅ Election Commission of India, New Delhi |
| 10-point automated test suite | ✅ 10/10 |
| Responsive design | ✅ |
| Accessibility (WCAG 2.1) | ✅ |
| Security best practices | ✅ |
| Non-partisan content | ✅ |
| Built with Google Antigravity | ✅ |

---

## 🌟 Key Design Decisions

- **India-first content** — All election data, rights, FAQs, and fallbacks reflect the Indian electoral system (ECI, EVM, VVPAT, NOTA, EPIC)
- **Lazy chart rendering** — Charts draw only when their tab is visited, improving initial load performance
- **Dark-first UI** — Reduces eye strain for extended research sessions; uses a curated color palette with accent glows
- **Progressive disclosure** — Timeline cards and guide steps expand on click, keeping the initial view clean
- **Session-only API storage** — API keys never touch `localStorage` or cookies; they vanish when the tab closes
- **Zero-dependency architecture** — No npm, no bundler, no framework. Maximum portability, minimum attack surface
- **Accessible by default** — Every interactive element is keyboard-reachable with proper ARIA semantics

---

## 👤 Author

**Shiva Ram Mogili**

Built with ❤️ using [Google Antigravity](https://blog.google/technology/google-deepmind/) + [Gemini AI](https://ai.google.dev/) for the **PromptWars 2026** Virtual Hackathon.

---

<p align="center">
  <img src="https://img.shields.io/badge/License-MIT-green?style=flat-square" alt="MIT License"/>
  <img src="https://img.shields.io/badge/PRs-Welcome-brightgreen?style=flat-square" alt="PRs Welcome"/>
  <img src="https://img.shields.io/badge/Made_with-❤️-red?style=flat-square" alt="Made with love"/>
</p>

<p align="center"><em>Every vote counts. Every voter matters. 🗳️</em></p>
