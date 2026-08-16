# AI Model Pareto Trade-offs

This interactive chart compares AI models by intelligence, output speed, and blended token price.

[Explore the interactive chart](https://siioh.github.io/ai-model-pareto/)

## What the chart shows

Each point represents one tested model. Higher intelligence and output speed are better; lower blended price is better. The price axis is logarithmic, which keeps differences among lower-cost models visible.

## Reading the results

- A **Pareto-optimal model** has no tested alternative that is at least as good on every metric and better on at least one.
- A **dominated model** has at least one tested alternative that is at least as good on every metric and better on at least one.
- An **anchor** is the tested model with the best result on one metric:
  - Intelligence anchor: highest intelligence
  - Speed anchor: fastest output
  - Price anchor: lowest blended price
- The **balanced candidate** is the Pareto model closest to the normalized ideal of high intelligence, fast output, and low price.

Highlight a model in the sidebar to see its metrics and locate its point in the 3D plot. You can also show or hide individual models, filter by provider, and switch between light and dark mode.

## Data and assumptions

- The intelligence, price, and speed values come from the sources cited in the visualization and reflect a single point in time. Treat them as comparative estimates rather than permanent facts.
- Blended price assumes a **7:2:1** mix of input, cached-input, and output tokens.
- The comparison covers only the models listed in the visualization. A model's absence does not imply poor quality.

## Files

- `index.html`: self-contained interactive visualization
- `model_pareto_front.png`: publication-ready static figure
- `model_pareto_front.pdf`: vector-ready static figure
- `model_pareto_classification.csv`: classified model data

## Notes and limitations

Performance and pricing vary by provider, region, deployment, workload, and time. Use the visualization to explore trade-offs, then evaluate candidate models against the needs of your production workload.
