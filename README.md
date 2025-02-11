
# Astronomy Data Analysis

Repository untuk analisis data astronomi, menggunakan Python dan machine learning untuk mengolah dan menganalisis data observasi astronomi.

## Struktur Repository

```
astronomy-data-analysis/
├── data/              # Direktori data
│   ├── raw/          # Data mentah
│   ├── processed/    # Data yang sudah diolah
│   └── external/     # Data dari sumber eksternal
├── notebooks/        # Jupyter notebooks
│   ├── exploration/  # EDA notebooks
│   ├── analysis/     # Analisis mendalam
│   └── visualization/# Visualisasi data
└── src/              # Source code
    ├── data/         # Script pengolahan data
    ├── features/     # Feature engineering
    ├── models/       # Model ML
    └── visualization/# Kode visualisasi
```

## Setup Environment

1. Clone repository:

```bash
git clone https://github.com/yourusername/astronomy-data-analysis.git
cd astronomy-data-analysis
```

2. Create virtual environment:

```bash
python -m venv venv
source venv/bin/activate  # Linux/Mac
# atau
venv\Scripts\activate     # Windows
```

3. Install dependencies:

```bash
pip install -r requirements.txt
```

## Workflow Analisis Data

### 1. Data Processing

```python
from src.data.make_dataset import load_data
from src.data.process_data import preprocess_spectrum

# Load data
raw_data = load_data("path/to/data")

# Preprocess
processed_data = preprocess_spectrum(raw_data)
```

### 2. Feature Engineering

```python
from src.features.build_features import extract_features

features = extract_features(processed_data)
```

### 3. Model Training

```python
from src.models.train_model import train_classifier

model = train_classifier(features, labels)
```

## Notebooks

### Exploration

- `01_initial_data_exploration.ipynb`: EDA awal
- `02_feature_analysis.ipynb`: Analisis fitur
- `03_statistical_tests.ipynb`: Pengujian statistik

### Analysis

- `01_spectral_analysis.ipynb`: Analisis spektral
- `02_variable_star_analysis.ipynb`: Analisis bintang variabel
- `03_classification_models.ipynb`: Model klasifikasi

### Visualization

- `01_data_visualization.ipynb`: Visualisasi data
- `02_results_visualization.ipynb`: Visualisasi hasil
- `03_interactive_plots.ipynb`: Plot interaktif

## Data Sources

### Raw Data

- Spektrum bintang
- Data fotometri
- Data variabilitas

### External Data

- Katalog SDSS
- Data AAVSO
- Reference spectra

## Features

### Data Processing

- Reduksi data spektral
- Kalibrasi fotometri
- Cleaning dan normalisasi

### Analysis

- Spectral line analysis
- Period detection
- Classification methods

### Visualization

- Interactive plots
- Statistical visualizations
- Time series analysis

## Testing

Run tests:

```bash
pytest tests/
```

## Contributing

1. Fork repository
2. Create feature branch
3. Implement changes
4. Run tests
5. Submit pull request

## Dependencies

### Required

- numpy
- pandas
- astropy
- scipy
- scikit-learn
- matplotlib

### Optional

- tensorflow/pytorch
- specutils
- astroML

## Development Guidelines

### Code Style

- PEP 8 compliance
- Type hints
- Comprehensive docstrings

### Documentation

- Function documentation
- Notebook markdown
- Example usage

## Project Status

- Data Processing: Active
- Feature Engineering: In Progress
- Model Development: Planning

## Roadmap

- [ ] Implement basic pipeline
- [ ] Add advanced features
- [ ] Develop ML models
- [ ] Create visualization dashboard
- [ ] Add API endpoints

## Contact

- Email: [khalifardy.miqdarsah@gmail.com]
- GitHub: [@khalifardy]

## License

MIT License - see [LICENSE](LICENSE)

## Acknowledgments

- Data sources
- Research papers
- Open source tools
- Community support

## Notes

- Active development
- Regular updates
- Open for collaboration
- Documentation WIP
