
# Rawlsian Ethics Module

Framework derived from Rawls’ veil-of-ignorance principle:

Assume you could be the most negatively affected stakeholder.
Would the recommendation still be fair?

## Pipeline

1. Stakeholder extraction
2. Harm/benefit modeling
3. Worst-off identification
4. Fairness score computation
5. Enforcement

## Enforcement Actions

- Warn
- Require justification
- Suggest least-harm alternative
- Refuse action if threshold breached

## Example Policy YAML

ethics:
  framework: rawls
  worst_off_weight: 0.65
  thresholds:
    warn_below: 0.55
    block_below: 0.35
