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
  <img align="right" width="380" src="https://github-readme-stats.vercel.app/api/pin/?username=Khanz9664&repo=TrustLens&theme=tokyonight&hide_border=true&bg_color=0D1117&title_color=00F7F4&text_color=ffffff&icon_color=FF6E4A" />
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
<!--
### Open-Source Contribution: Roboflow `supervision`

**PR [#2247](https://github.com/roboflow/supervision/pull/2247) — Add OBB support to `ConfusionMatrix` via `MetricTarget`** *(under review)*

`ConfusionMatrix` was silently computing IoU on axis-aligned bounding boxes even when users passed oriented (rotated) detections. This PR fixes that by routing through `oriented_box_iou_batch` when `MetricTarget.ORIENTED_BOUNDING_BOXES` is selected — aligning `ConfusionMatrix` with every other metric in the library. 118 tests passing, full backward compatibility preserved.

---
-->

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

I write derivation-first articles — intuition before formulas, full proofs included. No hand-waving.

| Article | What It Covers |
|---------|---------------|
| [**Gradient Descent**](https://khanz9664.github.io/portfolio/articles/gradient-descent.html) | Partial derivatives · learning rates · convergence from first principles |
| [**Lagrange Multipliers**](https://khanz9664.github.io/portfolio/articles/lagrange-multipliers.html) | Constrained optimization · dual problems · geometric intuition |
| [**Bias–Variance Trade-Off**](https://khanz9664.github.io/portfolio/articles/biasvariance.html) | The fundamental tension between model simplicity and prediction accuracy |
| [**Linear Regression**](https://khanz9664.github.io/portfolio/articles/linear-regression.html) | OLS derivation · normal equations · assumption breakdown |
| [**Logistic Regression**](https://khanz9664.github.io/portfolio/articles/logistic-regression.html) | Sigmoid · MLE · cross-entropy loss gradient derivation |

→ [All articles →](https://khanz9664.github.io/portfolio/articles.html)

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

<!-- ─── GITHUB STATS ────────────────────────────────────────────────────── -->

## GitHub Activity

<div align="center">

<table><tr>
  <td><img src="https://github-readme-streak-stats.herokuapp.com?user=Khanz9664&theme=tokyonight&hide_border=true&border_radius=4&short_numbers=true&hide_total_contributions=true" alt="GitHub Streak" /></td>
  <td><img src="https://awesome-github-stats.azurewebsites.net/user-stats/Khanz9664?cardType=level&preferLogin=false&theme=tokyonight" /></td>
</tr></table>

<img src="https://github-readme-activity-graph.vercel.app/graph?username=Khanz9664&theme=tokyo-night&hide_border=true&bg_color=0D1117&color=00F7F4&line=00F7F4&point=FFFFFF" alt="Contribution Graph" />

![Trophies](https://github-profile-trophy.vercel.app/?username=Khanz9664&theme=tokyonight&no-frame=true&no-bg=true&margin-w=6)

</div>

---

<!-- ─── QUOTE ──────────────────────────────────────────────────────────── -->

<div align="center">

*"In God we trust. All others must bring data."* — W. Edwards Deming

<br/>

**If your model can't explain itself, it has no business making decisions.**

</div>
