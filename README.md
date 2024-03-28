# R_Place Analysis Project


### Overview
This repository contains code and resources for analyzing data from the R_Place platform. The dataset comprises 130 million rows of data capturing pixel placement and replacement by over 8 million users. The analysis aims to identify bot activities within the dataset.

### Data Preparation
The raw data is stored in Amazon S3 and is available for download. To replicate the project, follow these steps:

Download the raw data from Amazon S3.
Convert the CSV file into a Parquet file format using the provided conversion script.
Split the Parquet file into five smaller files for ease of analysis.

### Analysis
#### Part 1 - Finding Bots
In this section, we identify potential bot activities by analyzing pixel placement and color changes. The process involves:

Filtering pixels based on placement time and color.
Detecting color changes over time.
Identifying immediate color changes back to the original within a specified timeframe.
To run the analysis, ensure you have the following libraries installed:

Parquet
Boto3
PyArrow
Pandas
Numpy
Os
Glob
Shutil
Run the provided Jupyter Notebook (Part1_Finding_Bots.ipynb) to execute the code.

#### Part 2 - Plotting Bot Activities
This section visualizes the identified bot activities on a coordinate plane. The notebook (Part2_Plotting_Bot_Activities.ipynb) contains code to plot the pixels based on their x-y coordinates.

### Additional Resources
Extended Slide Deck: Refer to R_Place Analysis Extended Slide Deck.pptx for a detailed overview of the analysis process.
Data Summary and Visualizations: Explore early data summary and visualizations in the Tableau file RPlace_Project.twb.
Contributors
Minh Tran - Project Lead
Brian Sobell
Riley Svennson

### License
This project is licensed under the MIT License.

### Contact
For any inquiries or feedback, feel free to reach out:

Email: minh.trancao30@gmail.com
