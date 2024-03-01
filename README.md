# Build Recommendation Engine Project

## Table of Contents
1. [Description](#description)
2. [Getting Started](#getting_started)
    1. [Project Structure](#structure)
	2. [Dependencies](#dependencies)
	3. [Setting Up](#setting-enviroment)
	4. [Executing Program](#execution)
3. [Authors](#authors)

<a name="descripton"></a>
## Description

This project focuses on building a recommendation engine for articles on the IBM Watson Studio platform. The engine will make recommendations to users based on their interactions with articles. The project is divided into the following key sections:

This project is divided in the following key sections:

1. Before making recommendations, the data is explored to understand its structure and characteristics.
2. Initial recommendations are made based on the popularity of articles, assuming that articles with the most interactions are the most popular.
3. Recommendations are improved by finding users similar in terms of the articles they have interacted with. Articles from similar users are recommended.
4. An optional section where content-based recommendation systems can be explored using NLP techniques.
5. Machine learning approach to building recommendations. A matrix decomposition is used to predict new articles a user might interact with.

<a name="getting_started"></a>
## Getting Started

To get started with the project, follow the steps below.

<a name="structure"></a>
### Project Structure

```bash
.
├── data
│   ├── articles_community.csv
│   └── user-item-interactions.csv
├── LICENSE
├── Makefile
├── project_tests.py
├── README.md
├── Recommendations_with_IBM.ipynb
├── requirements.txt
├── test_environment.py
├── top_10.p
├── top_20.p
├── top_5.p
└── user_item_matrix.p
```

<a name="dependencies"></a>
Make sure you have the following dependencies installed:

    Python 3.10
    NumPy
    Pandas
    Scikit-Learn
    Matplotlib
    Pickle<a name="material"></a>
### Additional Material

In the notebooks folder, you can find a Jupyter notebook:

1. **Recommendations_with_IBM**: This notebook provides detailed information about the implemented ETL pipeline and the recommendation systems.

<a name="importantfiles"></a>
### Important Files

**project_tests.py**: 



<a name="setting-enviroment"></a>
### Setting Up the Environment with Makefile

To set up the Python environment for this project, follow these steps:

1. If you have conda installed, you can create a new environment with Python 3.10 using the Makefile:
    ```
    make create_environment
    ```

2. This will create a conda environment named `recommendation_engine` with Python 3.10. You can activate this environment with:
    ```
    conda activate recommendation_engine
    ```

3. Next, install the required Python dependencies by running:
    ```
    make requirements
    ```

This will install the necessary libraries listed in `requirements.txt`.

<a name="execution"></a>
### Executing Program

Run the Jupyter notebook Recommendations_with_IBM.ipynb to go through the project and understand the implemented recommendation systems.

<a name="authors"></a>
## Authors

* [Daniel Perdomo](https://github.com/Dalperdomoe)