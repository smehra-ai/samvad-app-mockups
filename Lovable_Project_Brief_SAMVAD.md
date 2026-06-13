# Lovable Project Brief: SAMVAD App
**The Art of Mindful Conversations**
*PURE BEING by Shalini Mehra*

---

## 1. Project Overview

**Project Name:** SAMVAD
**Domain:** samvad.purebeing.eu
**App Type:** Progressive Web App (PWA) built with React/Tailwind, mobile-first design.
**Core Purpose:** A SaaS productivity tool for managers and executives. SAMVAD provides structured conversation preparation frameworks based on established leadership and business communication models. Users input their workplace situation, and the app generates a structured preparation guide with phrasing examples. No therapy, counseling, or medical advice is provided. All content is based on business communication and leadership development frameworks used in executive education.
**Target Audience:** Sensitive Leaders & Entrepreneurs, Executive Level, and aspiring leaders internationally.
**Languages:** Bilingual (German and English), toggleable in the UI.

> **Paddle Compliance Note:** SAMVAD is a SaaS software product. It is a structured preparation and reflection tool for workplace conversations. It does not provide psychological therapy, medical advice, personal coaching, or human advisory services of any kind.

---

## 2. Design System & Brand Identity

The app follows the "ZENDO interior style" — a member of the PURE BEING brand family. It combines modern executive professionalism with Zen/Tao philosophy.

### 2.1 Color Palette
- **Background (Interior):** Warm Cream `#F5F0E8` (Ensures perfect readability for text-heavy screens)
- **Primary Text:** Dark Charcoal `#2D3748`
- **Accent & Borders:** Warm Gold `#D4B26A`
- **Active Elements:** Deep Midnight Navy `#0F1B3D`
- **Cards:** Pure White `#FFFFFF` with soft, subtle drop shadows

### 2.2 Typography
- **Headlines & Logos:** Cormorant Garamond (Elegant, light, serif)
- **Body Text & UI Elements:** Crimson Pro (Highly readable serif)

### 2.3 Visual Assets & Imagery
- **Hero Image (Home):** Atmospheric Zen garden at golden hour featuring an Asian female master in conversation with a Western professional.
- **Library Thumbnails:** Diverse, international leadership settings (e.g., Zen boardroom with a dragon painting, modern executive office with a city skyline, outdoor Zen garden). The imagery must reflect a global executive audience, not exclusively Asian.
- **Icons:** Minimalist gold line-art (e.g., scale, triangle, eye, speech bubble, heart, gear, key, shield).

---

## 3. Information Architecture & Navigation

The app uses a minimal bottom navigation bar with four items:
1. **Home:** Entry point, Generator CTA, 4 Knowledge Modules.
2. **Bibliothek (Library):** Saved conversation guides and "Insights for Leaders" articles.
3. **Favoriten (Favorites):** Bookmarked guides and articles.
4. **Profil (Profile):** Account settings, subscription status, language toggle (DE/EN).

---

## 4. Core Features & User Flows

### 4.1 The Conversation Guide Generator (3 Steps)

This is the core AI feature of the app. It generates structured preparation frameworks for workplace conversations.

**Step 1: Choose Conversation Framework**
- User can directly select from 11 types (Motivate, Set Goals, Praise, Criticize, Address Difficult Topics, Control/Review, Objectify Conflicts, Support/Develop, Confess Mistakes, Responsibility Dialogue, Present).
- *OR* user can use the **Leadership Self-Reflection Tool** (see Step 1b).

**Step 1b: Leadership Self-Reflection Tool (Two-Stage)**

This tool helps the leader reflect on their own leadership responsibility *before* preparing a conversation. It is a structured self-check for the leader — not an analysis of another person.

*Stage 1 — Leader Self-Check (Has the leader fulfilled their responsibility?):*

The leader answers three questions about their own actions:

| Question (DE) | Question (EN) | What it checks |
|---|---|---|
| Habe ich klar kommuniziert, was erwartet wird? | Have I clearly communicated what is expected? | Sollen / Must — clarity of mandate |
| Habe ich die nötige Befugnis erteilt? | Have I granted the necessary authority? | Dürfen / Allowed — authorization |
| Habe ich Ressourcen und Mittel bereitgestellt? | Have I provided the necessary resources and means? | Können / Can — enablement |

Only when all three are answered Yes does the leader proceed to Stage 2.

*Stage 2 — Conversation Context:*

| Question (DE) | Question (EN) | What it checks |
|---|---|---|
| Zeigt die Person Bereitschaft und Engagement? | Is the person showing willingness and engagement? | Wollen / Will — motivation context |

The app then routes to the correct conversation framework based on the combined answers (e.g., if Stage 1 reveals a missing mandate → Responsibility Dialogue; if Stage 2 reveals low motivation → Motivation Conversation).

**Step 2: Provide Context**
- User answers 3 open text questions:
  1. What is the topic?
  2. Why is this conversation happening?
  3. What is the desired outcome?

**Step 3: Generated Guide (Result)**
- The AI generates a structured preparation framework containing:
  - **Preparation:** Recommended mindset, key facts to have ready.
  - **Opening:** Concrete opening sentence suggestion.
  - **Phrasing Examples:** 3–5 specific sentence suggestions.
  - **What to watch for:** Awareness reminders about communication patterns, perception biases, and evaluation errors.
  - **Close & Commitment:** Suggested next steps and follow-up actions.
- **Actions:** Save to Library, Share, Export as PDF.

---

### 4.2 Knowledge Modules (Home Screen)

Four interactive educational modules based on established business communication and leadership development frameworks:

**1. Welche Verantwortung fehlt? / Which responsibility is missing?**
A structured self-reflection framework for leaders to identify which dimension of leadership responsibility may be unclear or missing before a conversation. Based on the four-dimension responsibility model used in executive education (Schmid/Messmer). Includes a standalone self-check usable independently of the generator.

**2. Kommunikationsmuster erkennen / Recognize Communication Patterns**
*(Previously: "Welches Spiel läuft hier?" — renamed for Paddle compliance)*
A module on recurring workplace interaction patterns that can block productive dialogue. Based on the Karpman Drama Triangle, a widely used business communication model taught in leadership programs worldwide. Content:
- Three workplace interaction roles: Critic (Verfolger), Enabler (Retter), Victim (Opfer)
- Common patterns: Yes-But, Blame Game, Courtroom
- Practical exit strategies: Activate adult communication mode, address the factual level, return ownership
- Self-reflection questions: *"Which communication pattern am I falling into? Which pattern is my counterpart showing?"*

> **Note for Lovable:** Do NOT use the word "psychologisch" (psychological) anywhere in the UI. Use "Kommunikationsmuster" (communication patterns), "Gesprächsdynamik" (conversation dynamics), or "Führungsverhalten" (leadership behavior) instead.

**3. Vor dem Beurteilen / Before You Evaluate**
A pre-flight checklist of 8 common evaluation errors in leadership conversations. Based on established HR and management science. Positioned as an awareness tool to improve fairness and objectivity in performance conversations.

Errors covered:
1. Voreilige Schlussfolgerungen / Jumping to conclusions
2. Vorurteile / Prejudice
3. Überstrahlungseffekt (Halo) / Halo effect
4. Kontakteffekt / Recency bias
5. Tendenz zur blassen Mitte / Central tendency error
6. Beurteilung aus zweiter Hand / Second-hand assessment
7. Beurteiler als Maßstab / Self-reference criterion
8. Tendenz zur Nachsicht/Strenge / Leniency or strictness bias

**4. Kommunikations-Basics / Communication Basics**
A micro-learning module on business communication techniques for leaders. Content:
- **Kommunikationsstile im Gespräch / Communication Styles** (Parent / Adult / Child communication modes — based on Transactional Analysis, a standard business communication model used in executive education. Do NOT label this as "psychotherapy" or "psychological analysis" in the UI. Label as: "Kommunikationsstile" / "Communication Styles".)
- **Wahrnehmungsregeln / Rules of Perception** (5 rules for separating observation from interpretation)
- **Quittungen / Acknowledgements** (Example phrases for active listening and acknowledgement)
- **Fragetechnik / Questioning Techniques** (Open questions for information, closed questions for action)
- *[UMIT Leadership Training Content — to be added once transcripts are available]*

---

### 4.3 Insights for Leaders
- Curated leadership articles located in the Library section (NOT called a "Blog").
- Examples: *Recognizing Communication Patterns That Block Dialogue*, *Leading Without Fear*, *The Art of the Difficult Conversation*.
- Future addition: UMIT leadership training content will be integrated here.

---

## 5. Technical Requirements for Lovable

### 5.1 Frontend Stack
- React with Vite
- Tailwind CSS for styling (using the specific color hex codes above)
- Framer Motion for subtle, calm animations
- PWA setup (manifest.json, installable only — no offline service worker for v1)

### 5.2 Backend & Integrations
- **Database:** Supabase for user accounts, saved guides, and language preferences.
- **AI Integration:** OpenAI API (GPT-4o) with bring-your-own API key. The prompt must be fed the user's context (Step 2), the selected conversation framework type, and the specific rules for that type.
- **PDF Generation:** Server-side PDF rendering via a Supabase Edge Function (Puppeteer or PDFShift) for guide download/email.
- **Payment Gateway:** Paddle integration. SAMVAD is a SaaS software product — subscription to a digital productivity tool.

### 5.3 Subscription Model (Paddle)

| Plan | Price | Includes |
|---|---|---|
| Free | €0 | 2 generated guides per month, read-only module access |
| Essential | €12.99/month or €99/year (Save 36%) | 10 guides/month, full module access, Insights access, PDF export |
| Professional | €24.99/month or €199/year | Unlimited guides, full access, priority support |

---

## 6. Paddle-Compliant Formulations — Reference List

The following table shows which formulations to use and which to avoid throughout the entire app UI, marketing copy, and Paddle onboarding description:

| Avoid (Risk) | Use Instead (Safe) |
|---|---|
| "Psychological analysis" | "Communication pattern awareness" |
| "Diagnose your employee" | "Reflect on your leadership responsibility" |
| "Psychologische Beratung" | "Strukturierte Gesprächsvorbereitung" |
| "Transaktionsanalyse" (in UI) | "Kommunikationsstile" / "Communication Styles" |
| "Drama-Dreieck" (in UI labels) | "Kommunikationsmuster" / "Interaction Patterns" |
| "Therapie" / "Therapy" | Never use |
| "Coaching" (as a service) | "Structured preparation framework" |
| "Diagnose responsibility gaps" | "Reflect on your leadership responsibility" |
| "Analyze your counterpart" | "Prepare for the conversation" |
| "Pseudo-science" adjacent terms | Never use |

---

## 7. Paddle Onboarding Description (Copy-Paste Ready)

Use this exact description when registering SAMVAD with Paddle:

> *SAMVAD is a SaaS productivity tool for managers and executives. It provides structured conversation preparation frameworks based on established leadership and business communication models used in executive education worldwide. Users describe their workplace situation, select a conversation framework, and receive a structured preparation guide with suggested phrasing, awareness reminders, and follow-up steps. The app also includes four educational modules covering leadership responsibility models, communication pattern awareness, evaluation bias checklists, and business communication techniques. No therapy, psychological counseling, medical advice, or human advisory services are provided. All content is based on business communication and leadership development frameworks.*

---

## 8. Assets Provided in GitHub

The following assets are uploaded to the GitHub repository to guide the Lovable build:
- **Mockups (9 UI Screens):** Showing the exact layout, spacing, and typography.
- **Image Assets (5 Library Thumbnails):** High-quality, diverse international leadership imagery.
- **Landing Page Mockup:** samvad_landing_signup_v2.png
- **Lockscreen Wallpaper:** samvad_lockscreen_wallpaper.png
- **This Documentation:** As the definitive build guide.

---

*Document prepared as the foundation for the Lovable build of SAMVAD. Content based on leadership training materials by Shalini Mehra. Last updated: June 2026.*
