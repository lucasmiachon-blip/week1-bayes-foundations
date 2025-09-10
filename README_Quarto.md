
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
