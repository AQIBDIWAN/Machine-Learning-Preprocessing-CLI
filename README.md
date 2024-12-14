# Machine Learning Preprocessing CLI

## Overview
The **Machine Learning Preprocessing CLI** is a command-line interface tool designed to simplify and streamline the preprocessing of datasets for machine learning projects. It allows users to clean, transform, and preprocess datasets efficiently with minimal effort, directly from the terminal.

---

## Features
- **Data Cleaning**: Handle missing values, remove duplicates, and outliers.
- **Feature Scaling**: Apply normalization or standardization techniques.
- **Encoding**: Encode categorical variables using various encoding techniques (e.g., one-hot, label encoding).
- **Feature Selection**: Automatically identify and select the most relevant features.
- **Custom Transformations**: Apply user-defined preprocessing functions.
- **Pipeline Export**: Save preprocessing pipelines for reuse.

---

## Installation

### Prerequisites
- Python 3.8+
- pip

### Steps
1. Clone the repository:
   ```bash
   git clone https://github.com/yourusername/Machine-Learning-Preprocessing-CLI.git
   cd Machine-Learning-Preprocessing-CLI
   ```
2. Install dependencies:
   ```bash
   pip install -r requirements.txt
   ```
3. Install the package locally:
   ```bash
   pip install .
   ```

---

## Usage

### Basic Commands
Run the tool by invoking the `ml-preprocess` command in the terminal:

```bash
ml-preprocess [OPTIONS]
```

### Options
- `--input, -i` : Path to the input dataset (CSV format).
- `--output, -o` : Path to save the processed dataset.
- `--clean` : Perform data cleaning (e.g., handle missing values, remove duplicates).
- `--scale` : Apply feature scaling (choose between `minmax`, `standard`, or `robust`).
- `--encode` : Encode categorical variables (options: `onehot`, `label`).
- `--select` : Perform feature selection (based on correlation or variance).
- `--custom` : Specify a Python script for custom preprocessing logic.

### Examples
#### Basic Cleaning and Scaling
```bash
ml-preprocess -i data/raw_dataset.csv -o data/processed_dataset.csv --clean --scale minmax
```

#### Encoding and Feature Selection
```bash
ml-preprocess -i data/raw_dataset.csv -o data/processed_dataset.csv --encode onehot --select correlation
```

#### Custom Preprocessing
```bash
ml-preprocess -i data/raw_dataset.csv -o data/processed_dataset.csv --custom my_custom_preprocessor.py
```

---

## Development

### Setting Up for Development
1. Fork and clone the repository:
   ```bash
   git clone https://github.com/yourusername/Machine-Learning-Preprocessing-CLI.git
   ```
2. Create and activate a virtual environment:
   ```bash
   python -m venv venv
   source venv/bin/activate   # On Windows: venv\Scripts\activate
   ```
3. Install development dependencies:
   ```bash
   pip install -r requirements-dev.txt
   ```

### Running Tests
Run the test suite with:
```bash
pytest tests/
```

---

## Contributing
We welcome contributions to the **Machine Learning Preprocessing CLI**! Please follow these steps:
1. Fork the repository.
2. Create a feature branch.
3. Commit your changes with clear commit messages.
4. Push to your fork and submit a pull request.

For detailed contribution guidelines, refer to `CONTRIBUTING.md`.

---

## License
This project is licensed under the MIT License. See the `LICENSE` file for details.

---


## Acknowledgments
- Open-source contributors and the Python community.
- Libraries like pandas, scikit-learn, and numpy that power the tool.

