# Python 101 Workshop — Library Circulation Analytics (Main)

**Audience:** non-technical stakeholders / new analysts  
**Duration:** 60–90 minutes  
**Goal:** learn how to turn circulation data into actionable insights using pandas + matplotlib.

## Agenda
1) (5 min) Project context + what questions matter
2) (10 min) Data model overview (items / patrons / txns / holds)
3) (20 min) KPI basics: late rate, renewal rate, hold wait quantiles
4) (20 min) Segmentation: who is late? what gets renewed?
5) (15 min) Viz Clinic mindset: bad chart → improved chart → actions
6) (Optional) Mini-exercises + solutions

## Datasets
- `data/txns.csv` (circulation transactions)
- `data/holds.csv` (hold requests + wait time)
- `data/items.csv`, `data/patrons.csv`

## Learning outcomes
- Load CSVs, validate schema, compute derived flags
- Build KPI tables and trend charts
- Use quantiles to describe long-tail experience
- Prioritize segments by impact (volume × rate)
- Package insights into a repeatable report
