<div align="center">

<!-- Typing SVG -->
<a href="https://git.io/typing-svg">
  <img src="https://readme-typing-svg.demolab.com?font=JetBrains+Mono&weight=700&size=28&pause=1000&color=00F7F4&center=true&vCenter=true&width=700&lines=Shahid+Ul+Islam;ML+Engineer+%7C+XAI+Researcher;Building+models+you+can+actually+trust." alt="Typing SVG" />
</a>

<br/>

<p>
  <a href="https://khanz9664.github.io/portfolio/"><img src="https://img.shields.io/badge/Portfolio-FF5722?style=for-the-badge&logo=todoist&logoColor=white"/></a>
  <a href="mailto:shahid9664@gmail.com"><img src="https://img.shields.io/badge/Email-D14836?style=for-the-badge&logo=gmail&logoColor=white"/></a>
  <a href="https://linkedin.com/in/shahid-ul-islam-13650998"><img src="https://img.shields.io/badge/LinkedIn-0077B5?style=for-the-badge&logo=linkedin&logoColor=white"/></a>
  <a href="https://x.com/Shaddy9664"><img src="https://img.shields.io/badge/X%2FTwitter-000000?style=for-the-badge&logo=x&logoColor=white"/></a>
  <a href="https://pypi.org/project/trustlens/"><img src="https://img.shields.io/badge/PyPI-trustlens-3775A9?style=for-the-badge&logo=pypi&logoColor=white"/></a>
</p>

<p>
  <img src="https://komarev.com/ghpvc/?username=Khanz9664&label=Profile+Views&color=0e75b6&style=flat-square" />
  <img src="https://img.shields.io/github/followers/Khanz9664?label=Followers&style=flat-square&color=00F7F4" />
  <img src="https://img.shields.io/github/stars/Khanz9664?label=Total+Stars&style=flat-square&color=FF6E4A" />
</p>

</div>

---

<!-- ─── WHO I AM ─────────────────────────────────────────────────────────── -->

> *Most teams stop at accuracy. I ask: **why** did the model decide that — and can you **prove** it?*

I'm a Machine Learning Engineer specializing in **Explainable AI (XAI)** and **clinical ML systems**. My work sits at the boundary between statistical rigor and software engineering — building pipelines that are not only high-performing but *accountable*.

My research uncovered what I call the **Explainability Paradox**: visually convincing saliency maps that fail causal validity tests. That finding is now under peer review.

---

<!-- ─── FEATURED: TRUSTLENS ────────────────────────────────────────────────── -->

## TrustLens — Open-Source ML Reliability Framework

<a href="https://github.com/Khanz9664/TrustLens">
  <img align="right" alt="coding gif" width="360" src="https://media.giphy.com/media/L1R1tvI9svkIWwpVYr/giphy.gif"/>
</a>

Most evaluation stops at `accuracy_score`. **TrustLens** goes deeper.

A single `analyze()` call surfaces calibration drift, subgroup bias, failure patterns, and representation quality — the things that matter in production, but don't appear on leaderboards.

```python
from trustlens import analyze

report = analyze(model, X_val, y_val, y_prob=proba)
# → Calibration · Bias · Failure Modes · Representation
```

**Live on PyPI** · Built with production CI/CD (multi-Python testing, Ruff, MyPy) · Active contributor community

<br clear="right"/>

→ [Full writeup](https://khanz9664.github.io/portfolio/projects/trustlens.html) &nbsp;|&nbsp; [PyPI package](https://pypi.org/project/trustlens/) &nbsp;|&nbsp; [Repository](https://github.com/Khanz9664/TrustLens)

---

<!-- ─── RESEARCH ────────────────────────────────────────────────────────── -->

## Research

### Paper Under Review
**Quantitative Faithfulness Benchmarking of CNNs vs. Vision Transformers: Implications for Clinical Trustworthiness**

I Trained 3 different Models (VGG16, ViT B/16 and Custom CNN) and ran GradCAM++ and EigenCam on a chest X-ray dataset and found something counterintuitive: **visually plausible heatmaps lacked causal validity**. A 6-dimensional benchmark along with Pixel Deletion (AOPC/AUC) showed that patch-based Transformer attention was causally faithful where CNNs weren't — despite CNNs looking more "correct" to the human eye. I call this the **Explainability Paradox**.

*Metrics used: Sparsity · Entropy · Inter-Method Agreement · AOPC/AUC · Bonferroni-corrected non-parametric testing*

→ [Project writeup](https://khanz9664.github.io/portfolio/projects/TransferLearning.html) &nbsp;|&nbsp; [Repository](https://github.com/Khanz9664/Transfer-Learning-for-Respiratory-Disease-Classification)

---

### Open-Source Contribution: Roboflow Supervision

**Merged PR [#2247](https://github.com/roboflow/supervision/pull/2247) — Add OBB Support to `ConfusionMatrix` via `MetricTarget`**

Implemented Oriented Bounding Box (OBB) support for `ConfusionMatrix`, enabling correct IoU computation for rotated detections through `MetricTarget.ORIENTED_BOUNDING_BOXES`. This aligned `ConfusionMatrix` with the library's existing metrics architecture and resolved a long-standing gap where OBB inputs were evaluated using axis-aligned IoU. The contribution included validation logic, regression tests, documentation updates, and full backward compatibility with existing workflows.

---

<!-- ─── DEPLOYED SYSTEMS ───────────────────────────────────────────────── -->

## Deployed Systems

| System | Stack | Live | Highlight |
|--------|-------|------|-----------|
| **[CardioSense-AI](https://github.com/Khanz9664/CardioSense-AI)** | XGBoost · FastAPI · Docker · Optuna | [🟢 Live](https://cardio-sense-ai.streamlit.app/) | 90.16% acc · 0.9524 AUC · "Least Effort Path" optimizer for patient intervention |
| **[Breast Cancer MLOps Suite](https://github.com/Khanz9664/Breast-Cancer-Prediction)** | Random Forest · Z-Score Drift · Streamlit | [🟢 Live](https://breast-cancer-predict1.streamlit.app/) | 98.2% acc · Real-time out-of-distribution detection |
| **[Respiratory Disease Classifier](https://github.com/Khanz9664/Transfer-Learning-for-Respiratory-Disease-Classification)** | VGG16 · ViT-B/16 · GradCAM++ · LIME | Research | 99% recall for COVID-19 · Explainability Paradox discovery |
| **[Apple Sales Intelligence](https://github.com/Khanz9664/Comprehensive-Data-Analysis-Visualization-of-Apple-Product-Sales)** | Scikit-Learn · SciPy SLSQP · Streamlit | [🟢 Live](https://applesalesanalytics.streamlit.app/) | Constrained optimization for hardware-mix revenue maximization |
| **[Patient Safety Guardian](https://github.com/Khanz9664/The-Patient-Guardian-)** | Gemini 2.5 Pro · Google ADK · Streamlit | [🟢 Live](https://the-patient-guardian-git-jahk4i2rnm93uwceqnk7qu.streamlit.app/) | Kaggle Agents Intensive · Multi-agent clinical safety net · 100% critical interaction detection |

---

<!-- ─── MATHEMATICAL FOUNDATIONS ───────────────────────────────────────── -->
 
## Mathematical Foundations of ML
 
I write derivation-first articles — intuition before formulas, complete proofs included. No hand-waving, no shortcuts.
</br>
<!-- ── Article 1 — Gradient Descent ── -->
<h3><a href="https://khanz9664.github.io/portfolio/articles/gradient-descent.html">Gradient Descent</a></h3>
<a href="https://khanz9664.github.io/portfolio/articles/gradient-descent.html">
  <img align="left" width="200" alt="Gradient Descent" src="https://raw.githubusercontent.com/Khanz9664/Khanz9664/main/assets/1.png"/>
</a>
<blockquote><em>The workhorse of machine learning optimization.</em></blockquote>
<p>A rigorous, ground-up treatment of how gradient descent navigates the loss landscape. Covers the derivation of partial derivatives and the chain rule in the context of multi-parameter loss functions, the geometry of steepest descent, and why learning rate choice is not arbitrary — too large diverges, too small stalls. Analyses convergence behavior, introduces momentum variants, and connects the mathematics to practical PyTorch training loops. Written for readers who want to truly understand <strong>why</strong> the optimizer works, not just how to call <code>.backward()</code>.</p>
<a href="https://khanz9664.github.io/portfolio/articles/gradient-descent.html"><strong>Read Article →</strong></a>
<br clear="left"/><hr/>
<!-- ── Article 2 — Lagrange Multipliers ── -->
<h3><a href="https://khanz9664.github.io/portfolio/articles/lagrange-multipliers.html">Lagrange Multipliers</a></h3>
<a href="https://khanz9664.github.io/portfolio/articles/lagrange-multipliers.html">
  <img align="left" width="200" alt="Lagrange Multipliers" src="https://raw.githubusercontent.com/Khanz9664/Khanz9664/main/assets/2.png"/>
</a>
<blockquote><em>Constrained optimization — the math behind SVMs, regularization, and resource allocation.</em></blockquote>
<p>When you can't just follow the gradient because the solution must satisfy a constraint, Lagrange multipliers are the tool. This article builds the method from its geometric foundations — explaining why the gradient of the objective must be parallel to the gradient of the constraint at a solution — and derives the KKT conditions used throughout modern ML. Covers the primal and dual problem formulation, the role of the Lagrangian, saddle-point interpretation, and worked examples in both geometric and analytical form. Directly applicable to understanding <strong>Support Vector Machine margins</strong> and constrained portfolio optimization.</p>
<a href="https://khanz9664.github.io/portfolio/articles/lagrange-multipliers.html"><strong>Read Article →</strong></a>
<br clear="left"/><hr/>
<!-- ── Article 5 — Logistic Regression ── -->
<h3><a href="https://khanz9664.github.io/portfolio/articles/logistic-regression.html">Logistic Regression</a></h3>
<a href="https://khanz9664.github.io/portfolio/articles/logistic-regression.html">
  <img align="left" width="200" alt="Logistic Regression" src="https://raw.githubusercontent.com/Khanz9664/Khanz9664/main/assets/5.png"/>
</a>
<blockquote><em>From continuous predictions to calibrated class probabilities — the complete derivation.</em></blockquote>
<p>Walks through the motivation for squashing linear outputs through the sigmoid function, deriving its form from the odds-ratio and log-odds perspective. Constructs the Binary Cross-Entropy loss function from scratch using Maximum Likelihood Estimation over the Bernoulli distribution, then derives its gradient with respect to model weights — revealing the elegant result that the gradient takes the same form as linear regression's residual. Covers numerical stability considerations (log-sum-exp trick), the probabilistic interpretation of outputs, and why logistic regression is not just a classifier but a <strong>calibrated probabilistic model</strong>.</p>
<a href="https://khanz9664.github.io/portfolio/articles/logistic-regression.html"><strong>Read Article →</strong></a>
<br clear="left"/><hr/>
<!-- ── Article 6 — Neural Networks ── -->
<h3><a href="https://khanz9664.github.io/portfolio/articles/neuralnets.html">Neural Networks</a></h3>
<a href="https://khanz9664.github.io/portfolio/articles/neuralnets.html">
  <img align="left" width="200" alt="Neural Networks" src="https://raw.githubusercontent.com/Khanz9664/Khanz9664/main/assets/6.png"/>
</a>
<blockquote><em>Where calculus, linear algebra, and biology collide to build machines that learn.</em></blockquote>
<p>Constructs a neural network from absolute zero — starting with the biological neuron analogy, then formalizing the mathematical model as a composition of affine transformations and nonlinear activations. Derives the backpropagation algorithm in full using the chain rule across the computation graph, showing exactly how gradients flow from the loss back through every weight in the network. Covers the vanishing gradient problem, why activation function choice (ReLU vs. sigmoid vs. tanh) is not cosmetic, and how depth creates <strong>hierarchical feature representations</strong> that shallow models fundamentally cannot. By the end, you will have built and trained a network from scratch in NumPy — no framework magic, no black boxes.</p>
<a href="https://khanz9664.github.io/portfolio/articles/neuralnets.html"><strong>Read Article →</strong></a>
<br clear="left"/>
<br/>

<h1 align="center">→ <a href="https://khanz9664.github.io/portfolio/articles.html"><strong>Explore All Articles →</strong></a></h1>

---

<!-- ─── SKILLS SNAPSHOT ────────────────────────────────────────────────── -->

## Technical Stack

```
ML / DL          PyTorch · XGBoost · Scikit-Learn · VGG16 · ViT · Optuna
XAI              SHAP · LIME · GradCAM++ · EigenCAM · Pixel Deletion (AOPC/AUC)
MLOps            FastAPI · Docker · GitHub Actions CI/CD · Streamlit · REST APIs
Data Engineering Python · SQL · Pandas · NumPy · PCA · K-Means · Plotly
Drift Detection  Z-Score · Counterfactual Analysis · Synthetic Stress Testing
```

---

## GitHub Activity

<div align="center">

<table>
<tr>
<td align="center">
<img width="380" src="https://github-readme-streak-stats.herokuapp.com?user=Khanz9664&theme=radical" />
</td>

<td align="center">
<img width="400" src="http://github-profile-summary-cards.vercel.app/api/cards/profile-details?username=Khanz9664&theme=github_dark"/>
</td>
</tr>
</table>
<table>
<tr>
<td align="center">
<img width="250" src="http://github-profile-summary-cards.vercel.app/api/cards/most-commit-language?username=Khanz9664&theme=dracula"/>
</td>
<td align="center">
<img width="250" src="http://github-profile-summary-cards.vercel.app/api/cards/productive-time?username=Khanz9664&theme=2077&utcOffset=8" alt="Commits per day badge"/>
</td>
<td align="center">
<img width="250" src="https://github-readme-activity-graph.vercel.app/graph?username=Khanz9664&theme=merko&hide_border=true"/>
</td>
</tr>

</table>

</div>

---

<!-- ─── QUOTE ──────────────────────────────────────────────────────────── -->

<div align="center">

*"In God we trust. All others must bring data."* — W. Edwards Deming

<br/>

**If your model can't explain itself, it has no business making decisions.**

</div>
