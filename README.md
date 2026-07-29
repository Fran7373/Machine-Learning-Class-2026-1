# Machine Learning — Task List & Answers

This README indexes all the exercises assigned for this course. Each item below links directly to where the answer lives in this repository (notebook, script, or PDF), so the professor can jump straight to the corresponding solution.

> All answers in this repository are written in English.

---

## How the links work

Each question links to a specific file (and, where useful, a specific section/heading inside that file) instead of just the repo root. There are two ways I used to do this — pick whichever fits how you organize your repo:

**1. Link straight to a file (or a folder) in the repo**
GitHub resolves relative paths automatically, so from this README you can just write:
```markdown
[Answer](./notebooks/01_hoeffding_simulation.ipynb)
[Answer](./answers/02_entropy.pdf)
[Answer](./src/perceptron.py)
```
If you want the professor to land on a specific commit/version instead of "whatever is on main right now", use a permalink (press `y` on GitHub while viewing the file to get a URL locked to that commit), e.g.:
```markdown
[Answer](https://github.com/<user>/<repo>/blob/<commit-sha>/notebooks/01_hoeffding_simulation.ipynb)
```

**2. Link to a specific heading inside one long file (anchor link)**
If all answers live in a single Markdown file or notebook, GitHub auto-generates an anchor for every heading: lowercase the text, replace spaces with hyphens, strip punctuation. So a heading like:
```markdown
## 4. Perceptron
```
gets the anchor `#4-perceptron`, and you link to it like this:
```markdown
[Answer](./ANSWERS.md#4-perceptron)
```
This also works pointing *into* this same README if you keep answers below the questions instead of in separate files.

I used placeholder links (`#`) below — swap each one for the real path/anchor once you drop this into your repo.

---

## Questions & Answers

1. **Hoeffding inequality doesn't apply** — Exercise 1.10: Simulate flipping 1,000 fair coins, 10 flips each. Track three coins: `c_1` (first coin flipped), `c_rand` (a randomly chosen coin), and `c_min` (the coin with the minimum fraction of heads, earliest one in case of a tie). Let `v_1`, `v_rand`, `v_min` be the fraction of heads for each.
   - (a) What is μ for the three selected coins?
   - (b) Repeat the experiment many times (e.g., 100,000 runs) to get many instances of `v_1`, `v_rand`, `v_min`, and plot histograms of their distributions.
   - (c) Using (b), plot estimates of P[|v − μ| > ε] as a function of ε, together with the Hoeffding bound 2e^(−2ε²N), on the same graph.
   - (d) Which coins obey the Hoeffding bound, and which don't? Explain why.
   - (e) Relate part (d) to the multiple-bins figure.
   → [Answer](#)

2. **Entropy** — Prove that log₂ P(X = i) represents the number of binary questions needed to identify a message with that probability, and derive why the entropy of a random variable can be expressed with the attached formula.
   → [Answer](#)

3. **Support Vector Machine** — The optimization problem behind finding the best weights for an SVM; develop it using convex optimization.
   → [Answer](#)

4. **Perceptron** — Implement the perceptron algorithm and explain why it works. Complete exercises 1.2 and 1.3, plus answer:
   - (a) Does the algorithm find the correct parameters (does it separate the data)?
   - (b) Does the algorithm stop in a finite number of steps? How is convergence guaranteed?
   - (c) Why does it work? (This connects to exercise 1.3.)
   → [Answer](#)

5. **XOR modeling** — Model XOR by connecting several basic neurons, then model XOR using perceptrons with specific weights for each one.
   → [Answer](#)

6. **Netflix Prize via SVD** — Read the *KDD Cup 2007 Task 1 Winner Report* (co-authored by Miklós Kurucz) and explain in detail how the Netflix Challenge was addressed using SVD. (Hint: draw a parallel between Topics vs. Genres and Genres vs. Movies to reason about the factorization's behavior.)
   → [Answer](#)

7. **KNN** — What is the hypothesis set of the K-Nearest-Neighbours learning model? What is its learning algorithm?
   → [Answer](#)

8. **Concentration bounds**
   - (a) Prove the Markov bound and give one example.
   - (b) Prove the Chebyshev bound.
   - (c) Prove the Hoeffding bound (assuming Hoeffding's Lemma).
   → [Answer](#)

9. **Inequalities (learning slide 29/30)** — Answer the last question: μ is the cause of ν, but we can infer that μ ≈ ν. Why?
   → [Answer](#)

10. **Hoeffding inequality — parameter control** — Given ε and δ = 2Me^(−2Nε²), which parameter better controls N (the number of data points)?
    → [Answer](#)

11. **Effective number of separating lines** — What is the effective number of lines that can separate 5 points (into 2 labels) in ℝ²? (Consider all possible lines separating the 5 points into two classes, discard the cases where no line can separate them, and count the effective number of lines.)
    → [Answer](#)

12. **Shallow neural network kinks** — What is the origin of the "joints"/kinks in a shallow neural network?
    → [Answer](#)

13. **Folds/creases** — How many folds can this have? (referring to the attached figure)
    → [Answer](#)

---

*Repository maintained for [course/professor name] — Machine Learning.*
