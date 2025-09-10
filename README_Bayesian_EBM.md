

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


```
