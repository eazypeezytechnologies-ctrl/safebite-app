# 🛡️ SafeBite
"Scan products. Detect allergens. Protect real people."

🚧 Actively under development — real-world tested with live product scans

## 💡 Why I Built SafeBite

SafeBite started as a personal solution.

My daughter has allergies and eczema, and like many parents, I realized quickly that reading labels isn’t enough. Ingredients are often hidden, unclear, or change without notice.

As she grows, her allergies evolve — which makes it even harder to trust what’s actually safe.

I didn’t want to rely on guesswork.

So I built SafeBite — a system that scans products and helps families make safer decisions in real time, based on their specific needs.

This is not a demo project.

It’s something I actively use and test in real life.

## Overview
SafeBite is a mobile app that helps users scan food and beauty products to detect allergens, ingredients, and safety concerns in real time.

## Features
- Barcode-based product lookup
- Ingredient and allergen detection
- Mobile-friendly experience
- Cached product results for faster repeat searches
- Built for real-world daily use

## 🧠 Key Innovation

SafeBite uses a dual-layer safety system:

- AI analysis for interpreting ingredients and labels  
- Rule-based validation to prioritize known allergen risks  

When results conflict, the system defaults to the safer outcome, reducing the chance of harmful recommendations.

## 🆕 Latest Progress — v3.0 (Core System Stabilization)

April 10th, 2026

### 🧠 Unified Evaluation Engine (CORE BREAKTHROUGH)
- Replaced all legacy `calculateVerdict()` logic with a single unified evaluation system
- Introduced clear decision hierarchy:
  - Direct allergen match → highest priority
  - AI validation → overrides false positives
  - Trusted products → safe override (with safeguards)
  - Incomplete data → lowers confidence

**Result:**
- Consistent verdicts across ALL screens
- Eliminated conflicting logic between AI + rule engine

---

### ⚡ Performance Optimization (Scan → Result Flow)

**Before:**
- 10+ API sources (many useless)
- Sequential calls (slow)
- 30s timeouts + retries
- UI blocked during loading

**After:**
- Reduced to high-value sources (OpenFoodFacts + USDA)
- Parallelized:
  - API calls
  - Cache checks
  - Background processing

**Improvements:**
- Faster scan response
- Instant product display
- Background loading for secondary data
- Reduced timeouts (30s → 8s)

---

### 🔐 Supabase Backend Fully Activated

**Critical Fix:**
- Added `SUPABASE_SERVICE_KEY`

**Now Working:**
- Profile CRUD
- Scan history logging
- Product caching (UPSERT)
- Analytics tracking
- RPC functions

---

### 📊 Data Pipeline Audit

**Strong Sources:**
- OpenFoodFacts
- Supabase
- AI analysis

**Removed / Reduced:**
- UPCItemDB
- EAN Search
- Datakick
- Unused APIs

---

### 🔄 Scan Stability Fixes
- Prevented duplicate scans
- Added cooldown + dedupe logic
- Improved scan reliability

---

### 🧪 Real-World Testing Insights

**Issues Found:**
- Profile update error (PGRST204)
- Minor async/state warnings
- Missing AI alternatives
- Incomplete dietary preferences

---

### 🧭 Product Direction

SafeBite is evolving into:

> A personalized safety assistant for families — not just a barcode scanner

Key realization:
- Allergies ≠ Eczema ≠ Preferences

---

### 🧩 Next Sprint
1. Fix profile schema mismatch
2. Clean async/state errors
3. Expand dietary preferences
4. Restore AI alternatives

---

### 🏁 Current Status

- Core system working  
- Backend connected  
- Performance improved  
- Final stability in progress  

## 📸 App Preview

### 🛡️ Allergy Guardian (Home)
<img src="./screenshots:/home.jpg" width="300" />

### 👨‍👩‍👧 Multi-Profile Safety System
<img src="./screenshots:/profiles.jpg" width="300" />

### 📷 Smart Scanning
<img src="./screenshots:/classic-scan.jpg" width="300" />

### 🧠 AI Processing Pipeline
<img src="./screenshots:/ai-capture-processing.jpg" width="300" />


### 📊 Scan Results & History
<img src="./screenshots:/history.jpg" width="300" />

## Tech Stack
- React Native
- Expo
- TypeScript
- Supabase
- External product APIs
- Node.js (API layer)

## What I Learned
- Structuring a mobile app around real user safety needs
- Working with third-party APIs and fallback logic
- Designing app flows that balance speed, trust, and usability

## Status
In active development and being expanded with stronger UX, better product intelligence, and improved reliability.

## Author
Babatunde Jegede
