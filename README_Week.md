# Week 2 Plan — Math/EBM first. AI tools second. Teaching third. Coding last.
Time per day: **4h**. Split: **3h Math/Prob/EBM/Biostats** · **45m AI tools** · **15m Coding**.  
Preference: videos first. Keep notes in `docs/` as Markdown. Track with Anki.

---

## Day 1 — Precalculus ➜ Calculus (limits, derivatives) · VS Code + Markdown
**Watch (80–90m)**
- Khan Academy Precalculus (start “Functions” then “Trig”): https://www.khanacademy.org/math/precalculus
- 3Blue1Brown *Essence of Calculus* (chapters 1–3): https://www.youtube.com/playlist?list=PLZHQObOWTQDMsr9K-rj53DwVRMYO3t5Yr

**Read (10m)**
- Khan Academy Calculus 1 overview: https://www.khanacademy.org/math/calculus-1

**Practice (60m)**
- KA exercises on limits/derivative intuition (same links).
- Notes: `docs/Math_Week2_D1.md` with worked examples.
- Anki: 8 cards (limits, derivative idea, slope as rate, common pitfalls).

**AI tools (30–45m)**
- ChatGPT “Getting started” overview: https://help.openai.com/en/collections/3742473-chatgpt
- Prompt demo: ask for a step-by-step limit proof, then rewrite simpler.

**Coding (15m)**
- VS Code intro video: https://code.visualstudio.com/docs/getstarted/introvideos
- Create `notes/README.md` and use preview side-by-side.

**Ship**
- Commit `docs/Math_Week2_D1.md` + 8 Anki cards.

---

## Day 2 — Probability basics · Diagnostic LRs (LR+, LR–)
**Watch (60–75m)**
- Harvard Stat 110 playlist (Lectures 1–2 selections): https://www.youtube.com/playlist?list=PL2SOU6wwxB0uwwH80KTQ6ht66KWxbzTIo
- CEBM Likelihood Ratios (quick read): https://www.cebm.ox.ac.uk/resources/ebm-tools/likelihood-ratios

**Practice (75–90m)**
- Compute LR+ = sens/(1–spec); LR– = (1–sens)/spec on 3 tests.
- Convert pretest→posttest with odds and with Fagan nomogram:
  - Fagan explainer: https://pmc.ncbi.nlm.nih.gov/articles/PMC4744617/

**AI tools (30–45m)**
- Google Cloud “Intro to Generative AI” (45min micro-course): https://www.cloudskillsboost.google/course_templates/536

**Coding (15m)**
- Python `post_prob(pre, LR)` and R equivalent; test 3 cases. Save `code/day2_prob.py`, `code/day2_prob.R`.

**Ship**
- `docs/EBM_LRs.md` with 3 worked clinical examples + screenshots of Fagan lines.

---

## Day 3 — Distributions (normal, binomial, Poisson) · PPV/NPV vs LRs
**Watch (60–70m)**
- StatQuest “Probability Distributions” + Normal + Binomial:  
  - https://www.youtube.com/watch?v=oI3hZJqXJuc  
  - https://www.youtube.com/watch?v=rzFX5NWojp0  
  - https://www.youtube.com/watch?v=J8jNoF-K8E8

**Practice (80–90m)**
- From sensitivity/specificity, compute PPV/NPV at 3 prevalences; compare to LR method.

**AI tools (30–45m)**
- Coursera “Generative AI for Everyone” Module 1: https://www.coursera.org/learn/generative-ai-for-everyone

**Coding (15m)**
- R: `dbinom`, `pbinom`, `ppois` quick checks that match your manual calcs.

**Ship**
- `docs/Distributions_Notes.md` + table comparing PPV/NPV vs LR-derived post-test.

---

## Day 4 — Biostatistics core: hypothesis tests, CIs, Logistic regression intro
**Watch (75–90m)**
- StatQuest Logistic Regression intro and odds/OR:  
  - https://www.youtube.com/watch?v=ARfXDSkQf1Y  
  - https://www.youtube.com/watch?v=8nm0G-1uJzA  
  - https://www.youtube.com/watch?v=yIYKR4sgzI8

**Practice (60–75m)**
- Build 2×2 tables from case vignettes. Compute OR, 95% CI (approx). Interpret.

**AI tools (30–45m)**
- Notion Academy 101 (first lessons) + Notion AI basics: https://www.notion.com/help/notion-academy/course/101-introduction

**Coding (15m)**
- R: `glm(y~x, family=binomial, data=...)` on a toy dataset. Save code + interpretation.

**Ship**
- `docs/Logistic_Regression_FirstSteps.md` with OR vs RR vs OR_logit explanations.

---

## Day 5 — GLM overview → GEE for correlated data
**Watch (60–75m)**
- StatQuest GLMs overview: https://statquest.org/statquest-linear-regression-aka-glms-part-1/
- UW BIRCH “Foundations of GEE for Longitudinal Analysis”: https://www.youtube.com/watch?v=rDfHfkTRlak
- PSU STAT 504 GEE notes (Lesson 12): https://online.stat.psu.edu/stat504/lesson/12

**Practice (75–90m)**
- Identify when GEE is appropriate from 3 clinical study abstracts. Specify link, family, working correlation you’d choose.

**AI tools (30–45m)**
- Notion: build a simple patient-study database with “Study design, Outcome, Repeated? yes/no”.

**Coding (15m)**
- R: sketch formula for GEE (no deep run needed). Note `geepack::geeglm` for later.

**Ship**
- `docs/GEE_When_and_Why.md` with examples and decisions.

---

## Day 6 — Teaching & Assessment: IRT + Standard setting (Angoff)
**Watch (60–75m)**
- IRT introductions:  
  - https://www.youtube.com/watch?v=_VzpAU3vuLg  
  - https://www.youtube.com/watch?v=IuzR9rsfUlE
- Modified Angoff overview: https://www.youtube.com/watch?v=bQF1kSlZkBE

**Practice (75–90m)**
- Draft a 6-item checklist for your rotation exam. Run a **mock Modified Angoff** with yourself. Record cut score method and rationale.

**AI tools (30–45m)**
- Obsidian beginner video: https://www.youtube.com/watch?v=QgbLb6QCK88  
  Create a vault “Teaching/IRT” and link notes.

**Coding (15m)**
- R: install `mirt` and note 2 functions you’ll try next week.

**Ship**
- `docs/IRT_and_CutScores.md` with your mock Angoff table and decisions.

---

## Day 7 — Review + Integration
**Watch (30–45m)**
- 3Blue1Brown calc recap (pick 2 chapters): https://www.youtube.com/playlist?list=PLZHQObOWTQDMsr9K-rj53DwVRMYO3t5Yr
- CEBM SpPin/SnNout refresher: https://www.cebm.ox.ac.uk/resources/ebm-tools/sppin-and-snnout

**Practice (120m)**
- One full clinical workflow: pretest → choose test → LR → post-test → decision.
- Summarize all week in `docs/Week2_Summary.md`.

**AI tools (30–45m)**
- ChatGPT Educators quick-start prompts: https://help.openai.com/en/articles/8313929-how-can-educators-get-started-with-chatgpt

**Coding (15m)**
- Clean repo; tag `week2-done`.

**Ship**
- Push repo. Share `Week2_Summary.md`. Add 20 Anki cards from weak spots.

---

## Tooling quick links
- VS Code intros: https://code.visualstudio.com/docs/getstarted/introvideos
- Git & GitHub crash course (video): https://www.youtube.com/watch?v=vA5TTz6BXhY
- Python docs: https://docs.python.org/3/
- R quick video: https://www.youtube.com/watch?v=eR-XRSKsuR4
- Java 1-hour intro: https://www.youtube.com/watch?v=XWnwR-Rxjk8
- Anki download: https://apps.ankiweb.net/

---

## Tracking
Update these each night in `docs/Week2_Summary.md`:
- **Learned well:** …
- **Needs more practice:** …
- **Not started:** …

Add 10–20 Anki cards per day from problems you missed.

---

## Folder structure

## EXTRA  
## Focus Course: Logarithms (Khan Academy)
Link: https://www.khanacademy.org/math/algebra2/x2ec2f6f830c9fb89%3Alogs
https://www.khanacademy.org/math/trigonometry?utm_source=chatgpt.com

### Why for biostats
- Natural log (ln), base-10 log, change of base
- Log rules for transformations, OR/log-odds, log-likelihood intuition

### How to complete (2–3 sessions)
1) Sign in → open the unit → turn on “Unit mastery”.
2) Do in order: intro → e & ln → properties → change of base → solve log eqs → graph logs → applications.
3) After each subtopic: finish the practice until “Mastered”.

### Minimum outputs
- Notes: 1 page of rules + 3 worked examples (incl. ln).
- Anki: 8 cards (definitions, properties, change-of-base, two solved eqs).
- Quick check: derive ln(ab)=ln a+ln b and solve log10 x = 3 → x=1000.


# Inial Prompt

Primary focus: math (precalculus and calculus), probability, distributions, EBM, and biostatistics.
Secondary: start with AI principles and AI tools (include Notion and Obsidian).
Coding: very short daily block, from zero.

I have 4 hours per day. Create a plan in README format. I prefer videos; include the video links directly in the text. Spend most of the time on math/probability/distributions/EBM/biostatistics. Keep coding time small.

Assume I am a beginner in AI, AI tools, and programming, and I have limited background in precalculus, calculus, probability, and EBM. I want to learn quickly and survey a wide set of AI tools and their core principles. In biostatistics I need both Bayesian and frequentist methods, distributions, GLM, GEE, and newer methods, in a natural order starting from basics. We can use R to practice the math as we go.

I have Coursera Plus, Udemy, and edX. I can pay for a highly rated course if needed. When possible, prefer Khan Academy to track progress.

For each day, include:

A time budget that sums to 4 hours

Video links

Short practice tasks I can do now

Anki prompts to add

At the end of the plan, add three lists for longitudinal tracking:

Learned well

Needs more practice

Not started

Order of priority:

Math (precalculus and calculus), probability, biostatistics, EBM

AI principles and tools

Teaching strategies, Item Response Theory, and pass/fail cutoff methods

Coding from zero (Git, GitHub, VS Code, Markdown, Python, R, Java)

#  Adicionar
---
###  Theory of information

### Trigonometry advanced

### Pre calculus
---  
#  Aprendido





