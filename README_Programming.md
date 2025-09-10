
**R (15–20 min/day)**

* Open RStudio → New Script. Practice:

```
x <- c(0.2, 0.5, 0.8)
odd <- x/(1-x)
post_odd <- odd * 4  # example LR+
post_p <- post_odd/(1+post_odd)
post_p
```

* Read CSV example:

```
d <- data.frame(test=c("pos","neg","pos"), disease=c(1,0,1))
prop.table(table(d$test, d$disease), 1)
```

**Python (15–20 min/day)**

```
ps = [0.2, 0.5, 0.8]
def prob_to_odds(p):
    return p/(1-p)

def odds_to_prob(o):
    return o/(1+o)

LRp = 4
post = [odds_to_prob(prob_to_odds(p)*LRp) for p in ps]
print(post)
```

* Extend: ask user input for pretest and LR, print post‑test.

**Principle**: tiny scripts that compute real clinical examples.

---

## README\_Math.md — algebra → logs → functions

**Sequence**

1. Variables and linear equations (solve for x)
2. Functions: f(x), slope, intercept; read graphs
3. Exponents and scientific notation
4. Logarithms: definition, ln vs log10; change‑of‑base
5. Percentages ↔ decimals; probability vs odds

**Checkpoint questions**

* Solve: 3x + 5 = 20
* If f(x)=2x+1, what is f(3)?
* Convert 0.2 to odds; convert odds 3 to probability
* If p=0.1 and LR+=8, compute post‑test probability

**Tip**: when stuck, write steps; avoid mental math; check with calculator.

---

## README\_Bayesian\_EBM.md — from LRs to Bayes

**Concept map**

* Pretest probability → convert to odds → multiply by LR (or divide by LR−) → posterior odds → convert to probability.

**Core formulas**

* Odds = p/(1−p)
* Posterior odds (positive test) = Prior odds × LR+
* Posterior odds (negative test) = Prior odds × LR−
* LR+ = sens/(1−spec); LR− = (1−sens)/spec

**Practice set**

1. p=0.30, LR+=5 → post‑test?
2. p=0.60, LR−=0.2 → post‑test?
3. p=0.05, LR+=12 → post‑test?

**Vignette template**

* Write a 3‑line case.
* State a pretest probability.
* Look up LR for one finding or test.
* Compute post‑test probability.
* Decide: below test threshold, between test and treat thresholds, or above treat threshold.

**Stretch goals (later weeks)**

* Compare Bayesian vs frequentist language.
* Simple conjugate priors (Beta‑Binomial) with R.
* Intro to MCMC idea; why we need sampling.

---

## README\_Quarto.md — first render

**Steps**

1. RStudio: *File → New File → Quarto Document…*
2. Title: `Bayes and Fagan` → **Create**
3. Replace body with a worked LR example and a small R chunk.
4. Click **Render**. Check the HTML in the preview pane.
5. Save as `bayes-fagan.qmd` in the repo.

**Minimal chunk**

````
```{r}
pretest <- 0.2; LRp <- 4
odds <- pretest/(1-pretest)
post <- (odds*LRp)/(1+odds*LRp)
post
````

```

---

## README_GitHub_README_Principles.md — how to write

**Keep it** short, scannable, link‑rich. Put a purpose line at top.

**Template**
```

# Project name

One‑line purpose.

## What is inside

* Key files
* How to run
* Links to videos/resources used

## Quick start

* Step 1
* Step 2

## License / Credits

```

**Markdown cheats you’ll use daily**
- `# H1`, `## H2`, `**bold**`, `*italics*`, backticks for code, lists with `-`.
- Use relative links between READMEs.

---

### Checklist — end of week
- [ ] Repo created and pushed
- [ ] All README files filled with links
- [ ] Quarto HTML rendered
- [ ] 50+ Anki cards made and reviewed
- [ ] Three vignettes solved with LR → posterior

```
