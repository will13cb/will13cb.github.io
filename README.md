# William Caron-Bastarache, Portfolio Website

Personal portfolio website, bilingual (English and French), hosted on GitHub Pages.

🌐 **Live site: https://williamcaronbastarache.com**

---

## Overview

Source for my personal portfolio. It presents:

- Selected software and systems projects
- Quantitative research work
- Academic background (B.Sc. Computer Science, Université de Montréal, 2024 to 2027 expected)
- Technical skills and professional experience

Static HTML and CSS with a small amount of vanilla JavaScript, deployed from the `main` branch.
Every page exists in English and French, paired with `hreflang` so search engines serve the right
language.

---

## Featured projects

### Event-Driven Market Probability Engine (Phases A to D complete)

A layered PostgreSQL warehouse and a walk-forward-validated probability model, built to test
honestly whether next-day ETF moves are predictable. Measured answer: no tradeable edge. 15 ETFs,
32,295 rows, 36 tests.

**Stack:** PostgreSQL, Python (asyncio, pandas, psycopg, scikit-learn, matplotlib), SQL window
functions, Make, pytest

**Focus:**
- Point-in-time correctness enforced by database-level assertions
- Walk-forward validation with a purge and embargo
- Backtesting against a hold-the-market benchmark
- Reporting a negative result rather than burying it

---

### Multi-Source Financial Intelligence (planning)

A planned agentic pipeline that reads official documents alongside the informal commentary around
them, produces a research report and a daily point-in-time feature panel, feeds the probability
engine above, and is judged by a pre-registered backtest before it runs live.

**Planned stack:** Dagster, LangGraph, PostgreSQL with pgvector, Claude and open models behind one
interface

**Focus:**
- Architecture and build order fixed before any implementation
- Evaluation defined up front, so the result can come back negative
- Point-in-time discipline on documents (publication timestamp, initial print)

---

### Building Operating System Components in C (IFT 2245)

Five systems written from scratch in C: a Unix shell, a scheduler on two simulated cores, a virtual
memory manager with a TLB and demand paging, a FAT32 reader working on raw disk bytes, and a Turing
machine interpreter.

**Stack:** C, CMake, pthreads, bison and flex, Check, Valgrind, gdb, Docker, GitHub Actions

**Graded on:** hidden tests, performance against baselines, Valgrind cleanliness

Coursework for IFT 2245, Operating Systems, Université de Montréal. Assignment repositories are not
published.

---

### Implementing and Benchmarking Classic Algorithms (IFT 2125)

Stable matching, greedy against dynamic programming, and the closest pair of points. Each
implemented, then benchmarked against the alternatives on the same inputs rather than trusting the
complexity class on paper. Two of the three results contradicted the intuition.

**Stack:** Python, NumPy, Matplotlib

**Verified by:** known optimal solutions, checked within a tolerance

Coursework for IFT 2125, Introduction to Algorithms, Université de Montréal. The assignment
repository is private.

---

### MaVille, Java CLI application

Municipal management simulation: resident and contractor profiles, notifications, data persistence,
and integration with a public REST API.

**Stack:** Java, Maven, Javalin (REST), JUnit

---

### Software quality and CI (GraphHopper, IFT 3913)

- AutoParams (JUnit 5) presentation and live demo
- Unit testing and mutation testing with JaCoCo and PIT
- GitHub Actions CI quality gate with mutation-score regression control

---

## Repository layout

```
index.html / index-fr.html     landing pages, English and French
404.html                       custom not-found page
projects/en/ , projects/fr/    one page per project, paired across languages
styles.css                     single stylesheet for the whole site
img/                           diagrams (SVG), screenshots, tile thumbnails (WebP)
cv/                            CV, English and French (PDF)
sitemap.xml , robots.txt       crawl directives
CNAME                          custom domain
```

---

## Tech stack (website)

- HTML5, CSS3, vanilla JavaScript
- Inline SVG for all diagrams and charts
- Google Fonts (Inter, Source Serif 4)
- GitHub Pages (static hosting), custom domain over HTTPS

**Search and sharing:** per-page titles, meta descriptions and canonical URLs; reciprocal
`hreflang` across the English and French trees; Open Graph and Twitter card tags; Person structured
data (JSON-LD) on both landing pages; `sitemap.xml` and `robots.txt`.

---

## Deployment

Deployed automatically by GitHub Pages from the `main` branch. `will13cb.github.io` redirects to
the custom domain.

---

## Contact

- Email: will13cb@gmail.com
- LinkedIn: https://www.linkedin.com/in/william-caron-bastarache
- GitHub: https://github.com/will13cb

---

© 2026 William Caron-Bastarache
