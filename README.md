# student-cme-ust-calendar-calculator

A simple student project for estimating the theoretical fair value of CME U.S. Treasury futures calendar spreads using a carry-based pricing model.

This spreadsheet was built as an educational tool for understanding how Treasury futures calendar spreads can be influenced by financing costs and bond yield carry.

The goal is not to predict markets or build a professional trading system.

The goal is to make the structure behind Treasury futures calendars easier to visualize and understand.

---

# Core Idea

Treasury futures calendar spreads can be viewed as a carry relationship.

Holding Treasury exposure through time has:
- a financing cost (repo / SOFR)
- but also a yield benefit from the underlying bond

This project models that simplified net carry relationship.

---

# Formula

The spreadsheet uses a simplified continuous compounding model:

F₂ = F₁ × e^((r - y) × t)

Where:

- F₁ = front futures contract price
- r = repo / financing rate
- y = CTD yield assumption
- t = time between expiries in years
- F₂ = implied next contract futures price

The fair value calendar spread is then:

Calendar Spread = F₂ - F₁

---

# Inputs

- Front Futures Price
- Repo / Financing Rate
- CTD Yield
- Days Between Contracts
- Day Count Basis
- Tick Size

---

# Outputs

- Implied Next Contract Futures Price
- Fair Value Calendar Spread
- Spread in Ticks
- Time Fraction
- Net Carry Rate
- Carry Factor

---

# What This Project Is

This is:
- a student educational project
- a simplified carry model
- a way to build intuition around Treasury futures calendars
- a lightweight fixed income learning tool

---

# What This Project Is Not

This spreadsheet does NOT model:
- real-world CTD switching
- delivery optionality
- repo specials
- liquidity stress
- volatility premia
- balance sheet constraints
- convexity effects
- professional dealer pricing systems

It is intentionally simplified for learning purposes.

---

# Educational Goal

The broader goal of this project is to make complex fixed income and derivatives concepts easier to understand visually and structurally.

This project continues earlier student work involving:
- Treasury futures hedge ratios
- DV01 concepts
- CTD and net basis relationships
- Treasury butterflies
- futures carry intuition

---

# Notes

Built using native Excel formulas with a simple and minimal spreadsheet layout.

No VBA, macros, or advanced automation were used.
