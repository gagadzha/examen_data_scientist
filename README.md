# README for Data Analysis in Python Exam

## Introduction

This project involves analyzing a simulated dataset of births in Belgium for the year 2019. The data is contained in `.csv` files, each labeled with the actual birth date of the individuals in the file. The goal is to explore this dataset through various data manipulation and visualization techniques.

Here's a concise description of your project's folder structure and files:

- **`examen_env.yml`**: YAML file specifying the conda environment for the project.
- **`data/geboortes/`**: Directory containing CSV files with birth data for 2019.
- **`examen.ipynb`**: Jupyter Notebook with the data analysis code and findings.
- **`opgave.pdf`**: PDF document outlining the data science exam assignment.
- **`README.md`**: Markdown file providing an overview and instructions for the project.

This structure organizes the environment setup, data, analysis, assignment details, and project documentation.

### Key Steps:
- Create a Virtual Environment and export a `.yml` file to include in the codebase.
- Set up a GitHub page with a `.gitignore` and `readme.md`, and include a link to the GitHub repo in the readme file.
- Clean up the code for clarity and understandability.
- At the end, create a `.zip` file of the entire codebase for submission.

## Code Breakdown

### Step 1: Data Import

The first block of code involves iterating over all files in the `data/geboortes` directory, reading each `.csv` file, and merging them into one large DataFrame. An extra column is added to represent the "day of the year" for each birth date.


### Getting to Know Our Data

This section converts 'verwachte datum' (expected birth date) to a datetime object and handles invalid dates in 'werkelijke datum' (actual birth date). It provides an overview of the dataset structure and types.

### Step 2: Daily Birth Analysis

#### Question 1: 
A plot is created to visualize the number of births per day throughout the year.

#### Question 2: Outlier Identification and Handling

Dates with birth counts deviating more than 50% from the average are classified as outliers and are addressed appropriately. Notably, outliers on January 1 and July 1 are due to misrecorded dates and are removed from the main dataset and added to `df_wrong`.

### Step 3: Research Questions

#### Research 1: Unisex Names

Several questions regarding unisex names in the dataset are answered, including the number of unisex names, the most common unisex name among males and females, and the most popular unisex name overall.

#### Visualization:
A visualization is created to show all genuine unisex names and their relative occurrences among males and females.

#### Research 2: Accuracy of Estimated Delivery Dates

A comparison is made between the total number of births per day and the total number of expected births. A histogram and scatter plot are used to analyze the deviation from expected birth dates.

#### Research 3: Number of Names vs. Number of Babies

An investigation into the relationship between the number of unique names and the number of babies born. This section challenges the linear assumption of this relationship and encourages a deeper analysis based on the provided dataset.

## Conclusion

Each code block serves a specific purpose in the data analysis process, from data preparation and cleaning to in-depth analysis and visualization. This readme provides a concise summary of each step, guiding the reader through the logical flow of the project.