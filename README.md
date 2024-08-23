---

# Documentation: Classification of Type Ia Supernovae Based on Light Curves from ZTF Data

[![License: MIT](https://img.shields.io/badge/License-MIT-yellow.svg)](https://opensource.org/licenses/MIT)
[![Python Version](https://img.shields.io/badge/Python-3.7%2B-blue.svg)](https://www.python.org/downloads/)

## Project Overview

This documentation covers the classification of Type Ia Supernovae (SN Ia) using light curves from the Zwicky Transient Facility (ZTF). The project involves a series of steps including data filtering, feature extraction, and the application of machine learning models.

## Directory Structure and Notebook Descriptions

The `.ipynb_checkpoints` folder contains Jupyter notebooks that guide the user through the data processing and classification pipeline. The following is an overview of each notebook:

### 📂 **1. TAR_to_CSV-checkpoint.ipynb**
- **Function**: Filters alerts to extract extragalactic transient candidates, saving them in CSV format.
- **Details**: This notebook processes raw alert data, applying specific filters to identify potential SN Ia candidates.
- **Output**: A CSV file containing filtered candidates for further analysis.

### 📂 **1.5.Merge Data ZTF Publik-checkpoint.ipynb**
- **Function**: Merges multiple CSV files into a single dataset.
- **Details**: Consolidates individual CSV files generated in the previous step into a unified dataset.
- **Output**: A merged dataset ready for further processing.

### 📂 **2. Extract Pval-checkpoint.ipynb**
- **Function**: Converts magnitudes to flux and calculates p-values for validation.
- **Details**: This notebook focuses on data transformation and statistical validation of SN Ia candidates.
- **Output**: A dataset with flux values and corresponding p-values.

### 📂 **3. Esktrak Data Latih.ipynb**
- **Function**: Completes the dataset by adding labels required for machine learning.
- **Details**: Labels the dataset, preparing it for the training of machine learning models.
- **Output**: A labeled dataset for model training.

### 📂 **4. ML_DATASET_XXX-checkpoint.ipynb**
- **Function**: Applies machine learning models to the labeled dataset, performing validation and evaluation.
- **Details**: These notebooks train, validate, and test various machine learning models on the dataset.
- **Output**: Model performance metrics and evaluation results.

### 📂 **5. Transfer learning Data Baru-checkpoint.ipynb**
- **Function**: Implements transfer learning techniques to enhance model performance.
- **Details**: Applies pre-trained models to the dataset to improve classification accuracy.
- **Output**: Enhanced model performance metrics.

## Installation and Dependencies

To set up the environment, install the necessary dependencies using the following command:

```bash
pip install -r requirements.txt
```

### Key Dependencies:
- **NumPy**: For numerical operations.
- **Pandas**: For data manipulation.
- **Scikit-learn**: For machine learning algorithms.
- **TensorFlow or PyTorch**: For neural networks and transfer learning.
- **Matplotlib or Seaborn**: For data visualization.

## Running the Notebooks

To run the notebooks, use Jupyter Notebook or Jupyter Lab. Start the environment by executing:

```bash
jupyter notebook
```

Navigate to the `.ipynb_checkpoints` directory and execute the notebooks in the order specified above. Each notebook is designed to build upon the previous steps.

## Outputs and Results

The outputs from each notebook are saved locally in the directory and include filtered datasets, computed features, and performance metrics for the models. These results can be reviewed to assess the effectiveness of the classification process.

### Visualization

Throughout the notebooks, visualization tools like Matplotlib and Seaborn are used to generate plots and graphs that provide insight into the data and model performance. Users can interact with these visualizations by running the corresponding cells.

## Documentation and Notes

- The notebooks contain detailed comments explaining the purpose of each code block.
- Markdown cells within the notebooks provide additional context and explanations, helping users understand the workflow.

### Additional Resources
- [ZTF Data Documentation](https://www.ztf.caltech.edu/page/documentation)
- [Scikit-learn Documentation](https://scikit-learn.org/stable/documentation.html)
- [TensorFlow Documentation](https://www.tensorflow.org/guide)

## Contribution Guidelines

This project is open-source and contributions are welcome. Please follow the standard GitHub workflow for contributing, and refer to the [CONTRIBUTING.md](./CONTRIBUTING.md) file for more details.

### License

This project is licensed under the MIT License. See the [LICENSE](./LICENSE) file for more information.

---
