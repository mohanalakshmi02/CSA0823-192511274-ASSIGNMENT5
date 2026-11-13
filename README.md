# CSA08 – Python Programming Assignment 5 (CO5)

## Data Acquisition, Cleaning, Analysis and AI Applications

### Project Overview

This repository contains the implementation of Python Programming Assignment 5 (CO5), based on a **City Air-Quality Monitoring Network**.

The project focuses on acquiring, cleaning, storing, analysing and visualising air-quality data collected from multiple monitoring stations. It also explores data validation, adversarial inputs, performance comparisons between different data-processing approaches and basic sentiment analysis.

The assignment demonstrates the practical application of Python programming, file handling, data processing, database management, data visualisation and AI-related techniques.

---

## Assignment Details

| Field | Details |
|---|---|
| Course Code | CSA08 |
| Assignment | Assignment 5 – CO5 |
| Title | Data Acquisition, Cleaning, Analysis and AI Applications |
| Domain | City Air-Quality Monitoring Network |
| Programming Language | Python |
| Database | SQLite |
| Libraries | Pandas, Matplotlib |
| Repository Type | Individual Assignment |

---

## Project Objectives

- Acquire and process air-quality monitoring data.
- Identify and handle missing, duplicate, invalid and inconsistent records.
- Clean and normalise pollutant readings.
- Store cleaned data in an SQLite database.
- Perform SQL queries to obtain useful information.
- Generate charts to analyse air-quality trends.
- Test the system using incorrect and adversarial inputs.
- Compare Python loops, Pandas and SQL-based approaches.
- Evaluate performance using execution time and memory usage.
- Apply sentiment analysis to understand the limitations of basic text-scoring techniques.

---

## Technologies Used

| Technology | Purpose |
|---|---|
| Python | Main programming language |
| CSV Module | Reading and processing CSV files |
| SQLite3 | Database creation, storage and querying |
| Pandas | Data cleaning and data processing |
| Matplotlib | Data visualisation |
| Time Module | Measuring execution time |
| VS Code | Development environment |
| Git and GitHub | Version control and project submission |

---

## Project Tasks

### Part A – Design and Conceptual Analysis

Part A focuses on designing the proposed solution and understanding the concepts required for the implementation.

The work covers:

- Data acquisition and database design.
- Data cleaning and normalisation.
- Data analysis and visualisation.
- Debugging and performance profiling.
- Sentiment analysis and chatbot concepts.

### Part B – Implementation and Experimental Investigation

**B1 – Implement and Validate the Cleaning Pipeline**

- Implemented a data-cleaning pipeline.
- Handled missing and invalid pollutant readings.
- Removed duplicate records.
- Converted Fahrenheit temperatures into Celsius.
- Standardised date, time and numeric formats.
- Stored cleaned data in SQLite.
- Executed SQL queries for air-quality analysis.
- Generated charts using Matplotlib.
- Compared CSV-based processing with Pandas.

**B2 – Engineer Adversarial Data**

- Tested incorrect and malformed input files.
- Examined missing columns, incorrect delimiters, different text encodings and empty files.
- Tested SQL queries with special characters and attempted SQL injection.
- Compared unsafe SQL string construction with parameterised queries.
- Evaluated sentiment scoring using sarcasm, double negatives and mixed opinions.

**B3 – Compare Processing Approaches**

- Examined different data-processing approaches.
- Compared Python loops, library-based processing and SQL operations.
- Evaluated execution performance and processing behaviour.
- Analysed the suitability of each approach for different dataset sizes.

**B4 – Sentiment Analysis and Final Engineering Decision**

- Evaluated sentiment analysis results.
- Examined the limitations of basic sentiment scoring.
- Considered the accuracy, efficiency and reliability of different approaches.
- Prepared the final engineering decision based on the experimental observations.

---

## Data Cleaning Operations

The air-quality dataset contains the following fields:

- Station
- Date
- Hour
- PM2.5
- PM10
- NO₂
- Temperature

The cleaning pipeline addresses:

1. Missing values.
2. Negative and invalid pollutant readings.
3. Duplicate records.
4. Inconsistent date and time formats.
5. Temperature unit conversion.
6. Numeric data standardisation.

Invalid pollutant readings are treated as missing values. Missing values are filled using the previous valid reading from the same station where available, or the median as a fallback.

---

## Performance Evaluation

The CSV module and Pandas implementations were compared using datasets containing 1,000, 100,000 and 1,000,000 records.

| Dataset Size | CSV Execution Time (s) | Pandas Execution Time (s) |
|---:|---:|---:|
| 1,000 | 0.035230 | 0.039933 |
| 100,000 | 0.229893 | 0.026967 |
| 1,000,000 | 2.416614 | 0.243142 |

The experiment showed that Pandas performed better for larger datasets, while the CSV module remained suitable for simpler, smaller-scale processing.

Both implementations produced matching results during correctness verification.

---

## Installation and Execution

### 1. Clone the Repository

```bash
git clone https://github.com/YOUR-USERNAME/YOUR-REPOSITORY.git
```

### 2. Open the Project Folder

```bash
cd YOUR-REPOSITORY
```

### 3. Install Required Libraries

```bash
py -m pip install pandas matplotlib
```

### 4. Run the Python Programs

Run the required Python scripts using:

```bash
py filename.py
```

Replace `filename.py` with the name of the program you want to execute.

---

## Expected Outputs

The project generates or uses the following outputs:

- Raw air-quality CSV dataset.
- Cleaned air-quality CSV dataset.
- SQLite database containing station and reading information.
- SQL query results.
- Air-quality visualisation charts.
- Adversarial input testing results.
- Performance comparison results.
- Sentiment analysis observations.

---

## Learning Outcomes

Through this assignment, the following concepts were practised:

- Python file handling and exception handling.
- Data acquisition and preprocessing.
- Data validation and cleaning.
- SQLite database operations.
- SQL queries and parameterised statements.
- Data visualisation using Matplotlib.
- Data manipulation using Pandas.
- Algorithmic time and space complexity.
- Performance measurement and comparison.
- Adversarial testing and secure programming.
- Basic sentiment analysis and its limitations.

---

## Conclusion

This assignment provided practical experience in developing a data-processing workflow for a City Air-Quality Monitoring Network. It demonstrated how raw data can be acquired, cleaned, stored, analysed and visualised using Python and its supporting libraries.

The experiments also highlighted the importance of input validation, secure database operations, performance evaluation and selecting appropriate tools for different dataset sizes.

Overall, the project strengthened the understanding of Python programming, data engineering concepts, database management and basic AI applications.

---

## Repository Information

**Course:** CSA08 – Python Programming  
**Assignment:** Assignment 5 (CO5)  
**Project:** Data Acquisition, Cleaning, Analysis and AI Applications  
**Domain:** City Air-Quality Monitoring Network  

**GitHub Repository:** YOUR-GITHUB-REPOSITORY-LINK
