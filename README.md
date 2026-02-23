# Data Synthesizer - SDV

## Project Overview
Automated data synthesis tool using SDV (Synthetic Data Vault) for generating large-scale synthetic datasets while preserving statistical properties of original data.

## Features
- **Synthetic Data Generation**: Create realistic synthetic datasets
- **Multi-table Support**: Handle relational database structures
- **Statistical Preservation**: Maintain correlations and distributions
- **Web Interface**: User-friendly interface for data synthesis

## Project Structure
```
├── sdv/                    # Core SDV library
│   ├── single_table/       # Single table synthesis
│   ├── multi_table/        # Multi-table synthesis
│   ├── sequential/         # Time series synthesis
│   └── metadata/           # Data metadata handling
├── tests/                  # Test suites
└── docs/                   # Documentation
```

## Key Technologies
- SDV (Synthetic Data Vault)
- Deep Learning models (CTGAN, CopulaGAN)
- Statistical modeling
- Privacy-preserving data generation

## Requirements
- Python 3.8+
- SDV
- Pandas
- NumPy
- PyTorch

## Installation
```bash
pip install sdv
```

## Usage
```python
from sdv.single_table import CTGANSynthesizer
synthesizer = CTGANSynthesizer(metadata)
synthesizer.fit(data)
synthetic_data = synthesizer.sample(num_rows=1000)
```
