# Evaluate Manufacturing Process Using Statistical Process Control

## Project Overview

This project focuses on enhancing the monitoring and control of manufacturing processes using a methodical approach known as Statistical Process Control (SPC). The main objective is to ensure that the manufacturing process operates within an acceptable range, which is essential for maintaining consistent high-quality production.

### Key Concepts
- **Statistical Process Control (SPC)**: A strategy that uses data to determine the efficiency of a process, making adjustments only when necessary.
- **Control Limits**: The process is considered acceptable if it operates within the Upper Control Limit (UCL) and Lower Control Limit (LCL).

### Goals
- Analyse historical manufacturing data.
- Define acceptable range using UCL and LCL.
- Identify points in the process that require adjustments.

## Data Description

The analysis is based on data from the `manufacturing_parts` table in a PostgreSQL database and a corresponding `parts.csv` file.

### Data Fields
- `item_no`: The item number.
- `length`: The length of the item.
- `width`: The width of the item.
- `height`: The height of the item.
- `operator`: The operating machine.

## Tasks and Analysis

1. **Database Connection**
   - Connect to the PostgreSQL database.
   - Load data from the table into a Pandas DataFrame.

2. **Exploratory Data Analysis (EDA)**
   - Assess dataset integrity (no missing values).
   - Evaluate dataset composition (500 items).
   - Analyse data variation (mean values and standard deviations for length, width, and height).

3. **Control Limit Calculation and Alert System**
   - Use UCL and LCL formulas to establish control limits.
   - Create an alert system to flag deviations from the control limits.
   - Focus on the height measurement, employing a specific windowing technique for analysis.

## Conclusion

This notebook serves as a practical application of SPC in manufacturing, demonstrating how data-driven approaches can significantly enhance process monitoring and quality control.

## Skills Applied in the Project

In the course of this project, a variety of technical skills and tools were utilized to achieve the objectives. These include:

- **SQLalchemy**: Used for connecting to the PostgreSQL database to retrieve the necessary data.
- **SQL**: Used for querying the PostgreSQL database to retrieve the necessary data.
- **Python**: The primary programming language for analysis and algorithm development.
- **Pandas**: Employed for data manipulation and analysis, providing the means to handle the data efficiently.
- **Matplotlib & Seaborn**: These Python libraries were used for data visualisation, helping in the interpretation of results and trends in the data.
- **Statistical Analysis**: Fundamental statistical methods were applied to determine control limits and assess the manufacturing process.
- **Jupyter Notebook**: Served as the development environment, facilitating an interactive approach to coding, documenting, and presenting the analysis.