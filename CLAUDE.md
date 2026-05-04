 # Tufin Data Science Home Assignment

## Context

This is a data science take-home assignment for Tufin. The goal is to predict security-zone tags for unlabeled network objects using observed security policy (firewall rule) data.

The problem is semi-supervised: only a subset of objects have known tags. The approach must be reasonable and well-reasoned — not necessarily the most complex.

## Dataset

- `rules.csv` — allowed connections between objects (`rule_id`, `src_obj_id`, `dst_obj_id`)
- `tags.csv` — known tags for a subset of objects (`obj_id`, `tag`)

**Assumptions (per assignment):**
- All rules are allow rules
- All rules use HTTPS (TCP/443)

## Deliverables

| File | Description |
|------|-------------|
| `notebook.ipynb` | Main notebook with EDA, method, predictions, evaluation, and discussion |
| `predictions.csv` | Columns: `obj_id`, `predicted_tag` — predictions for all unlabeled objects |
| `metrics.csv` | Columns: `metric`, `value` — evaluation metrics |

## Required Notebook Sections

1. **EDA** — Key observations about labeled data, unlabeled data, rule structure, and any anomalies or risks
2. **Method** — Problem framing, chosen approach, and alternatives considered
3. **Predictions** — Tag predictions for all unlabeled objects
4. **Evaluation** — Metrics used, what results mean and don't mean, caveats
5. **Discussion** — Limitations, data risks, and what would be improved with more time

## Guiding Principles

- Reasoning and judgment matter more than model complexity
- A simple, well-explained solution is preferred over an elaborate unexplained one
- Explicitly state assumptions when simplifying
- If incomplete, clearly describe what was done, what was skipped, and what would come next