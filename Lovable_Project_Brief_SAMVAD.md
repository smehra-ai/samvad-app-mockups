# Lovable Project Brief: SAMVAD App
**The Art of Mindful Conversations**
*PURE BEING by Shalini Mehra*

## 1. Project Overview
**Project Name:** SAMVAD
**Domain:** samvad.purebeing.eu
**App Type:** Progressive Web App (PWA) built with React/Tailwind, mobile-first design.
**Core Purpose:** An AI-powered application that guides sensitive leaders and entrepreneurs through difficult employee conversations. The app diagnoses the situation using a responsibility model and generates a personalized, concrete conversation script.
**Target Audience:** Sensitive Leaders & Entrepreneurs, Executive Level, and aspiring leaders internationally.
**Languages:** Bilingual (German and English), toggleable in the UI.

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

## 3. Information Architecture & Navigation
The app uses a minimal bottom navigation bar with four items:
1. **Home:** Entry point, Generator CTA, 4 Knowledge Modules.
2. **Bibliothek (Library):** Saved conversation guides and "Insights for Leaders" articles.
3. **Favoriten (Favorites):** Bookmarked guides and articles.
4. **Profil (Profile):** Account settings, subscription status, language toggle (DE/EN).

## 4. Core Features & User Flows

### 4.1 The Conversation Guide Generator (3 Steps)
This is the core AI feature of the app.

**Step 1: Choose Conversation Type**
- User can directly select from 9 types (Motivate, Set Goals, Praise, Criticize, Support, Conflicts, Responsibility Dialogue, Confess Mistakes, Control).
- *OR* user can use the **Diagnose Tool**.

**Step 1b: Diagnose (The Responsibility Model)**
- User answers 4 questions (Yes / No / Unsure):
  - **Wollen (Will):** Is the motivation there?
  - **Können (Can):** Does the person have the skill?
  - **Dürfen (Allowed):** Do they have the resources/permission?
  - **Müssen (Must):** Are they actually responsible?
- The app evaluates the answers and routes to the correct conversation type (e.g., "Not responsible" -> "Responsibility Dialogue").

**Step 2: Provide Context**
- User answers 3 open text questions:
  1. What is the topic?
  2. Why is this conversation happening?
  3. What is the desired goal?

**Step 3: Generated Guide (Result)**
- The AI generates a structured script containing:
  - **Preparation:** Mood, mindset, facts.
  - **Opening:** Concrete opening sentence.
  - **Phrasing Examples:** 3-5 specific sentences.
  - **What to watch for:** Warnings regarding the Drama Triangle, Evaluation Biases, and Perception.
  - **Close & Commitment:** Next steps and follow-up.
- **Actions:** Save to Library, Share, Export as PDF.

### 4.2 Knowledge Modules (Home Screen)
Four interactive educational modules:
1. **Welche Verantwortung fehlt?** (The 4-dimension responsibility model and self-check).
2. **Welches Spiel läuft hier?** (The Drama Triangle: Victim, Rescuer, Persecutor, and exit strategies).
3. **Vor dem Beurteilen** (Pre-flight checklist of 8 evaluation biases).
4. **Kommunikations-Basics** (Transactional analysis ego states, rules of perception, questioning techniques).

### 4.3 Insights for Leaders
- Curated articles located in the Library (not called a "Blog").
- Examples: Recognizing the Drama Triangle, Leading without Fear.
- *Future Addition:* UMIT leadership training transcripts will be integrated here.

## 5. Technical Requirements for Lovable

### 5.1 Frontend Stack
- React with Vite
- Tailwind CSS for styling (using the specific color hex codes above)
- Framer Motion for subtle, calm animations
- PWA setup (manifest.json, service workers) for installability

### 5.2 Backend & Integrations
- **Database:** Supabase or equivalent for user accounts and saving generated guides to the Library.
- **AI Integration:** OpenAI API (GPT-4o) connection to power the Generator. The prompt must be fed the user's context (Step 2) and the specific rules for the selected conversation type.
- **PDF Generation:** Server-side PDF rendering (e.g., via a Supabase Edge Function using Puppeteer or an external API like PDFShift) to allow users to download their guides.
- **Payment Gateway:** Paddle integration for the subscription model.

### 5.3 Subscription Model (Paddle)
- **Free:** 2 generated guides per month.
- **Essential:** €12.99/month or €99/year — Save 36% (10 guides/month, full module access, Insights access, PDF export).
- **Professional:** €24.99/month or €199/year (Unlimited guides, full access, priority support).

## 6. Assets Provided in GitHub
The following assets will be uploaded to the GitHub repository to guide the Lovable build:
- **Mockups (9 UI Screens):** Showing the exact layout, spacing, and typography.
- **Image Assets (5 Library Thumbnails):** High-quality, diverse leadership imagery.
- **This Documentation:** As the definitive build guide.
