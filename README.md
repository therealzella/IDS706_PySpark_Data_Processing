# PySpark Data Processing Project

This project uses PySpark for data processing on a large dataset, specifically for analyzing a cereal dataset. The project includes data transformation and SQL querying capabilities within Databricks and a CI/CD pipeline set up in GitHub Actions.

## Project Structure

- `IDS706_PySpark_Data_Processing_Assignment.ipynb`: Jupyter Notebook containing data processing and transformations using PySpark.
- `requirements.txt`: Lists the Python dependencies required for the project.
- `ci.yml`: GitHub Actions workflow file for Continuous Integration (CI).
- `cereal.csv`: The dataset used in this project (uploaded in Databricks DBFS).

## Setup

1. **Databricks Setup**: 
   - Sign up at [Databricks Community Edition](https://community.cloud.databricks.com/) if you haven't already.
   - Upload `cereal.csv` to `/FileStore/shared_uploads/your_email@domain.com/cereal.csv` in Databricks.

2. **Clone Repository**:
   ```bash
   git clone https://github.com/therealzella/IDS706_PySpark_Data_Processing.git
   cd IDS706_PySpark_Data_Processing

3. **Python Environment**:

- Create a virtual environment (recommended).
- Install dependencies:
  ```bash
  pip install -r requirements.txt

## Usage

The main steps in the notebook include:

Data Loading: Load the cereal dataset from DBFS.
Data Transformation: Apply transformations like filtering and aggregation.
SQL Queries: Use Spark SQL to query the dataset for analysis.

## CI/CD Pipeline

GitHub Actions Workflow
The CI/CD pipeline (ci.yml) is configured to:

- Lint the code with Flake8.
- Run tests using Pytest.
- Execute notebooks with Papermill (if required).
Note: Papermill is only necessary if you want to automate the execution of Jupyter Notebooks in the CI/CD pipeline. Otherwise, it can be omitted for simpler pipelines focusing on PySpark scripts alone.
