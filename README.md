# 🏏 Cricket Analytics

A Python-based data analytics project for exploring, visualizing, and deriving insights from cricket statistics — covering players, teams, matches, and tournaments.

---

## 📋 Table of Contents

- [Overview](#overview)
- [Features](#features)
- [Tech Stack](#tech-stack)
- [Prerequisites](#prerequisites)
- [Installation](#installation)
- [Usage](#usage)
- [Project Structure](#project-structure)
- [Data Sources](#data-sources)
- [Contributing](#contributing)
- [License](#license)

---

## Overview

**Cricket Analytics** aims to make cricket data accessible and meaningful through statistical analysis and visualisation. Whether you want to compare batting averages, analyse bowling economy rates across tournaments, or discover trends in team performance over time, this project provides the tools to do it.

---

## Features

- 📊 **Player Performance Analysis** — batting, bowling, and fielding statistics across formats (Test, ODI, T20)
- 🏆 **Team & Tournament Insights** — win/loss trends, head-to-head records, and tournament summaries
- 📈 **Data Visualisation** — interactive charts and plots for easy interpretation of trends
- 🔎 **Match-by-Match Breakdown** — deep-dive into individual match scorecards and key events
- 🗃️ **Dataset Exploration** — load and query structured cricket datasets with ease
- 🤖 **Predictive Modelling** *(planned)* — machine-learning models for match outcome prediction

---

## Tech Stack

| Layer | Technology |
|---|---|
| Language | Python 3.9+ |
| Data Manipulation | pandas, NumPy |
| Visualisation | Matplotlib, Seaborn, Plotly |
| Machine Learning | scikit-learn *(planned)* |
| Notebooks | Jupyter |
| Code Quality | Ruff, mypy |
| Testing | pytest, coverage |
| Documentation | MkDocs / Sphinx |

---

## Prerequisites

- Python **3.9** or higher
- `pip` (or `Poetry` / `PDM` for dependency management)
- Git

---

## Installation

1. **Clone the repository**

   ```bash
   git clone https://github.com/nDilshan916/cricket-analytics.git
   cd cricket-analytics
   ```

2. **Create and activate a virtual environment**

   ```bash
   python -m venv venv

   # macOS / Linux
   source venv/bin/activate

   # Windows
   venv\Scripts\activate
   ```

3. **Install dependencies**

   ```bash
   pip install -r requirements.txt
   ```

4. *(Optional)* **Install development dependencies**

   ```bash
   pip install -r requirements-dev.txt
   ```

---

## Usage

### Running Jupyter Notebooks

```bash
jupyter notebook notebooks/
```

Open any notebook in the `notebooks/` directory to explore pre-built analyses.

### Running Analysis Scripts

```bash
python scripts/player_analysis.py --player "Virat Kohli" --format odi
python scripts/team_analysis.py --team "India" --tournament "World Cup"
```

### Running Tests

```bash
pytest
```

---

## Project Structure

```
cricket-analytics/
├── data/                   # Raw and processed datasets
│   ├── raw/                # Original, unmodified data files
│   └── processed/          # Cleaned and transformed data
├── notebooks/              # Jupyter notebooks for exploration & analysis
├── scripts/                # Standalone analysis and utility scripts
├── src/
│   └── cricket_analytics/  # Core Python package
│       ├── __init__.py
│       ├── data_loader.py  # Data ingestion utilities
│       ├── analysis.py     # Statistical analysis functions
│       └── visualisation.py  # Plotting and chart helpers
├── tests/                  # Unit and integration tests
├── docs/                   # Project documentation
├── .gitignore
├── requirements.txt        # Runtime dependencies
├── requirements-dev.txt    # Development dependencies
├── pyproject.toml          # Project metadata & tool configuration
└── README.md
```

---

## Data Sources

Cricket data can be sourced from:

- [Cricsheet](https://cricsheet.org/) — ball-by-ball data in YAML/JSON/CSV format
- [ESPN Cricinfo](https://www.espncricinfo.com/) — comprehensive match and player statistics
- [Kaggle Cricket Datasets](https://www.kaggle.com/datasets?search=cricket) — community-contributed datasets

> **Note:** Always review and respect the terms of use for any data source before using it in this project.

---

## Contributing

Contributions are welcome! To get started:

1. Fork the repository
2. Create a feature branch: `git checkout -b feature/your-feature-name`
3. Commit your changes: `git commit -m "Add your feature"`
4. Push to your fork: `git push origin feature/your-feature-name`
5. Open a Pull Request against `main`

Please ensure your code:
- Passes all existing tests (`pytest`)
- Follows the project's code style (run `ruff check .` before committing)
- Includes tests for any new functionality

---

## License

This project is licensed under the [MIT License](LICENSE).

---

> Made with ❤️ for cricket fans and data enthusiasts alike.
