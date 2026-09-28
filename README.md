# Neuromorphic SNN Research

A research portfolio repository summarizing my work on **Spiking Neural Networks (SNNs), low-power embedded AI, and hardware-aware neuromorphic computing**.

> **Scope note:** this repository documents the research direction, design constraints, and hardware–software co-design questions I worked on. I do not currently have a complete public source-code release from the original research period, so this repository intentionally avoids presenting reconstructed code as the historical implementation.

## Research focus

The work investigated how SNN architectures can be adapted for deployment under constrained embedded / neuromorphic hardware environments, with emphasis on:

- event-driven computation
- low-power inference
- resource-aware network design
- hardware-aware optimization
- algorithm ↔ hardware mapping
- embedded and neuromorphic deployment constraints

## Why SNNs?

Conventional neural networks evaluate dense activations at every layer. SNNs instead communicate through sparse spike events and can exploit temporal structure. This makes them attractive for energy-efficient inference when paired with suitable neuromorphic or FPGA-style hardware.

## Hardware–software co-design questions

The research centered on questions such as:

1. How should network structure change when compute, memory, precision, and latency are constrained?
2. Which operations dominate implementation cost?
3. How do spike sparsity and temporal coding affect memory traffic and arithmetic activity?
4. What model-level choices make later mapping to embedded / neuromorphic hardware easier?
5. How should algorithm evaluation incorporate hardware constraints instead of accuracy alone?

## Research workflow

```text
SNN architecture
      ↓
spike representation / temporal behavior
      ↓
compute + memory requirements
      ↓
hardware-aware constraints
      ↓
mapping / implementation considerations
      ↓
energy-efficiency and deployment trade-offs
```

## Repository contents

- [Research notes](docs/RESEARCH_NOTES.md)
- [Hardware mapping considerations](docs/HARDWARE_MAPPING.md)
- [Reproducibility roadmap](docs/REPRODUCIBILITY.md)

## Connection to my broader work

This research fits into a larger interest in **efficient intelligent systems**:

- [ROS 2 autonomous navigation](https://github.com/Jillian06/ros2-autonomous-navigation) — planning + control + robotics software
- [FMCW adaptive BFP FFT](https://github.com/Jillian06/fmcw-radar-bfp-fft) — DSP + FPGA + numerical hardware design
- [Safe A* path planning](https://github.com/Jillian06/safe-astar-path-planning) — autonomous planning research

Together, these projects reflect my interest in connecting **algorithms, learning, control, and efficient hardware**.

## Status

Research experience: **May–June 2025**, University of Toronto & York University.

This repository is documentation-first until original or independently revalidated implementation artifacts are suitable for public release.
