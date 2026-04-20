# 🎰 Prediction Market

**Personal prediction tracking — create beliefs, resolve outcomes, measure calibration**

---

A private prediction market for tracking your personal forecasts. Log what you believe will happen, assign probabilities, then come back later to resolve outcomes and see how well-calibrated your thinking really is.

No servers, no accounts, no data leaving your machine — just you versus reality.

## ✨ Features

- **localStorage persistence** — all data stays in your browser, no backend required
- **Calibration chart** — visual plot of predicted vs. actual probabilities
- **Brier scores** — rigorous scoring of prediction accuracy
- **Categories** — organize predictions by topic (tech, politics, personal, etc.)
- **Probability updates** — revise your credences over time as evidence changes
- **Import/Export** — backup your predictions as JSON, move between devices

## 🚀 Quick Start

Just open `index.html` in your browser. That's it.

For a local dev server:

```bash
python3 -m http.server 5001
# or
python3 server.py
```

Then visit [http://localhost:5001](http://localhost:5001).

## 📖 How It Works

### 1. Create Predictions

Write down a belief about the future and assign a probability (0–100%). Be specific — "Bitcoin above $100k by Dec 2026" is better than "Bitcoin goes up."

### 2. Resolve Outcomes

When the time comes, mark each prediction as **Yes** (it happened) or **No** (it didn't). Be honest — the only person you'd be fooling is yourself.

### 3. Measure Calibration

The app computes your calibration curve and scores. Over time, you'll see whether your 70% predictions actually come true ~70% of the time.

## 📊 Scoring

### Brier Score

The **Brier score** measures the accuracy of probabilistic predictions. It ranges from **0** (perfect) to **1** (worst possible):

```
Brier Score = (forecast − outcome)²
```

A score of **0.25** is the baseline — equivalent to always predicting 50%. Anything below that means you're adding real signal.

### Calibration

A perfectly calibrated forecaster has their predictions match reality: events they assign 80% probability to happen 80% of the time. The calibration chart plots your predicted probabilities against observed frequencies so you can spot systematic over- or under-confidence.

## ⌨️ Keyboard Shortcuts

| Shortcut | Action |
|----------|--------|
| `N` | New prediction |
| `Esc` | Close modal / cancel |
| `/` | Focus search |
| `E` | Export data |
| `I` | Import data |
| `C` | Toggle calibration view |

## 🎨 Part of the Creative Suite

**Project 2 of 5** in the Creative Suite — a collection of focused, single-page tools that run entirely in the browser.

## 📄 License

[MIT](LICENSE) — Copyright 2026 QuietRiverTech

---

Built by **QuietRiverTech**
