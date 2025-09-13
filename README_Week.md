# Week 1 — Bayesian EBM Foundations (links + minutes)

Daily cadence (45–75 min)
- 10–15 min Algebra
- 15–25 min Probability/Bayes (clinician focus)
- 10–15 min Programming (R or Python)
- 5–10 min Tooling (repo, Quarto, Anki, bookmarks)

Links (used all week)
- Algebra — https://www.khanacademy.org/math/algebra
- Probability — https://www.khanacademy.org/math/statistics-probability
- Harvard Stat 110 playlist — https://www.youtube.com/playlist?list=PL2SOU6wwxB0uwwH80KTQ6ht66KWxbzTIo
- CEBM: Likelihood Ratios — https://www.cebm.ox.ac.uk/resources/ebm-tools/likelihood-ratios
- Fagan explainer — https://s4be.cochrane.org/blog/2016/07/26/fagans-nomogram-for-bayes-theorem/
- Quarto Get Started — https://quarto.org/docs/get-started/
- GitHub Hello World — https://docs.github.com/en/get-started/start-your-journey/hello-world
- Anki Manual — https://docs.ankiweb.net/
- Python for Everybody — https://www.coursera.org/specializations/python
- R Programming (JHU) — https://www.coursera.org/learn/r-programming

---

## Day 1 (45–75 min)
Algebra (10–15): Khan → Variables and two-step equations (first unit).
Probability/Bayes (15–25): CEBM Likelihood Ratios; read Fagan explainer.
Programming (10–15): RStudio basics (Console, Run) or start PY4E/R Programming.
Tooling (5–10): Create/verify repo `week1-bayes-foundations`; enable 2FA; Quarto “Hello” render.
Ship: commit `day1: algebra notes, LR notes, first render`.

## Day 2 (45–75 min)
## Day 2 — Tooling Links
- GitHub Markdown basics: https://docs.github.com/en/get-started/writing-on-github/getting-started-with-writing-and-formatting-on-github/basic-writing-and-formatting-syntax
- GitHub writing quickstart: https://docs.github.com/en/get-started/wwriting-on-github/getting-started-with-writing-and-formatting-on-github/quickstart-for-writing-on-github
- GitHub-Flavored Markdown spec: https://github.github.com/gfm/
- Python docs (latest): https://docs.python.org/3/
- Python tutorial: https://docs.python.org/3/tutorial/index.html
- Python docs by version: https://www.python.org/doc/versions/

## Day 3 (45–75 min)
Algebra (10–15): Multi-step linear equations.
Probability/Bayes (15–25): Work 3 vignettes; use Fagan method.
Programming (10–15): Add a table of cases in `bayes-fagan.qmd` and render HTML.
Tooling (5–10): Short “Formulas” and “Takeaways” sections.
Ship: `day3: vignettes table + formulas`.

## Day 4 (45–75 min)
Algebra (10–15): Intro to exponents and logs (properties).
Probability/Bayes (15–25): Log-odds view: posterior logit = prior logit + log(LR).
Programming (10–15): Implement `logit`, `inv_logit`, `post_prob_log`; check equals `post_prob`.
Tooling (5–10): Update README with one paragraph on log-odds.
Ship: `day4: logit method + checks`.

## Day 5 (45–75 min)
Algebra (10–15): Fractions with variables; simplify.
Probability/Bayes (15–25): Multiple independent tests → multiply LRs (or add log LRs).
Programming (10–15): Add a multi-test example chunk; verify results match both methods.
Tooling (5–10): Clean repo; push.
Ship: `day5: multi-test example`.

## Day 6 (45–75 min)
Algebra (10–15): Quick mixed practice (percent, ratio, solve for x).
Probability/Bayes (15–25): Mixed set of 5 cases (2 positive LRs, 3 negative).
Programming (10–15): Render PDF (install TinyTeX if needed).
Tooling (5–10): Save `bayes-fagan.html/pdf`; push.
Ship: `day6: mixed cases + pdf`.

## Day 7 (45–75 min)
Algebra (10–15): Light review.
Probability/Bayes (15–25): Summarize what changes pre→post most; note LR thresholds.
Programming (10–15): Small refactor of helper functions; tidy file.
Tooling (5–10): Write a 5-bullet summary in `README_Bayesian_EBM.md`; optional GitHub Pages.
Ship: `day7: weekly summary + publish`.

---

## Quick checks (put in bayes-fagan.qmd)
- Pre 0.20, LR+ 4 → 0.50
- Pre 0.60, LR− 0.2 → ≈0.231
- Pre 0.05, LR+ 12 → ≈0.387

