# Finance Project — Consolidated Handoff

## Purpose
A progressive project to learn and research neural-network-based options pricing and stochastic-volatility calibration.

## Project overview

- Working title: Neural Network-Based Options Pricing and Stochastic Volatility Calibration.
- Research question: Can neural networks approximate option prices and calibrate stochastic-volatility models more efficiently than traditional numerical methods while maintaining comparable accuracy?
- Approach: Build from the simplest financial concepts toward advanced numerical simulation, machine learning, deep learning, inverse calibration, and real-market validation. The user is relatively new to this specific topic and wants a guided, incremental learning path.

## User background relevant to this project

- B.S. in Computational Data Science from Penn State, with a minor in Mathematics.
- Completed coursework in Math for Finance. This provides relevant prior exposure to financial mathematics, but the exact topics covered in that course have not yet been specified.
- Has previously implemented a Monte Carlo option-pricing and stochastic-volatility project using Black-Scholes and Heston models, simulating 10,000 stock paths and reporting an absolute pricing error of 0.0043.
- Programming and quantitative background includes Python, SQL, R, statistical analysis, machine learning, optimization, and data science.
- Wants to develop deeper expertise in quantitative finance, derivatives, financial modeling, and machine learning applications in finance.

## Learning and collaboration preferences

- Start with foundational concepts and build complexity gradually; do not assume advanced options-pricing or stochastic-calculus knowledge.
- Teach the theory and intuition before introducing complex equations or code.
- Explain mathematical notation and financial terminology rather than skipping steps.
- Implement models incrementally in Python/Jupyter, explaining what each section of code does.
- Use experiments, visualizations, interpretation questions, and small coding exercises to reinforce understanding.
- Do not simply provide finished code. Guide the user through the reasoning and implementation.
- Keep a clear phase tracker and revisit the project plan when resuming.

## Project roadmap

- Phase 1 — Options fundamentals and Black-Scholes calculator: calls, puts, strikes, expiration, volatility, rates, Greeks, payoff versus profit, European versus American options.
- Phase 2 — Monte Carlo simulation: geometric Brownian motion, simulated stock paths, discounted payoffs, convergence, and standard error.
- Phase 3 — Heston stochastic volatility: Brownian motion, variance process, mean reversion, correlation, and simulation.
- Phase 4 — Synthetic dataset generation: create and validate option-price observations across strikes, maturities, rates, and Heston parameters.
- Phase 5 — Machine-learning benchmarks: linear regression, random forest, and gradient boosting compared with Heston benchmark prices.
- Phase 6 — Deep-learning pricing model: feedforward neural network in PyTorch to approximate Heston prices.
- Phase 7 — Inverse calibration and financial constraints: estimate Heston parameters from option prices or implied-volatility surfaces; compare with numerical optimization and test financial consistency.
- Phase 8 — Real-market validation and final application: evaluate on real options data if available, build visualizations/dashboard, and write a research report.

## Proposed mathematical models

- Black-Scholes is the initial analytical benchmark for European options.
- Heston is the primary stochastic-volatility model, with parameters v0 (initial variance), kappa (mean-reversion speed), theta (long-run variance), sigma_v (volatility of variance), and rho (correlation).
- Monte Carlo simulation provides a numerical benchmark and a way to generate synthetic training data.
- Two neural networks are planned: (1) a pricing surrogate mapping contract and model inputs to option prices; (2) an inverse calibration model mapping option prices or volatility surfaces to Heston parameters.

## Evaluation and research standards

- Compare pricing accuracy using MAE and RMSE.
- Compare calibration using parameter recovery error and calibration runtime.
- Test out-of-sample generalization across strikes, maturities, and parameter ranges.
- Check financial consistency, including put-call parity, appropriate price bounds, and monotonicity with respect to strike and underlying price.
- Avoid data leakage; keep training, validation, and test sets separate.
- Validate synthetic benchmark prices against an independent implementation on a sample.
- Treat synthetic-data performance and real-market performance as separate claims.
- Do not equate pricing accuracy with trading profitability.

## Technology stack

- Initial: Python, Jupyter Notebook, NumPy, SciPy, Pandas, Matplotlib.
- Later: scikit-learn, XGBoost, PyTorch, Plotly, Streamlit, MLflow.
- Optional later validation: QuantLib-Python.
- Do not require advanced packages or setup before the relevant phase.

## Research papers already identified

- Black, F. and Scholes, M. (1973), The Pricing of Options and Corporate Liabilities. DOI: https://doi.org/10.1086/260062
- Heston, S. L. (1993), A Closed-Form Solution for Options with Stochastic Volatility with Applications to Bond and Currency Options. DOI: https://doi.org/10.1093/rfs/6.2.327
- Liu, S., Oosterlee, C. W., and Bohte, S. M. (2019), Pricing Options and Computing Implied Volatilities using Neural Networks. https://www.mdpi.com/2227-9091/7/1/16
- Deep Learning Volatility: A Deep Neural Network Perspective on Pricing and Calibration in (Rough) Volatility Models (2021). DOI: https://doi.org/10.1080/14697688.2020.1817974
- Van Mieghem, L., Papapantoleon, A., and Papazoglou-Hennig, J. (2023), Machine Learning for Option Pricing: An Empirical Investigation of Network Architectures. https://arxiv.org/abs/2307.07657
- Calibrating FBSDEs Driven Models in Finance via NNs (2022). https://www.mdpi.com/2227-9091/10/12/227
- Kim, Y. S., Kim, H., and Choi, J. (2023), Deep Calibration With Artificial Neural Network: A Performance Comparison on Option Pricing Models. https://arxiv.org/abs/2303.08760
- Improved Accuracy of an Analytical Approximation for Option Pricing under Stochastic Volatility Models Using Deep Learning Techniques (2025). DOI: https://doi.org/10.1016/j.camwa.2025.03.029
- A Comparative Analysis of Option Pricing Models: Black–Scholes, Bachelier, and Artificial Neural Networks (2025). DOI: https://doi.org/10.1057/s41283-025-00160-0

## Current status and next action

- Project roadmap has been drafted.
- A Word project plan and a Phase 1 Jupyter notebook have been created and should be retained with this handoff.
- The Phase 1 notebook starts with an illustrative European option: S = 100, K = 100, 30 days to expiration, annualized volatility = 20%, risk-free rate = 5%, and dividend yield = 0%.
- Next action: begin Phase 1 by explaining option contract mechanics and each Black-Scholes input, then work through the notebook cell by cell. Do not jump ahead to Heston or neural networks until the user is comfortable with the foundations.

## Included files

- `Options_Pricing_Deep_Learning_Project_Plan.docx`
- `Options_Pricing_Phase_1_Starter.ipynb`

