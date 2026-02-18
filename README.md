# Filters – Simulation Exercise (LTspice + MATLAB)

**Course:** 521304A Filters – Simulation Exercise  
**Degree Programme:** Electronics (Master’s)  
**Author:** Arafat Miah (Study right no: 2512200)  
**Tools:** LTspice, MATLAB  
**Key parameter:** `ddmmyy = 151299`

---

## Overview

This repository contains my completed work for the **Filters – Simulation Exercise**, including:
- LTspice implementations and AC simulations of several analog filter circuits
- Design steps based on given transfer functions and Chebyshev prototype tables
- Group delay evaluation and improvement using an all-pass equalizer (APE)
- A MATLAB script to plot the pole–zero map of the optimized APE:contentReference[oaicite:1]{index=1}

---

## What’s Included (Tasks)

### Task 1 — Multiple-Feedback filter demos
- Simulated the given MFB circuits and documented component values.
- Verified responses (LP/HP/BP) and cutoff matching.

### Task 2 — Third-order active-RC all-pole filter
- Built a 3rd-order all-pole low-pass by cascading a 2nd-order section + 1st-order pole.
- Compared the response with Circuit A.

### Task 3 — Circuit A (balanced version)
- Implemented a differential/balanced version using a fully-differential amplifier concept.
- Verified the differential output matches the original response.

### Task 4 — Ladder filter with transfer function D
- Converted an LP ladder prototype into a BP ladder using LP→BP transformation.
- Scaled/denormalized values and verified that the ladder response matches the transfer function D.

### Task 5 — All-pass equalizer (APE) for transfer function D
- Measured group delay range of the BP response.
- Tuned APE parameters to reduce group-delay variation while keeping magnitude essentially unchanged.
- Generated the pole–zero map of the optimized APE in MATLAB. :contentReference[oaicite:2]{index=2}

---

## Repository Structure (Recommended)

```text
filters-simulation-exercise/
│
├─ report/
│  └─ Filters_Design_Exercise_Arafat_Miah_2512200.pdf
│
├─ ltspice/
│  ├─ task1.asc
│  ├─ task2.asc
│  ├─ task3.asc
│  ├─ task4.asc
│  └─ task5.asc
│
├─ matlab/
│  └─ task5_pole_zero_map.m
│
└─ README.md
