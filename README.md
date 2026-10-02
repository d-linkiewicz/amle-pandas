# Introduction to Pandas

This repository introduces Pandas, the library at the centre of most data work in Python. Working through the notebooks, you load tabular data, select, filter, and summarise it, combine datasets, work with dates, and produce basic plots.

## Learning Objectives

By the end of this repository, you should be able to:

- Load a CSV file into a DataFrame, and report its shape, column types, and summary statistics.
- Select rows and columns with `[]`, `.loc[]`, and `.iloc[]`, and filter rows with boolean conditions.
- Summarise a dataset with `groupby`, value counts, and new calculated columns, and answer a question about it with the result.
- Choose a histogram, scatter plot, box plot, or bar chart for a given question, and create it from a DataFrame.
- Convert a text column to dates with `pd.to_datetime()`, and extract the day, month, year, or weekday.
- Combine DataFrames with `pd.concat()`, `df.join()`, and `pd.merge()`, and predict how many rows each join type returns.
- Bin a numeric column with `pd.cut()`, and summarise it across two dimensions with `pd.pivot_table()`.

## Learning Path

The modules build on each other in order.

### 1 - Basics

Core Pandas: DataFrames, selection, filtering, grouping, and plotting.

| File | Description |
| --- | --- |
| [**01 - Introduction to Pandas**](1_basics/01_intro_to_pandas.ipynb) | Create and load DataFrames, inspect them, select with `.loc` / `.iloc`, filter, group, and handle missing values |
| [**02 - Exercise: Filtering and Aggregating**](1_basics/02_exercise_filter_aggregate.ipynb) | Practice on the red wine data: inspecting, selecting, filtering, grouping, and new columns |
| [**03 - Plotting with Pandas**](1_basics/03_plotting.ipynb) | Histograms, scatter plots, box plots, and bar charts with the Pandas `.plot()` method |
| [**04 - Exercise: Exploring the Iris Data**](1_basics/04_exercise_iris.ipynb) | Practice on the Iris data: statistics, groupby, new columns, filtering, and two plots |
| [**05 - Exercise: Bike Share Analysis**](1_basics/05_exercise_bike_share.ipynb) | An end-to-end analysis of bike-share trips: cleaning, counts, cross-tabulation, and trip durations |

### 2 - Dates and Combining

Dates and times, combining DataFrames, binning, and pivot tables.

| File | Description |
| --- | --- |
| [**01 - Dates and Times**](2_dates_and_combining/01_dates_and_times.ipynb) | Python's `datetime` module, parsing and formatting dates, `timedelta`, and dates in Pandas |
| [**02 - Combining DataFrames**](2_dates_and_combining/02_combining_dataframes.ipynb) | Concatenation, joins, and merges, plus dummy variables, binning with `pd.cut()`, and pivot tables |
| [**03 - Exercise: Binning and Pivot Tables**](2_dates_and_combining/03_exercise_bin_pivot.ipynb) | Practice on the red and white wine data: combining, filtering, binning, and pivot tables |

### Additional Folders and Files

| File / Folder | Description |
| --- | --- |
| [**Data**](data/) | CSV datasets used by the notebooks (`abalone`, `bike_share`, `iris`, `seattle-weather`, `winequality`) |
| [**Assets**](assets/) | Images embedded in the notebooks |
| [**Solutions**](solutions/) | Worked solutions to the exercises in the notebooks |
| [**pyproject.toml**](pyproject.toml) | Project configuration and dependencies |
| [**uv.lock**](uv.lock) | Reproducible dependency lock file |

## Setup

> [!NOTE]
> Throughout these steps, text in angle brackets like `<repo-name>` is a
> **placeholder**. Replace it including the `< >` brackets with your own
> value. For example, `cd <repo-name>` becomes `cd my-pandas-project`.

### 1. Create the Repository from the Template

Click **Use this template** on GitHub.

When creating the repository:

- Set yourself as the **Owner**
- Choose a repository name
- Disable **Include all branches**
- Click **Create repository**

> [!IMPORTANT]
> If you are working in pairs or groups, only **one person** should complete this step.

---

### 2. Add Collaborators (Pairs/Groups Only)

If working with teammates:

1. Open the repository on GitHub
2. Go to **Settings → Collaborators**
3. Add your teammates as collaborators
4. Share the repository link with your team

---

### 3. Clone the Repository

Copy the SSH URL from the **Code** button on GitHub, then run:

```bash
git clone <copied-ssh-url>
```

The copied SSH URL will look like:
`git@github.com:<your-username>/<repo-name>.git`.

---

### 4. Move into the Project Folder and Install Dependencies

This installs all dependencies and creates a virtual environment in `.venv/`.

```bash
cd <repo-name>
uv sync
```

---

### 5. Open the Notebooks

> [!NOTE]
> Open VS Code from the project root so it detects the environment created by `uv sync`.

Launch VS Code in the project root:

```bash
code .
```

Then open a notebook and select the Python environment created by `uv sync` as the kernel.

## References & Further Reading

- [**10 Minutes To Pandas**](https://pandas.pydata.org/docs/user_guide/10min.html): Official short introduction for new pandas users.
- [**Pandas Getting Started Tutorials**](https://pandas.pydata.org/docs/getting_started/intro_tutorials/index.html): Task-focused official tutorials covering loading, selecting, plotting, and combining data.
- [**Python Plotting With Matplotlib (Real Python)**](https://realpython.com/python-matplotlib-guide/): A clear, practical guide to Matplotlib's figure/axes model and its integration with pandas.
- [**Kaggle Learn Pandas**](https://www.kaggle.com/learn/pandas): A free hands-on course that applies pandas to real datasets.
