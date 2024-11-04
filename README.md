# User Behavior Analysis Project

## Introduction
This project aims to analyze user behavior data to uncover insights related to screen time, app usage, and battery drain. The analysis focuses on various demographics and operating systems to provide a comprehensive overview of user engagement.

## Table of Contents
1. [Import Libraries and Load the Dataset](#import-libraries-and-load-the-dataset)
2. [Data Cleaning and Exploration](#data-cleaning-and-exploration)
3. [Answering Key Questions with Visualizations](#answering-key-questions-with-visualizations)
   - [3.1 What Age and Gender Use the Most Screen Time?](#31-what-age-and-gender-use-the-most-screen-time)
   - [3.2 Which Operating System Has the Most App Usage Time and Screen On Time?](#32-which-operating-system-has-the-most-app-usage-time-and-screen-on-time)
   - [3.3 Find the Correlation Between Screen On Time and Battery Drain](#33-find-the-correlation-between-screen-on-time-and-battery-drain)
4. [Save Cleaned Data for Tableau Visualization](#save-cleaned-data-for-tableau-visualization)

## Step 1: Import Libraries and Load the Dataset
In this step, we import the necessary libraries and load the user behavior dataset.

```python
# Import necessary libraries
import pandas as pd
import numpy as np
import matplotlib.pyplot as plt
import seaborn as sns
from scipy.stats import pearsonr

# Load the dataset
data = pd.read_csv('user_behavior_dataset.csv')

# Display the first few rows
data.head()
