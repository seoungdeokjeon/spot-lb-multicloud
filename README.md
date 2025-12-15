# Spot LB — Spot-Only Multi-Cloud Load Balancing While Maintaining SLOs

This repository is a **public artifact store** for the Spot LB project. It contains the **paper-style report (PDF)** and **evaluation artifacts** (figures/tables). Source code is not included.

## Project Summary
Spot LB studies whether latency-sensitive services can meet **Service Level Objectives (SLOs)** using **only spot instances** in a **multi-cloud** environment—without relying on more expensive on-demand or reserved instances. We propose a **hierarchical load balancing** design that combines **predictive bidding**, **diversification**, and **real-time workload redistribution** to maintain service continuity despite spot preemptions. We validate resiliency using **chaos engineering** and **synthetic load injection** under failure scenarios and high traffic.

## Repository Contents
- `paper/` — paper/report PDF
- `results/` — evaluation artifacts (figures and tables)

## Paper
- `paper/spot-lb-paper.pdf`

## Results
All evaluation figures and tables are stored under `results/`:

### Architecture / Design
- `results/fig-01-dns-geolocation-weighted-routing.png`
- `results/fig-02-health-metrics-collector-collator-dns-weights.png`
- `results/fig-03-cloudsim-spotlb-design.png`

### CloudSim Evaluation
- `results/fig-04-cloudsim-successful-requests-baseline-vs-spotlb.png`
- `results/fig-05-cloudsim-requests-transferred-spotlb.png`
- `results/table-01-cloudsim-simulation-results-baseline-vs-spotlb.png`

### Scenario Response Times
- `results/fig-06-scenario-01-response-times-non-overload-handoff.png`
- `results/fig-07-scenario-01-response-times-overload-handoff.png`
- `results/fig-08-scenario-02-response-times-non-overload-handoff.png`
- `results/fig-09-scenario-02-response-times-overload-handoff.png`
- `results/fig-10-scenario-03-response-times-non-overload-handoff.png`
- `results/fig-11-scenario-03-response-times-overload-handoff.png`
- `results/fig-12-scenario-04-response-times-non-overload-handoff.png`
- `results/fig-13-scenario-04-response-times-overload-handoff.png`

## Authors
- Seoungdeok Jeon
- Zachary Colburn
- (Add additional collaborators as applicable)

## Notes
This repository is intended for **public sharing of the paper PDF and evaluation artifacts**.  
If you later add implementation details, include a separate reproducibility document with exact environment and commands.
