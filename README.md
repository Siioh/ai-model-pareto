# AI Model Pareto Trade-offs

An interactive comparison of AI models across intelligence, output speed, and blended price.

[Open the interactive visualization](https://siioh.github.io/ai-model-pareto/)

## What this shows

The chart identifies models on the Pareto frontier: models that are not simultaneously beaten by another tested model on intelligence, speed, and price.

- Higher intelligence is better.
- Higher output speed is better.
- Lower blended price is better.
- Prices use a logarithmic scale so lower-cost models remain distinguishable.

## How to read it

- **Pareto-optimal models** are efficient trade-off choices among the tested models.
- **Dominated models** are outperformed on all three objectives by at least one tested alternative.
- **Anchors** are the single-objective leaders:
  - Intelligence anchor: highest intelligence
  - Speed anchor: fastest output
  - Price anchor: lowest blended price
- **Balanced candidate** is the Pareto model nearest the normalized “ideal” across all three objectives.

Use the sidebar to:

- Highlight a model and locate it in the 3D plot
- View its metrics
- Show or hide individual models
- Filter by provider
- Switch between light and dark mode

## Data and assumptions

- Model metrics are a point-in-time snapshot and should be treated as comparative estimates, not permanent facts.
- Blended price uses a **7:2:1 input : cached-input : output** token mix.
- Intelligence, pricing, and speed values are a point-in-time compilation from the sources cited in the visualization.
- The comparison includes only the models listed in the visualization; absence does not imply poor quality.

## Files

- `index.html` — self-contained interactive visualization
- `model_pareto_front.png` — publication-ready static figure
- `model_pareto_front.pdf` — vector-ready static figure
- `model_pareto_classification.csv` — classified model data

## Notes and limitations

Performance and pricing vary by provider, region, deployment, workload, and time. The visualization is intended to make trade-offs easier to explore, not to replace model-specific evaluation for a production use case.
