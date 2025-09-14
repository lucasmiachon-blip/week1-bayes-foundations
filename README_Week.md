# Week 2 — Math → Probability → Biostatistics/EBM (Primary) • AI tools (Secondary) • Coding (Minimal)
**Time**: 4 h/day.  
**Priority split**: 3 h core (math/prob/distributions/EBM/biostats) • 30 min AI tools • 30 min coding.  
**Tools to touch this week**: Notion, Obsidian, VS Code, Git/GitHub, Markdown.  
**Practice**: Anki daily (5–10 cards), 1 mini-calc or LR problem/day, short note in README_Math.md / README_Bayesian_EBM.md.

---

## Daily Structure (repeat each day)
- **180 min Core**: watch selected videos + do 2–3 worked examples in notes.
- **30 min AI tools**: follow a beginner video segment and set up 1 template or action.
- **30 min Coding**: one tiny task only (Python or R), saved to `week2/`.

---

## Day 1 — Precalculus refresh → Bayes intuition → EBM LR basics
**Videos**
- Precalculus essentials (limits/functions): Khan Academy (pick 2–3 short videos)  
  https://www.youtube.com/playlist?list=PLSQl0a2vh4HB3iwQV5DR_W-Tzh9aT0C9U
- Bayes intuition for medical tests (visual)  
  https://www.3blue1brown.com/lessons/better-bayes
- Likelihood ratios primer (read/skim)  
  https://www.cebm.ox.ac.uk/resources/ebm-tools/likelihood-ratios

**Practice**
- Convert 3 clinic percentages ↔ odds.  
- Compute LR+ and LR− from given sens/spec (2×2 table).  
- Note: add 5 Anki cards.

**AI tools (30 min)**  
- Notion “Introduction” → create a **Daily Note** page and a **Cases** database.  
  https://www.notion.com/help/notion-academy/course/101-introduction

**Coding (30 min)**  
- Python: create `post_prob.py` with function `post_prob(pre_prob, LR)`; test 3 cases. Save outputs.

---

## Day 2 — Calculus intuition → Distributions overview → Fagan
**Videos**
- Essence of Calculus (watch first 2 chapters)  
  https://www.youtube.com/playlist?list=PLZHQObOWTQDMsr9K-rj53DwVRMYO3t5Yr
- Probability distributions overview (StatQuest)  
  https://www.youtube.com/playlist?list=PLblh5JKOoLUK0FLuzwntyYI10UQFUhsY9
- Fagan nomogram walkthrough (short)  
  https://www.youtube.com/watch?v=UNKEvEB7jd8

**Practice**
- Use LR and pretest to get post-test probability by formula and by Fagan (one case each).  
- Anki x5.

**AI tools (30 min)**  
- Obsidian “Start HERE” video; create vault **Clinical Math** and a template note.  
  https://www.youtube.com/watch?v=QgbLb6QCK88

**Coding (30 min)**  
- R: write `post_prob(pre, LR)` and mirror Day 1 tests in R script.

---

## Day 3 — Core distributions (Normal, Binomial, Poisson) → Logistic intro
**Videos**
- Normal/Binomial/Poisson (pick 2–3 StatQuest clips)  
  https://www.youtube.com/playlist?list=PLblh5JKOoLUK0FLuzwntyYI10UQFUhsY9
- Logistic regression (concept)  
  https://www.youtube.com/playlist?list=PLblh5JKOoLUKxzEP5HA2d-Li7IJkHfXSe

**Practice**
- Compute binomial probabilities for 3 cases (R or Python), interpret clinically.  
- Anki x5.

**AI tools (30 min)**  
- Notion beginner tutorial segment; add a **Templates** database (Note, Case, Calculation).  
  https://www.youtube.com/watch?v=kOf3QSBV29Y

**Coding (30 min)**  
- Python: small script to compute Normal CDF for z values you choose; save results to Markdown.

---

## Day 4 — Frequentist vs Bayesian → Post-test workflows
**Videos**
- Bayesian vs Frequentist (short explainer)  
  https://www.youtube.com/watch?v=r76oDIvwETI
- Stat 110 Bayes & conditional probability (one lecture)  
  https://www.youtube.com/playlist?list=PL2SOU6wwxB0uwwH80KTQ6ht66KWxbzTIo

**Practice**
- Work one bedside scenario both ways: PPV/NPV vs LR/Fagan.  
- Anki x5.

**AI tools (30 min)**  
- Obsidian: set up **Templates** and enable daily notes; link to your `week2/` files.

**Coding (30 min)**  
- R: function to convert probability ↔ odds; verify three LR problems.

---

## Day 5 — GLM overview → Poisson for counts → GEE concept
**Videos**
- GLM/Design matrix intuition (StatQuest)  
  https://www.youtube.com/watch?v=CqLGvw
