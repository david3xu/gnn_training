# GNN Training for MaintIE Dataset

This project provides a hardware-optimized pipeline for training Graph Neural Networks (GNNs) on the MaintIE maintenance text dataset for entity recognition and relation extraction.

## Features
- Memory-optimized data processing for 128GB+ RAM systems
- Parallel GNN training for 16-core CPUs
- Modular architecture for progressive model complexity
- Real-time resource monitoring and reporting
- Production-ready model serving with FastAPI

## Directory Structure
```
gnn_training/
├── data/
│   ├── raw/                    # Original MaintIE data
│   ├── processed/              # Converted graph data
│   └── splits/                 # Train/val/test splits
├── models/
│   ├── architectures/          # GNN model definitions
│   ├── training/               # Training utilities
│   └── checkpoints/            # Saved model weights
├── config/
│   └── training_config.yaml    # Training and data config
├── src/
│   ├── data_processing/        # Data pipeline
│   ├── models/                 # Model implementations
│   ├── training/               # Training loops
│   ├── evaluation/             # Metrics and validation
│   └── serving/                # Model serving
├── scripts/
├── tests/
└── requirements.txt
```

## Getting Started
1. Install dependencies: `pip install -r requirements.txt`
2. Prepare MaintIE data in `data/raw/`
3. Configure paths in `config/training_config.yaml`
4. Run training scripts in `scripts/`

See the training guide for details.
