---
title: "Enhancing Battery SOH Prediction with Butler-Volmer Informed Neural Networks in Data-Scarce Environments"
excerpt: "Published in *Energy* (IF: 9.4, JCR Top 4%) / 1st Author"
collection: portfolio
---

**Journal:** *Energy*, 335, 138316 (2025)
**Role:** 1st Author
**DOI:** [https://doi.org/10.1016/j.energy.2025.138316](https://doi.org/10.1016/j.energy.2025.138316)

## Abstract

This study proposes BVINN (Butler-Volmer Informed Neural Network), a physics-informed machine learning framework that directly incorporates the Butler-Volmer equation into the neural network training process for lithium-ion battery SOH prediction. Experiments on NASA and BIT datasets demonstrate that BVINN achieves high accuracy and physical validity even in data-scarce environments.

## Problem & Solution

| Problem | Limitation of Existing Methods | Solution |
|---------|-------------------------------|----------|
| Battery stability and lifespan management have become critical due to climate change and EV adoption | Physics-based and data-driven models lack interpretability or generalization, especially with limited data | BVINN incorporates electrochemical principles directly into learning via physics-informed regularization |

## Methodology

BVINN incorporates the Butler-Volmer equation as a physics-informed regularization term in the loss function:

- **Data Loss (L_data):** Minimizes difference between actual data and predictions
- **Butler-Volmer Loss (L_BV):** Enforces consistency with Butler-Volmer equation-based current-capacity relationship
- **Initial Condition Loss (L_IC):** Ensures initial values at the first cycle
- **Boundary Condition Loss (L_BC):** Reflects boundary conditions at the last cycle
- **Regeneration Loss (L_regen):** Captures temporary capacity recovery (Capacity Regeneration)
