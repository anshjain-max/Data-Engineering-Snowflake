# Data Engineering Pipelines with pandas on Snowflake

This repository contains a demo project that showcases how to build scalable data engineering pipelines using **pandas on Snowflake**. By leveraging the **Snowpark pandas API**, you can perform efficient data transformations, feature engineering, and schedule serverless tasks directly within the Snowflake ecosystem.

## Project Overview

This project utilizes the [Snowflake Sample TPC-H dataset](https://docs.snowflake.com/en/user-guide/sample-data-tpch) from the `SNOWFLAKE_SAMPLE_DATA` database. The workflow includes:

- **Loading data** from Snowflake tables into pandas dataframes.
- **Transforming and aggregating data** to create new features.
- **Visualizing results** using Python libraries like `matplotlib` and `seaborn`.
- **Saving results** back into Snowflake tables.
- **Scheduling feature engineering tasks** using Snowflake's serverless task framework.

## Key Features

- **Scalable Data Processing**: Run pandas operations at scale within Snowflake.
- **Visualization**: Use Python libraries to create insightful data visualizations.
- **Integration**: Seamless interaction between Snowflake and Python.

## Prerequisites

### Snowflake Setup

Ensure you have access to:

- A Snowflake account.
- The `SNOWFLAKE_SAMPLE_DATA` shared database.

### Environment Setup

This project requires a Python environment. Install the necessary dependencies using the provided `environment.yml` file:

```bash
git clone <repository-url>
cd <repository-directory>
conda env create -f environment.yml
conda activate app_environment
```

### Required Python Libraries

- `modin==0.28.1`
- `matplotlib`
- `seaborn`
- `snowflake`

## Running the Notebook

The Jupyter Notebook `0_start_here.ipynb` provides a step-by-step guide to:

1. Load data from Snowflake into pandas dataframes.
2. Perform feature engineering and transformations.
3. Save transformed data back into Snowflake.
4. Visualize insights using `matplotlib` and `seaborn`.

### Instructions

- Open the `0_start_here.ipynb` notebook in your Jupyter environment.
- Follow the instructions in each cell to execute the workflow.

## Key Concepts

### Snowpark pandas API

The Snowpark pandas API, available as part of the Snowpark Python library, enables scalable data processing directly within the Snowflake platform. This approach combines the simplicity of pandas with the power of Snowflake's computational engine.

### Libraries Used

- **modin**: Accelerated pandas for scalable data processing.
- **matplotlib & seaborn**: Libraries for creating data visualizations.
- **snowflake**: Python connector for Snowflake.

## Scheduling Tasks

Learn how to create and schedule serverless tasks in Snowflake to automate feature engineering pipelines.

## Contributing

Contributions are welcome! If you have suggestions or improvements, please open an issue or submit a pull request.



