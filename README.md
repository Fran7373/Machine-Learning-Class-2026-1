# Machine Learning — Task List & Answers

This README indexes all the exercises assigned for this course. Each item below links directly to where the answer lives in this repository (notebook, script,folder, or PDF), so the professor can jump straight to the corresponding solution.


## Questions & Answers

1. **Hoeffding inequality doesn't apply** — Exercise 1.10: Simulate flipping 1,000 fair coins, 10 flips each. Track three coins: `c_1` (first coin flipped), `c_rand` (a randomly chosen coin), and `c_min` (the coin with the minimum fraction of heads, earliest one in case of a tie). Let `v_1`, `v_rand`, `v_min` be the fraction of heads for each.
   - (a) What is μ for the three selected coins?
   - (b) Repeat the experiment many times (e.g., 100,000 runs) to get many instances of `v_1`, `v_rand`, `v_min`, and plot histograms of their distributions.
   - (c) Using (b), plot estimates of P[|v − μ| > ε] as a function of ε, together with the Hoeffding bound 2e^(−2ε²N), on the same graph.
   - (d) Which coins obey the Hoeffding bound, and which don't? Explain why.
   - (e) Relate part (d) to the multiple-bins figure.
     
     <img width="467" height="387" alt="image" src="https://github.com/user-attachments/assets/6ab30077-9e2d-4992-8c8c-28d6f6fbd134" />

   → [Answer](./Exercise1_10.ipynb)

2. **Entropy** — Prove that log₂ P(X = i) represents the number of binary questions needed to identify a message with that probability, and derive why the entropy of a random variable can be expressed with the attached formula.
   
   <img width="344" height="88" alt="image" src="https://github.com/user-attachments/assets/9815e7e2-b933-42d0-81fc-e35ee5aa3818" />

   → [Answer](./Entropy_BinaryRepresentationOfQuestions.pdf)

3. **Support Vector Machine** — The optimization problem behind finding the best weights for an SVM; develop it using convex optimization.
   → [Answer](./SVMOpti.ipynb)

4. **Perceptron** — Implement the perceptron algorithm and explain why it works. Complete exercises 1.2 and 1.3, plus answer:
   <img width="510" height="375" alt="image" src="https://github.com/user-attachments/assets/452b5c5d-2922-4f03-bd9c-c503e6dd6de3" />

   - (a) Does the algorithm find the correct parameters (does it separate the data)?
   - (b) Does the algorithm stop in a finite number of steps? How is convergence guaranteed?
   - (c) Why does it work? (This connects to exercise 1.3.)
   → [Answer](./Exercice4)

5. **XOR modeling** — Model XOR by connecting several basic neurons, then model XOR using perceptrons with specific weights for each one.
   → [Answer](#./XORWithMPNeuronsAndPerceptrons.pdf)

6. **Netflix Prize via SVD** — Read the *KDD Cup 2007 Task 1 Winner Report* (co-authored by Miklós Kurucz) and explain in detail how the Netflix Challenge was addressed using SVD. (Hint: draw a parallel between Topics vs. Genres and Genres vs. Movies to reason about the factorization's behavior.)
   → [Answer](./SVDSolvedWhoRatedWhatProblem.pdf)

7. **KNN** — What is the hypothesis set of the K-Nearest-Neighbours learning model? What is its learning algorithm?
   → [Answer](#)

8. **Concentration bounds**
   - (a) Prove the Markov bound and give one example.
   - (b) Prove the Chebyshev bound.
   - (c) Prove the Hoeffding bound (assuming Hoeffding's Lemma).
   → [Answer](./ConcentrationBounds.pdf)

9. **Inequalities (learning slide 29/30)** — Answer the last question: μ is the cause of ν, but we can infer that μ ≈ ν. Why?
   <img width="569" height="348" alt="image" src="https://github.com/user-attachments/assets/2cfb6b63-f610-4cb8-83a1-687728cd2235" />

   → [Answer](./WhyMuIsApproximatelyNu.pdf)

10. **Hoeffding inequality — parameter control** — Given ε and δ = 2Me^(−2Nε²), which parameter better controls N (the number of data points)?
    → [Answer](./EpsilonVSDelta.pdf)

11. **Effective number of separating lines** — What is the effective number of lines that can separate 5 points (into 2 labels) in ℝ²? (Consider all possible lines separating the 5 points into two classes, discard the cases where no line can separate them, and count the effective number of lines.)
    → [Answer](./Exercice11PointSeparation.png)

12. **Shallow neural network kinks** — What is the origin of the "joints"/kinks in a shallow neural network?
   <img width="564" height="326" alt="image" src="https://github.com/user-attachments/assets/374cb997-57e4-4488-8085-62397e11fd80" />

    → [Answer](./ReLUNumberHipotesis.pdf)

13. **Folds/creases** — How many folds can this have? 
<img width="553" height="343" alt="image" src="https://github.com/user-attachments/assets/9c27c8dd-8e90-4321-b5bb-083d620eda32" />

 → [Answer](./ReLUNumberHipotesis.pdf)

