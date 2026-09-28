# Reproducibility roadmap

This repository currently avoids publishing reconstructed historical code as though it were the original research implementation.

A future public reproduction should include:

1. a clearly identified dataset and task
2. a baseline ANN and SNN
3. deterministic train / validation / test splits
4. explicit spike encoding and neuron model
5. accuracy plus sparsity / operation-count metrics
6. parameter and state-memory estimates
7. quantization experiments
8. deployment-oriented latency / energy proxies
9. hardware mapping assumptions
10. reproducible environment and scripts

Any future implementation should be labeled either **original artifact** or **new reproduction** so provenance remains clear.
