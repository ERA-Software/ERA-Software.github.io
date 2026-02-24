# Software catalog

A curated set of ERA-Software tools for uncertainty quantification, reliability analysis, Bayesian inference, and surrogate modeling.

<div class="grid cards" markdown>

-   :material-chart-bell-curve: **eraUQ**
    
    Base library for uncertainty quantification and reliability workflows: probability distributions (e.g., `ERADist`, `EmpDist`), dependence models (e.g., Nataf/Gaussian copula), and related utilities.  
    [:octicons-mark-github-16: Repo](https://github.com/ERA-Software/eraUQ) ·
    [:material-package-variant: PyPI](https://pypi.org/project/eraUQ/) ·
    [:material-notebook: Notebook](https://github.com/ERA-Software/eraUQ#example-notebook)

-   :material-shield-check: **Reliability analysis tools (Python)**
    
    Methods for reliability analysis and rare-event probability estimation. Includes classic workhorses such as **FORM**, **Cross-Entropy / iCE**, **Subset Simulation**, **Sequential Importance Sampling**, and **Line Sampling variants**.  
    [:octicons-mark-github-16: Listed in Overview](https://github.com/ERA-Software/Overview)

-   :material-chart-scatter-plot: **Bayesian inference tools (Python)**
    
    Sampling-based Bayesian inference methods, including **BUS** (Bayesian Updating with Structural reliability methods), **Adaptive BUS**, **iTMCMC**, and **SMC-style** algorithms.  
    [:octicons-mark-github-16: Listed in Overview](https://github.com/ERA-Software/Overview)

-   :material-function-variant: **Surrogate modelling (Python)**
    
    Surrogate modelling tools for UQ, including **Partial-Least-Squares-based Polynomial Chaos Expansion (PLS-PCE)** (as listed in your org overview).  
    [:octicons-mark-github-16: Listed in Overview](https://github.com/ERA-Software/Overview)

</div>

---

## How these pieces fit together

A typical workflow looks like:

1. **Define uncertainty** (marginals + dependence) with `eraUQ`
2. **Approximate expensive models** with surrogate modelling (optional but often essential)
3. **Estimate failure probability** with reliability tools
4. **Update with data** using Bayesian inference tools (e.g., BUS / iTMCMC)
5. **Use results for decisions** (risk, inspection, design, etc.)