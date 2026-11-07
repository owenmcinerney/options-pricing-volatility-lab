# Phase 1 Readings — Options Fundamentals and Black–Scholes

This is the reading log for Phase 1 of **Neural Network-Based Options Pricing and Stochastic Volatility Calibration**. The handoff package supplies the project roadmap and learning preferences; this page turns the Phase 1 topics into a guided reading sequence. Notes under “My notes” are intentionally blank for Owen to fill in during the project.

## Reading path

### 1. Option contract basics

**Read:** [Options Basics — Options Industry Council](https://www.optionseducation.org/optionsoverview/options-basics)

**Summary:** Introduces calls and puts, contract terms, strike price, expiration, exercise, and option premium. Use it to build a clear picture of what the contract gives its holder before studying a pricing formula.

**Focus:** Call vs. put; buyer vs. seller; strike; expiration; exercise; premium; payoff vs. profit.

**My notes**

- In my own words, a call gives its holder the right to:
- In my own words, a put gives its holder the right to:
- One distinction between payoff and profit:
- Questions / examples I want to revisit:

### 2. Expiration payoff and moneyness

**Read:** [An Introduction to Options — Investor.gov](https://www.investor.gov/introduction-investing/general-resources/news-alerts/alerts-bulletins/investor-bulletins-63)

**Summary:** A regulator-authored overview of basic option transactions and the risks and terminology investors encounter. Pair it with the OIC basics page and sketch expiration payoffs for a long call and long put.

**Focus:** Intrinsic value at expiration, in-the-money / at-the-money / out-of-the-money, and why the option premium is not the same as expiration payoff.

**My notes**

- For a call with strike $K$, the expiration payoff is:
- For a put with strike $K$, the expiration payoff is:
- Example values of stock price and strike that make a call in the money:
- Questions / examples I want to revisit:

### 3. European vs. American exercise

**Read:** [Options Basics — Options Industry Council](https://www.optionseducation.org/optionsoverview/options-basics) (contract type and exercise sections)

**Summary:** Review the exercise terms: European-style options can be exercised only at expiration, while American-style options can be exercised before or at expiration. This distinction matters because the introductory Black–Scholes formula in our starter notebook prices European options.

**My notes**

- The exercise right that differs between European and American options:
- Why the starter example uses a European option:
- Questions / examples I want to revisit:

### 4. What moves an option price?

**Read:** [Options Pricing — Options Industry Council](https://www.optionseducation.org/optionsoverview/options-pricing)

**Summary:** Reviews the main pricing inputs and how they affect option premiums, including underlying price, strike, time, volatility, interest rates, and dividends. Keep this as an intuition-first companion to the starter notebook’s inputs ($S=100$, $K=100$, 30 days, 20% volatility, 5% rate, 0% dividend yield).

**My notes**

| Input | My intuition for how it affects a call / put |
|---|---|
| Underlying price ($S$) | |
| Strike ($K$) | |
| Time to expiration ($T$) | |
| Volatility ($\\sigma$) | |
| Risk-free rate ($r$) | |
| Dividend yield ($q$) | |

### 5. Greeks as sensitivities

**Read:** [Understanding Options Greeks — Options Industry Council](https://www.optionseducation.org/advancedconcepts/understanding-options-greeks)

**Summary:** Introduces the Greeks as estimates of how an option’s theoretical value responds to changes in market inputs. Start with delta, gamma, theta, vega, and rho; treat them as local sensitivities, not exact predictions.

**My notes**

- Delta measures:
- Gamma measures:
- Theta measures:
- Vega measures:
- Rho measures:
- Which Greek feels least intuitive, and why?

### 6. Black–Scholes context (optional reference for Phase 1)

**Read:** [Black–Scholes model — ICAEW](https://devmaster.icaew.com/library/research-guides/black-scholes)

**Summary:** Gives context for the Black–Scholes model and its use for theoretical European option prices. For this first pass, focus on what the model is used for and its European-option setting; we will unpack the formula and assumptions alongside the notebook rather than require a full derivation first.

**My notes**

- What does the model output?
- One assumption or limitation I noticed:
- What I want explained when we work through the calculator:

## Session notes and progress

| Date | Reading(s) completed | Key takeaway in my words | Open question |
|---|---|---|---|
| | | | |

## How we will reference readings

When we discuss a Phase 1 concept or change the starter notebook, we will point to the relevant reading by its number above. Add your own notes here; later phases can link back to the same sources when concepts such as volatility, risk-neutral pricing, or calibration reappear.

