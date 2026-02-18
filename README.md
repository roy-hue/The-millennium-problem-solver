<div align="center">

<img src="https://img.shields.io/badge/Millennium-Prize%20Solver-6366f1?style=for-the-badge&logo=react&logoColor=white" />
<img src="https://img.shields.io/badge/Prize%20Pool-$7%2C000%2C000-f59e0b?style=for-the-badge&logo=bitcoin&logoColor=white" />
<img src="https://img.shields.io/badge/Problems-6%20Unsolved-ef4444?style=for-the-badge" />
<img src="https://img.shields.io/badge/AI%20Powered-GPT--4-10b981?style=for-the-badge&logo=openai&logoColor=white" />

# 🏆 Millennium Prize Problems Solver Platform

### *The world's most advanced AI-powered research environment for tackling mathematics' greatest unsolved challenges*

[![React](https://img.shields.io/badge/React-18.2-61DAFB?logo=react)](https://react.dev)
[![Tailwind](https://img.shields.io/badge/Tailwind-CSS-06B6D4?logo=tailwindcss)](https://tailwindcss.com)
[![Stripe](https://img.shields.io/badge/Stripe-Payments-635BFF?logo=stripe)](https://stripe.com)
[![Base44](https://img.shields.io/badge/Base44-Platform-8B5CF6)](https://base44.com)
[![Framer](https://img.shields.io/badge/Framer-Motion-FF0055?logo=framer)](https://framer.com)

</div>

---

## 📌 Table of Contents

- [Overview](#overview)
- [Core Features](#core-features)
- [AI & Prompt Engineering](#ai--prompt-engineering)
- [Subscription Tiers](#subscription-tiers)
- [Tech Stack](#tech-stack)
- [Data Models](#data-models)
- [Business Intelligence](#business-intelligence)
- [UI/UX Design System](#uiux-design-system)

---

## 🌐 Overview

A full-stack, AI-driven research platform built for mathematicians, PhD students, and prize-seekers working on the **7 Millennium Prize Problems** — the most celebrated unsolved problems in mathematics, each carrying a **$1,000,000 USD** prize from the Clay Mathematics Institute.

> The platform combines structured proof-building tools, personalized AI tutoring, prerequisite tracking, and subscription-gated premium intelligence features into a single cohesive research environment.

---

## 🎯 Core Features

---

### 🔭 Problem Exploration

- **Interactive Problem Browser** — Browse all 6 active unsolved Millennium Prize Problems with full metadata

- **Custom Mathematical Visualizations** — Unique canvas-rendered, interactive visualizations per problem:
  - 📊 P vs NP — Complexity landscape diagrams
  - 🌊 Navier-Stokes — Fluid dynamics flow fields
  - 📈 Riemann Hypothesis — Critical strip visualization
  - 🔷 Birch-Swinnerton-Dyer — Elliptic curve + L-function plots
  - ⚡ Yang-Mills — Lattice gauge field dynamics & energy spectrum
  - 🔺 Hodge Conjecture — Algebraic cycle representations

- **Formal Statement Viewer** — Access rigorous mathematical definitions in structured format

- **Difficulty Ranking System** — Problems ranked 1–6 by approachability for structured learning

- **Prize Claim Guide Generator** — Downloadable Markdown guides with official Clay Mathematics Institute submission instructions

---

### 🧪 AI-Powered Proof Workspace

- **Step-by-Step Proof Builder** — Structured, ordered logical step editor with justification fields per step

- **Real-Time AI Step Validation** — LLM analyzes each step for:
  - Logical consistency with prior steps
  - Correct use of theorems and definitions
  - Gaps in reasoning
  - Boundary condition checks

- **Quantitative Formalization** — Converts informal/qualitative statements into rigorous mathematical notation with explicit quantifiers (∀, ∃)

- **Socratic Hint System** — AI provides guided hints without revealing answers — asks targeted questions to redirect thinking

- **Cross-Step Contradiction Detection** *(Pro)* — Scans all workspace steps for logical contradictions across the full proof history

- **Process Flow Analysis** — Compares user approach against standard textbook methods, identifies deviations, and generates Wikipedia learning links

- **Research Conclusion Export** — Generates comprehensive Markdown reports including:
  - Executive summary
  - Full validation results
  - Process flow deviations
  - Identified knowledge gaps
  - Recommended next steps

---

### 🎓 Personalized Learning System

- **Knowledge Assessment Engine** — AI-generated quizzes tailored to each Millennium Problem's prerequisite map

- **Adaptive Learning Paths** — Personalized study sequences generated from assessment scores

- **Prerequisite Dependency Trees** — Visual interactive graphs showing required knowledge chains

- **Mastery Tracking** — 0–100% mastery scale tracked per mathematical concept across 100+ prerequisites

- **Estimated Study Hours** — Realistic time-to-mastery estimates per concept

- **Curated Resource Lists** — Papers, textbooks, and exercises recommended per prerequisite

- **Multi-Status Tracking** — Track each concept as: `not_started` → `in_progress` → `reviewing` → `mastered`

---

### 📊 Progress Dashboard

- **Personal Stats Overview** — Track total workspaces, mastered prerequisites, hours studied, and active approaches

- **Workspace History** — Save, name, and revisit unlimited proof attempts *(Standard/Pro)*

- **Status Labels** — Mark approaches as `draft`, `promising`, `blocked`, or `abandoned`

- **Onboarding Flow** — Goal-based classification: *Learner* vs. *Prize Solver* with tailored plans

---

## 🤖 AI & Prompt Engineering

---

### Techniques Employed

1. **Role Assignment Priming**
   - Prompts open with: *"You are a rigorous mathematical validator..."* to set domain authority and precision tone

2. **Full Context Injection**
   - Every validation prompt includes: problem name, problem description, all prior steps, and current justification — preventing hallucination by providing ground truth

3. **Structured JSON Schema Output**
   - All LLM responses are forced into predefined JSON schemas:
     ```json
     {
       "validation_status": "valid | invalid | needs_review",
       "explanation": "string",
       "issues": ["string"],
       "suggestions": ["string"]
     }
     ```
   - Eliminates parsing failures and ensures consistent downstream processing

4. **Chain-of-Thought Reasoning**
   - Multi-criteria validation prompts direct the model to reason sequentially through logical consistency → theorem correctness → gaps → boundary conditions

5. **Socratic Constraint Prompting**
   - Hint prompts explicitly instruct: *"Do not give away the answer directly — ask questions that redirect thinking"* — enforcing pedagogical discipline

6. **Comparative Baseline Analysis**
   - Process flow prompts compare user approach against *"standard textbook methods"* and *"known prerequisite requirements"* to surface non-obvious gaps

7. **Severity Classification Prompting**
   - Issues are forced into `minor | moderate | critical` tiers for prioritized remediation

8. **Resource Generation via Web Context**
   - `add_context_from_internet: true` flag enables real-time Wikipedia and academic resource lookup during analysis

9. **Automated Formalization**
   - Quantification prompts convert informal language to symbolic notation with explicit quantifier binding

10. **Contradiction Detection Across Memory**
    - Pro consistency checks maintain full proof state context to detect logical conflicts that span non-adjacent steps

---

## 💳 Subscription Tiers

---

| Feature | 🔹 Free | ⚡ Standard ($29.99/mo) | 👑 Pro ($100/mo) |
|---|---|---|---|
| Browse Problems | ✅ | ✅ | ✅ |
| Visualizations | ✅ | ✅ | ✅ |
| Workspace Entries | 5 max | Unlimited | Unlimited |
| AI Step Validation | ❌ | ✅ | ✅ |
| AI Hints | ❌ | ✅ | ✅ |
| Quantitative Analysis | ❌ | ✅ | ✅ |
| Learning Paths | ❌ | ✅ | ✅ |
| Export Conclusions | ❌ | ✅ | ✅ |
| Contradiction Detection | ❌ | ❌ | ✅ |
| Cross-Step Validation | ❌ | ❌ | ✅ |
| Process Flow Analysis | ❌ | ❌ | ✅ |
| Priority AI Processing | ❌ | ❌ | ✅ |

---

## 🛠️ Tech Stack

---

### Frontend

| Technology | Purpose | Version |
|---|---|---|
| ![React](https://img.shields.io/badge/React-61DAFB?logo=react&logoColor=black) | UI Framework | 18.2 |
| ![TypeScript](https://img.shields.io/badge/TypeScript-3178C6?logo=typescript&logoColor=white) | Type Safety | Latest |
| ![Tailwind](https://img.shields.io/badge/Tailwind-06B6D4?logo=tailwindcss&logoColor=white) | Styling | Latest |
| ![Framer](https://img.shields.io/badge/Framer_Motion-FF0055?logo=framer&logoColor=white) | Animations | 11.x |
| ![Radix UI](https://img.shields.io/badge/Radix_UI-111827?logo=radixui) | Accessible Components | Latest |
| ![TanStack](https://img.shields.io/badge/TanStack_Query-FF4154?logo=reactquery&logoColor=white) | Server State | 5.x |
| ![React Router](https://img.shields.io/badge/React_Router-CA4245?logo=reactrouter&logoColor=white) | Client Routing | 6.x |
| ![Three.js](https://img.shields.io/badge/Three.js-000000?logo=threedotjs) | 3D Graphics | Latest |
| ![Recharts](https://img.shields.io/badge/Recharts-22C55E) | Data Charts | Latest |

---

### Backend & Services

| Technology | Purpose |
|---|---|
| ![Base44](https://img.shields.io/badge/Base44-Backend_as_a_Service-8B5CF6) | Database, Auth, Serverless Functions |
| ![Stripe](https://img.shields.io/badge/Stripe-635BFF?logo=stripe&logoColor=white) | Payments, Webhooks, Subscription Management |
| ![Deno](https://img.shields.io/badge/Deno-000000?logo=deno) | Serverless Function Runtime |
| ![OpenAI](https://img.shields.io/badge/GPT--4-10b981?logo=openai&logoColor=white) | AI Validation, Learning Path Generation |

---

## 🗃️ Data Models

---

### Core Entities

- **`Problem`** — Millennium problem definitions, formal statements, field, difficulty rank, techniques, prerequisites

- **`Prerequisite`** — Mathematical concepts with dependency chains, difficulty levels (1–10), estimated study hours, and problem unlock mappings

- **`Technique`** — Proof techniques categorized as: `proof_method`, `construction`, `reduction`, `approximation`, `invariant`, `barrier`

- **`WorkspaceEntry`** — User proof attempts with ordered steps, justifications, validation status, and AI feedback per step

- **`ValidationLog`** — Full audit trail of AI validation events including type, result, explanation, and suggestions

- **`UserProgress`** — Per-user mastery tracking with hours spent, last studied date, status, and key insights

- **`LearningPath`** — AI-generated study sequences with assessment scores, knowledge level, learning steps, recommended papers, and progress tracking

- **`User`** *(extended)* — Built-in auth entity extended with `subscription_tier` field (`free | standard | pro`)

---

## 📈 Business Intelligence

---

### Conversion Funnel Design

1. **Discovery** → Public problem browsing (no auth required)

2. **Activation** → Sign-up triggered by locked features (AI validation, workspace limit)

3. **Engagement** → Free tier creates sunk cost via saved workspaces and tracked prerequisites

4. **Conversion** → Upgrade prompts surface exactly when free limits are hit

5. **Retention** → Long-form learning paths and incomplete proof attempts create return visits

6. **Expansion** → Pro tier upsell triggered by Standard users hitting contradiction detection walls

---

### Revenue Strategy

- **Freemium Acquisition** — Free tier lowers barrier to entry, drives organic growth

- **Feature Gating** — AI features gated to avoid commodity positioning vs. raw ChatGPT usage

- **Workspace Limits** — Hard cap at 5 entries creates natural upgrade moment at peak engagement

- **Pro Exclusivity** — Contradiction detection is a genuine technical differentiator unavailable in Standard

- **Market Positioning** — Targets PhD students, researchers, and mathematical hobbyists — high willingness-to-pay segments

- **Pricing Psychology** — $29.99 anchors Standard as affordable; $100 Pro signals serious professional tooling

---

### Retention Mechanisms

- **Progress Sunk Cost** — Tracked mastery hours and learning paths encourage return visits

- **Proof Investment** — Multi-step workspaces with AI feedback create emotional investment in specific approaches

- **Long Horizon Problems** — Millennium Problems unsolved for decades mean no user "completes" the platform

- **Export Lock-In** — Research conclusion exports are tied to active subscriptions

---

## 🎨 UI/UX Design System

---

- **Color Language** — Difficulty represented via purple→red gradient; fields mapped to distinct icon+color pairs

- **Card Elevation** — Information hierarchy via shadow depth (`shadow-sm` → `shadow-lg`)

- **Responsive Layouts** — Mobile-first grid breakpoints (`sm:`, `md:`, `lg:`) throughout

- **Animation Philosophy** — Framer Motion used for mount/unmount transitions, never decorative-only

- **Loading States** — Skeleton loaders and spinners for all async operations — no blank screens

- **Toast Notifications** — Sonner library for non-blocking feedback on save/validate/export

- **Accessible Primitives** — All interactive elements built on WAI-ARIA compliant Radix UI components

- **Gradient Accents** — Brand identity maintained via `from-indigo-500 via-purple-500 to-pink-500` system

---

## 🔐 Auth & Security

---

- **JWT Authentication** — Session management via Base44 platform

- **Role-Based Access Control** — `admin` vs `user` roles with protected routes and admin-only backend functions

- **Subscription Enforcement** — Tier checked server-side on every AI-gated API call — cannot be bypassed client-side

- **Stripe Webhook Verification** — Async signature validation using `constructEventAsync` for Deno compatibility

- **Service Role Separation** — Admin operations use elevated `base44.asServiceRole` — never exposed to frontend

---

<div align="center">

**Built with Base44 · Powered by GPT-4 · Problems sourced from [Clay Mathematics Institute](https://www.claymath.org/millennium-problems)**

*"The formulation of a problem is often more essential than its solution."* — Albert Einstein

</div>

https://the-millennium-pursuer-beb186a2.base44.app

