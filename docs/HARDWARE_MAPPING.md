# Hardware mapping considerations

## Compute

SNN inference replaces some dense multiply-accumulate activity with event-driven updates, but this does not automatically guarantee efficiency. The implementation benefit depends on spike sparsity, neuron dynamics, temporal length, and platform support.

## Memory

Important state can include:

- membrane potentials
- thresholds / neuron parameters
- synaptic weights
- spike histories or temporal buffers

For embedded systems, memory traffic can dominate arithmetic cost.

## Precision

Reducing precision can lower storage and arithmetic cost, but numerical effects must be measured rather than assumed. Hardware-aware SNN design therefore benefits from explicit fixed-point / quantization experiments.

## Sparsity

Sparse spikes create an opportunity to avoid unnecessary computation. Real hardware must still provide an efficient event representation and scheduling mechanism to realize that opportunity.

## Platform mapping

Potential deployment targets include:

- neuromorphic accelerators
- FPGAs
- microcontrollers / embedded processors
- heterogeneous SoCs

Each target changes the preferred network structure and execution strategy.
