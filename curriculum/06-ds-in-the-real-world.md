# S06 — DS in the Real World

S06 prepares students to deliver, operate, monitor, and maintain a data-science product. It also develops skills required for the Capstone project.

## Curriculum overview

| Unit  | Name                          |
|-------|-------------------------------|
| BLU13 | Basic Model Deployment        |
| BLU14 | Deployment in the Real World  |
| BLU15 | Model CSI                     |

## BLU13 — Basic Model Deployment

- Serialize and deserialize scikit-learn models.
- Define the train, serialize, load, and predict data journey.
- Build a Flask service that accepts prediction requests and ground-truth updates.
- Deploy the service with Railway using the `LDSSA/railway-model-deploy` project.
- Test the deployed endpoints and diagnose common deployment problems.

## BLU14 — Deployment in the Real World

- Translate client, privacy, fairness, and operational requirements into technical decisions.
- Establish appropriate data splits, normalization, baselines, and trade-offs.
- Define and validate accepted input formats, values, and missing-data behavior.
- Make a service robust to malformed inputs and operational failures.
- Add logging, metrics, monitoring, alerting, and automated tests.

## BLU15 — Model CSI

- Diagnose model underperformance over time.
- Distinguish data drift, target drift, and concept drift.
- Work with robustness issues and unavailable or delayed ground truth.
- Detect changes with distributions, histograms, Kolmogorov–Smirnov tests, target distributions, and correlations.
- Choose manual, periodic, or continuous retraining strategies and suitable retraining data.
- Calibrate, repair, validate, and redeploy models while accounting for production risks.
