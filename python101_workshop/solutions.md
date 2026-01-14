# Workshop Solutions / Instructor Notes

## Exercise 1 — p95 by season
- Add month + season column based on request_dt
- Groupby season and compute quantiles

## Exercise 2 — top 3 segments (transactions >= 80)
- Filter `late_seg[late_seg.transactions >= 80]`
- Sort by risk_score desc and take head(3)

## Exercise 3 — example improvement ideas
- Track p90/p95 hold wait SLIs during semester peak
- Targeted reminder + renewal nudges for high-volume segments
- Asset-protection workflow for laptops (earlier reminders / policy tweaks)
