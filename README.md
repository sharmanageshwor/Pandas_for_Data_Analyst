# Pandas Learning Notebook

A collection of Jupyter notebooks for learning and practicing pandas, from Series and DataFrames through data cleaning and analysis workflows.

## Topics Covered

- Series and DataFrames
- Selecting and filtering data
- `loc` and `iloc`
- Adding, removing, and updating columns and rows
- Conditions and boolean filtering
- Indexes: setting, resetting, and using indexes
- Sorting data
- GroupBy operations
- Joining DataFrames
- Data cleaning with real-world datasets

## Notebook Guide

| Notebook | Focus |
| --- | --- |
| [Series and Dataframe.ipynb](Series%20and%20Dataframe.ipynb) | pandas fundamentals |
| [Pandas_selection_clean.ipynb](Pandas_selection_clean.ipynb) | Selection and cleaning |
| [loc and iloc.ipynb](loc%20and%20iloc.ipynb) | Label- and position-based selection |
| [Condition.ipynb](Condition.ipynb) | Conditional filtering |
| [Addingremoving.ipynb](Addingremoving.ipynb) | Adding and removing data |
| [Updating_in_Pandas.ipynb](Updating_in_Pandas.ipynb) | Updating values |
| [Indexes_How_to_Set,_Reset,_and_Use_Indexes.ipynb](Indexes_How_to_Set,_Reset,_and_Use_Indexes.ipynb) | Index management |
| [Sorting_in_pandas.ipynb](Sorting_in_pandas.ipynb) | Sorting rows and columns |
| [GroupBy.ipynb](GroupBy.ipynb) | Grouping and aggregation |
| [Pandas_joins_simple.ipynb](Pandas_joins_simple.ipynb) | Joining and combining DataFrames |
| [titanic_data_cleaning.ipynb](titanic_data_cleaning.ipynb) | Data cleaning with the Titanic dataset |
| [Handwritten Notes of Pandas](Handwritten%20Notes%20of%20Pandas/) | Additional handwritten notes |

## Getting Started

1. Install Python 3.9 or later.
2. Install the required packages:

   ```bash
   python -m pip install pandas jupyter matplotlib seaborn
   ```

3. Start Jupyter from this folder:

   ```bash
   jupyter notebook
   ```

4. Open a notebook and run the cells from top to bottom.

## Basic Example

```python
import pandas as pd

sales = pd.DataFrame(
    {
        "product": ["Notebook", "Pen", "Notebook"],
        "quantity": [2, 5, 3],
        "price": [4.50, 1.25, 4.50],
    }
)

sales["total"] = sales["quantity"] * sales["price"]
print(sales.groupby("product")["total"].sum())
```

## Recommended Learning Order

1. Start with Series and DataFrames.
2. Practice selection, conditions, `loc`, and `iloc`.
3. Learn how to add, remove, update, sort, and index data.
4. Continue with GroupBy and joins.
5. Finish with the data-cleaning notebooks and handwritten notes.
