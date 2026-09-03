# William Caron-Bastarache — Portfolio Website

Personal portfolio website hosted via GitHub Pages.

🌐 Live site: https://will13cb.github.io

---

## Overview

This repository contains the source code for my personal portfolio website.

It presents:
- Selected software projects
- Quantitative research work
- Academic background (B.Sc. Computer Science, Université de Montréal)
- Technical skills
- Professional experience

The website is built using static HTML/CSS and deployed through GitHub Pages.

---

## Featured Projects

### Event-Driven Market Probability Engine (Phases A–D complete)

A layered PostgreSQL warehouse and a walk-forward-validated probability model, built to test honestly
whether next-day ETF moves are predictable. Measured answer: no tradeable edge.

Stack:
- PostgreSQL
- Python (asyncio, pandas, psycopg, scikit-learn, matplotlib)
- SQL window functions
- Make, pytest

Focus:
- Point-in-time correctness enforced by database-level assertions
- Walk-forward validation with a purge/embargo
- Backtesting against a hold-the-market benchmark
- Reporting a negative result rather than burying it

---

### Financial Event Extraction (Design phase)

An agent system that turns financial documents into structured, timestamped events, built around an
evaluation harness rather than around the agent framework. SEC XBRL gives every extracted number an
authoritative value to score against, which turns "the agent seems to work" into a measurement.

Planned stack:
- Python, PostgreSQL
- EDGAR API, XBRL
- LangGraph (stage 6, wrapping work that is already validated)

Focus:
- Ground truth before subjective judgement
- Extraction accuracy measured against a regex baseline, with failure categories
- Point-in-time discipline on documents (publication timestamp, initial print)
- Feeds the event layer of the Event-Driven Market Probability Engine

---

### MaVille — Java CLI Application

Municipal management simulation system built with:
- Java
- Maven
- REST integration
- JUnit testing

---

### Software Quality & CI Projects (GraphHopper)

- Unit testing & mutation testing (JaCoCo, PIT)
- GitHub Actions CI quality gate
- Mutation score regression control

---

## Tech Stack (Website)

- HTML5
- CSS3
- Vanilla JavaScript
- Google Fonts
- GitHub Pages (static hosting)

---

## Deployment

The site is automatically deployed via GitHub Pages from the `main` branch.


---

## Contact

Email: will13cb@gmail.com  
LinkedIn: https://www.linkedin.com/in/william-caron-bastarache  
GitHub: https://github.com/will13cb  

---

© 2026 William Caron-Bastarache
