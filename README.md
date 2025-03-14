# Hyper DON Prediction

## Project Overview

This project aims to predict Deoxynivalenol (DON) concentration in corn samples using hyperspectral imaging data.  The workflow encompasses data preprocessing, dimensionality reduction (if necessary), model training using machine learning algorithms, and a comprehensive evaluation of the model's performance.  The project is implemented in a Jupyter Notebook (`hyper.ipynb`) for interactive execution and analysis.

## Repository Structure

<table>
  <tr>
    <td><code>.</code></td>
    <td></td>
  </tr>
  <tr>
    <td><code>├── hyper.ipynb</code></td>
    <td># Main Jupyter Notebook for the entire workflow</td>
  </tr>
  <tr>
    <td><code>├── requirements.txt</code></td>
    <td># Project dependencies</td>
  </tr>
  <tr>
    <td><code>├── README.md</code></td>
    <td># This file - Project documentation</td>
  </tr>
  <tr>
    <td><code>└── data/</code></td>
    <td># Directory for storing the dataset</td>
  </tr>
  <tr>
    <td><code>    └── your_dataset.csv</code></td>
    <td># ⬅️ Place your CSV dataset file HERE!</td>
  </tr>
</table>

*   **`hyper.ipynb`**:  This Jupyter Notebook contains the complete code for data loading, preprocessing, feature engineering, model training (using algorithms such as XGBoost), model evaluation, and visualization.
*   **`requirements.txt`**:  Lists all the Python packages required to run the project.
*   **`README.md`**: Provides an overview of the project, instructions, and setup information.
*   **`data/`**:  This directory should contain the CSV file with the hyperspectral data and DON concentration values.  **Ensure your dataset file is placed in this directory.**

## Installation and Usage

1.  **Clone the Repository:**

    ```bash
    git clone <repository_link>  # Replace <repository_link> with the actual URL
    cd <repository_directory>   # Replace <repository_directory> with the cloned directory name
    ```

2.  **Install Dependencies:**

    It is highly recommended to create a virtual environment before installing dependencies to avoid conflicts with other Python projects. You can use `venv` or `conda`:

    **Using `venv` (recommended):**

    ```bash
    python3 -m venv .venv  # Create a virtual environment named .venv
    source .venv/bin/activate  # Activate the virtual environment (Linux/macOS)
    # .venv\Scripts\activate  # Activate on Windows (CMD)
    # .venv\Scripts\Activate.ps1 # Activate on Windows (PowerShell)
    pip install -r requirements.txt
    ```

    **Using `conda`:**

    ```bash
    conda create -n myenv python=3.x  # Replace 3.x with your desired Python version
    conda activate myenv
    pip install -r requirements.txt
    ```

3.  **Prepare the Dataset:**

    *   Place your CSV dataset file (e.g., `your_dataset.csv`) inside the `data/` directory.

4.  **Run the Jupyter Notebook:**
    *   Open the anaconda prompt and go to the directory that contains the `hyper.ipynb` file, and then type`Jupyter notebook` to launch.

    ```bash
    jupyter notebook hyper.ipynb
    ```

    *   This will open the notebook in your web browser.  Run all the cells sequentially to execute the entire workflow. You can change the data path inside the notebook if it's needed.

## Dependencies

The project relies on the following Python libraries:

*   Python 3.x
*   `pandas`
*   `numpy`
*   `matplotlib`
*   `seaborn`
*   `scikit-learn` (sklearn)
*   `xgboost`

These dependencies are listed in `requirements.txt` and can be installed using `pip`.

## Instructions / Workflow

1.  **Dataset:** Ensure your dataset CSV file is placed in the `data/` directory.  The notebook assumes a CSV file as input.
2.  **File Path:** The `hyper.ipynb` file includes a variable (likely named `file_path` or similar) that points to the dataset.  *You may need to modify this variable within the notebook if your dataset has a different name or is located in a different subdirectory (although placing it in `data/` is strongly recommended).*
3.  **Execution:** Run all cells in the `hyper.ipynb` notebook sequentially.  This will execute the complete workflow: data loading, preprocessing, model training, and performance evaluation.
4. **Adjustments:** The Notebook is the primary place for making any project-specific changes, exploring different models, or tuning hyperparameters.

## Contact

For any questions, issues, or suggestions, please contact:

*   Ashis Baidya
*   ashunaukari01@gmail.com
