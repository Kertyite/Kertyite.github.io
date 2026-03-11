---
title: "Robust SOH Prediction for Lithium-Ion Batteries via ProbSparse Informer Architecture"
excerpt: "Presented at *2025 IEEE Global Reliability & PHM Conference (PHM-Xi'an)* / 1st Author"
collection: portfolio
---

**Conference:** *2025 IEEE Global Reliability & PHM Conference* (PHM-Xi'an), sponsored by IEEE Reliability Society
**Role:** 1st Author

## Abstract

This study proposes an end-to-end SOH prediction framework using the Informer, a Transformer-based model, with raw cycling data as input. Experiments on NASA and CALCE datasets show that Informer achieves higher accuracy and generalization than LSTM and standard Transformer, demonstrating its viability for Battery Management Systems (BMS).

## Problem & Solution

| Problem | Limitation of Existing Methods | Solution |
|---------|-------------------------------|----------|
| Battery degradation occurs as a time-series process, requiring long-term dependency modeling | RNN/LSTM/GRU capture long-term dependencies but lack parallelization; Transformer suffers from information loss in long sequences | Informer with ProbSparse Attention focuses on critical time steps and Self-Attention Distilling removes redundant information |

## Methodology

- **ProbSparse Self-Attention:** Reduces computational complexity of standard Transformer and enables efficient learning on long sequences by focusing on important time steps
- **Informer Encoder:** Parallel multi-distilling stacks learn both fine-grained short-term patterns and long-term dependencies simultaneously
- **Informer Decoder:** Masked ProbSparse Attention blocks future information while combining Encoder outputs to generate SOH estimates
