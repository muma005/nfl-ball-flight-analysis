# NFL Ball Flight Analysis

Project skeleton for analyzing ball flight and catch metrics (separation gain, closing speed, contested catch index, RSI).

This repository contains data folders, notebooks, reusable code in `src/`, and reports/visuals placeholders.


https://github.com/user-attachments/assets/5a6fc49b-3175-4ad7-8fca-7837cd34c702




Absolutely — here is the **full write-up outline**, crafted in the style and structure of previous winners, but tailored perfectly to *your three-metric system* (SG, TTI, RSI).
This is NOT filler — this is a polished, competition-grade blueprint that judges genuinely expect.

After the outline, I can expand each section into full prose.

---

# 🏈 **BIG DATA BOWL WRITE-UP (FULL STRUCTURED OUTLINE)**

### *Title: Uncovering the Hidden Movement Dynamics of Downfield Pass Plays*

---

# **I. Introduction — The Hidden Battle During Ball Flight**

**Purpose of this section:** Show judges that you *understand football first*, data second.

### Key points to include:

* Traditional pass-play evaluation (open, contested, incomplete, caught) describes the *outcome* but not the *process*.
* The ball flight phase — from throw to catch — is the most ambiguous and least measured moment in football.
* WRs and DBs are engaged in a **micro-battle of movement:**

  * WR attempts to *create space*
  * DB attempts to *close space*
  * Both attempt to *read and react to the ball*
* Existing metrics do not quantify how movement advantages are created or lost.
* **Motivation:** Coaches want to understand *why* a WR got open or a DB stayed in phase — not just whether it happened.

### Your thesis line:

> We introduce three movement-based metrics — **Separation Gain (SG)**, **Time-to-Intervention (TTI)**, and **Reactive Synchronization Index (RSI)** — that quantify the WR–DB interaction during ball flight. Together, they reveal how space is generated, how defenders close it, and how movement deception influences coverage outcomes.

---

# **II. A Unified Visualization of Pass Interaction**

(*This is your Figure 1 Analog — the critical diagram every winning paper has*)

You show ONE simple illustration containing:

* **SG curve (space over time)**
* **TTI marker (estimated defender arrival time)**
* **RSI band/curve (movement synchrony)**

This becomes the reader’s mental map for the entire paper.

### What to include:

* A side-by-side static diagram or composite visual:

  * WR–DB movement animation frame
  * SG curve
  * TTI vertical line
  * RSI synchrony bar under the curve
* Just 3–4 labels:

  * “WR creates space here”
  * “DB closes here”
  * “Movement out of sync here”

This visual should be **extremely simple** and used to explain the concepts before you show real plays.

---

# **III. Metric 1 — Separation Gain (SG): The Space Story**

### Purpose:

Explain how WR *wins leverage* through movement.

### What SG measures:

* Change in separation from throw → catch.
* Whether WR created space *because of movement advantage* rather than coverage breakdown.

### Why coaches care:

* SG reveals technique wins (hip drop, rocker step, tempo variation)
* Helps differentiate WRs who separate early vs. late in the route
* Identifies DBs who prevent space creation even on deep throws

### Include:

* **Simple SG visualization:**

  * Animation on left
  * Separation curve on right
  * Highlight SG arrow at end

* **1 Play Example:**

  * Play GIF
  * SG curve
  * 2–3 sentence football interpretation
    (“WR stems inside, DB hesitates, SG increases from 1.2 → 3.8 yds.”)

---

# **IV. Metric 2 — Time-to-Intervention (TTI): The Pursuit Story**

### Purpose:

Explain the defender’s ability to *recover* or *contest* the catch.

### What TTI measures:

* How quickly the DB could reach the WR’s catch location
* Incorporates DB closing speed and angle
* Predicts whether a catch window will be contested

### Why coaches care:

* Helps evaluate DB closing discipline
* Shows when DBs take inefficient angles
* Identifies late-recognition moments in coverage

### Include:

* **TTI Visualization:**

  * Animated WR–DB play
  * Vertical line at TTI on distance/time graph
  * “Catch window bar” showing contest probability

* **1 Play Example:**

  * GIF
  * TTI graph
  * Football explanation
    (“Despite early separation, DB accelerates from 6.1 yds to within reach in 0.73s — tight contest.”)

---

# **V. Metric 3 — Reactive Synchronization Index (RSI): The Dance Story**

### Purpose:

Explain *how well DB mirrors WR movement* during ball flight.

### What RSI measures:

* Whether WR & DB adjust direction at the same time
* Whether the defender matches the WR’s break magnitude
* Whether their movement is in-phase or out-of-phase

### Why coaches care:

* High RSI = sticky coverage
* Low RSI = WR movement deception → DB loses sync
* Helps identify elite route runners and elite mirror corners

### Include:

* **RSI GIF Visualization:**

  * Left: animated play
  * Right: scrolling synchrony bar that fills with red→yellow→green
  * Cursor moves along timeline with animation

* **1 Play Example:**

  * GIF
  * Synchrony bar
  * Football explanation
    (“WR breaks inside at 0.48s, DB reacts 0.23s later — RSI drops to 0.34.”)

---

# **VI. Case Studies — Putting All Metrics Together**

Show 2 complete plays where:

### A. WR Wins

* SG ↑
* RSI ↓
* TTI high
  → WR wins leverage + movement battle → separation

### B. DB Wins

* SG stable or ↓
* RSI ↑
* TTI low
  → DB stays glued + contests effectively

These two plays will be among your strongest visuals.

---

# **VII. League-Wide Insights (Your Competitive Advantage)**

This section proves your metrics are not just illustrative — they scale.

### Ideas:

#### **1. WR archetypes**

* Movement separators (RSI ↓, SG ↑)
* Speed separators (TTI ↑)
* Early separators vs. late separators

#### **2. DB archetypes**

* Sticky mirrors (RSI ↑)
* Fast closers (TTI ↓)
* Space-deniers (SG suppression)

#### **3. Route families**

* Which routes generate biggest SG?
* Which routes cause biggest RSI drops?
* Which coverages produce best TTI outcomes?

This shows serious football intelligence.

---

# **VIII. Practical Coaching Applications (Football Score Section)**

Explain exactly how coaches could use this weekly.

### Examples:

* WR coaching: drills for manipulating defender synchrony
* DB coaching: recognition cues to reduce TTI
* OC/DC strategy: choose routes that stress out DBs with low RSI tendencies
* Scouting: identify WRs who generate late separation vs early separation

---

# **IX. Conclusion**

Summarize:

* SG → tells the **space story**
* TTI → tells the **pursuit story**
* RSI → tells the **movement deception story**

Together, they reveal the **hidden dynamics of pass coverage** that were previously invisible.

This echoes the winner’s elegant closing tone.

---

# **X. Appendix (Optional but adds Data Science Cred)**

* Equations
* Parameter choices
* Peak detection logic
* Sensitivity checks
* Small code blocks
* Explanation of edge-case handling
* Data cleaning steps

This boosts Data Science Score **without cluttering the main narrative**.

---



**Do you want the entire write-up drafted now, or section-by-section?**
