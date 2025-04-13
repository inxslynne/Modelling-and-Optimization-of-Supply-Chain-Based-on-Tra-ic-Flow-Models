# Project Title

Simulation and Optimization of Supply Chains Based on Traffic Flow Models

## Introduction

This group project focuses on single-chain supply chains and examines both **discrete** and **continuous** models:

- **Discrete Model**: Utilizes discrete-event simulation to capture the exact dynamics of products flowing through each supplier node.
- **Continuous Model**: Adopts a traffic-flow-based approach, where products are treated as “vehicles” moving across suppliers, enabling a more efficient macro-level approximation.
- **Optimization Strategy**: Explores optimization techniques (e.g., minimizing inventory holding costs) using the continuous model to guide resource allocation under certain constraints.

## Highlights

1. **Discrete Model**  
   - Based on queueing theory: each node represents a queue with a processor and buffer.  
   - Tracks exact arrival and departure times of every product, giving a detailed (microscopic) view of the supply chain.

2. **Continuous Model**  
   - Treats the supply chain as a continuum of processing “stations,” using partial differential equations derived from traffic flow principles.  
   - Efficiently handles large-scale scenarios by approximating system dynamics, avoiding the need to track individual items.

3. **Numerical Experiments**  
   - Compare the accuracy of the discrete and continuous approaches under varying parameters (e.g., number of nodes, processing rates, etc.).  
   - Demonstrate that the continuous model can approximate the discrete model closely, while being computationally more efficient.

4. **Optimization & Holding Costs**  
   - Incorporates holding cost coefficients for each node.  
   - Implements algorithms (e.g., Sequential Least Squares Programming, SLSQP) to allocate service rates among suppliers, aiming to minimize total holding costs.

## Repository Structure


```plaintext
.
├── code/
│   └── supply chain final version.ipynb  # Total code
├── docs/
│   └── AdvancedModelingReport.pdf
└── README.md                      # Current file
