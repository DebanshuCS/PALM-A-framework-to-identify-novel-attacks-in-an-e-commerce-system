
# PALM

## Overview

PALM is an innovative framework that bridges the gap between event log analysis and threat modeling in e-commerce systems. By leveraging process mining techniques and graph convolutional networks, PALM transforms often-overlooked event log data into predictive insights for enhanced security analysis.

## Features

- Event log processing and analysis
- Process model discovery using Inductive Miner algorithm
- Attack graph generation incorporating domain knowledge
- Novel exploit prediction using Graph Convolutional Networks (GCN)


## Flow Chart

```mermaid
graph TD;
    A[palm/] --> B[data/];
    B --> B1[raw/];
    B --> B2[processed/];

    A --> C[src/];
    C --> C1[preprocessing/];
    C --> C2[process_mining/];
    C --> C3[attack_graph/];
    C --> C4[graph_convolution_network/];

    A --> D[model/];

    A --> E[tests/];

    E[tests/] --> F[evaluation/];
```

## Usage

1. Preprocess the raw event log data,

2. Discover the process model,

3. Generate the attack graph,

4. Train and evaluate the GNN models,

## Results

Our model achieves the following performance on the test set:

- Accuracy: 83.33%
- Precision: 83.33%
- Recall: 88.24%
- F1 Score: 85.71%
- AUC-ROC: 0.9186
