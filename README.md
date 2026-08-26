# Layoffs Data Cleaning using SQL

## Overview

This project focuses on cleaning and preparing a real-world layoffs dataset using SQL.

The dataset contains information about company layoffs across different industries, countries, locations, funding stages, and dates. The purpose of this project was to identify and resolve common data-quality issues before the data could be used for further analysis.

## Objective

The main objective was to transform the raw layoffs dataset into a clean and consistent dataset suitable for exploratory data analysis.

The cleaning process included:

* Identifying and removing duplicate records
* Standardizing inconsistent values
* Handling null and missing values
* Converting date values into the appropriate data type
* Populating missing information where possible
* Removing unnecessary columns and data
* Creating a separate staging table to preserve the original dataset

## Tools Used

* **MySQL**
* **MySQL Workbench**

## Data Cleaning Process

### 1. Creating a Staging Table

A staging table was created to work with a copy of the raw dataset while preserving the original data.

### 2. Identifying Duplicate Records

Duplicate records were identified using SQL window functions and `ROW_NUMBER()`.

Records with duplicate row numbers were then removed from the cleaned dataset.

### 3. Standardizing Data

Inconsistent values within categorical fields were standardized to maintain consistency throughout the dataset.

Examples included cleaning inconsistent industry and country values and removing unnecessary whitespace.

### 4. Handling Null Values

Missing values were investigated and handled where additional information could be derived from other records.

Rows with critical missing information that could not be reliably populated were removed where appropriate.

### 5. Standardizing Date Format

The date column was converted from its original format into a proper SQL `DATE` data type.

This makes the dataset easier to use for future time-based analysis.

### 6. Removing Unnecessary Data

Columns and records that were no longer required after the cleaning process were removed from the final dataset.

## SQL Skills Demonstrated

* Data cleaning and transformation
* `CREATE TABLE`
* `INSERT INTO`
* `UPDATE`
* `DELETE`
* `ALTER TABLE`
* `JOIN`
* `CASE`
* `NULL` handling
* String functions
* Date conversion
* Common Table Expressions (CTEs)
* Window functions
* `ROW_NUMBER()`
* Data validation

## Outcome

The raw layoffs dataset was transformed into a cleaner and more consistent dataset that can be used for further exploratory data analysis and visualization.

The cleaning process also provided practical experience working with common data-quality problems encountered in real-world datasets.
