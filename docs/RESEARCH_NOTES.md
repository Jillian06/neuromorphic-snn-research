# Research notes

## Core topic

Spiking Neural Networks for low-power embedded AI and neuromorphic computing.

## Main engineering perspective

The research was not only about model behavior. A central concern was whether an SNN could be mapped efficiently to constrained hardware.

Relevant dimensions included:

- arithmetic complexity
- memory footprint
- spike sparsity
- temporal simulation cost
- precision requirements
- data movement
- latency
- platform resource limits

## Hardware-aware ML

A model that performs well algorithmically may still be unattractive for embedded deployment if it requires excessive memory traffic, long temporal windows, or expensive neuron-state updates.

The useful design question is therefore:

> What network / encoding / execution choices preserve useful task performance while reducing implementation cost?

## Co-design viewpoint

This leads naturally to hardware–software co-design:

```text
model choice
   ↕
spike encoding
   ↕
precision / state representation
   ↕
memory organization
   ↕
compute architecture
   ↕
latency / energy constraints
```

The value of the work was in analyzing these interactions rather than treating the neural model and hardware target as independent systems.
