# GDP Data Extraction and Analysis

This project extracts nominal GDP data for the top 10 economies from a Wikipedia page, processes the data, and saves it to a CSV file.

## Project Steps

1.  **Install Libraries:** Installs the necessary Python libraries: pandas, numpy, and xlml.
2.  **Import Libraries:** Imports pandas and numpy.
3.  **Define URL:** Specifies the URL of the Wikipedia page containing the GDP data.
4.  **Extract Data:** Reads the HTML tables from the Wikipedia page using pandas and selects the relevant table (table 3).
5.  **Clean Column Headers:** Replaces the original multi-level column headers with simple numerical indices.
6.  **Select Columns and Rows:** Retains the 'Country/Territory' and 'IMF Estimate' columns and filters the rows to include only the top 10 economies.
7.  **Rename Columns:** Renames the selected columns to 'Country' and 'GDP (Million USD)'.
8.  **Convert Data Type:** Changes the data type of the 'GDP (Million USD)' column to integer.
9.  **Convert Units:** Converts the GDP values from Million USD to Billion USD by dividing by 1000.
10. **Round Values:** Rounds the GDP values to 2 decimal places.
11. **Rename Column Header:** Renames the 'GDP (Million USD)' column header to 'GDP (Billion USD)'.
12. **Save to CSV:** Saves the processed DataFrame to a CSV file named `Largest_economies.csv`.

## Files

*   `GDP Data Extraction and Processing.ipynb`: The Jupyter notebook containing the code for data extraction and processing.
*   `Largest_economies.csv`: The output CSV file containing the top 10 economies and their GDP in Billion USD.

## How to Use

1.  Clone this repository to your local machine.
2.  Open the notebook (`GDP Data Extraction and Processing.ipynb`) in a compatible environment (like Google Colab or Jupyter Notebook).
3.  Run the cells in the notebook sequentially to perform the data extraction and processing.
4.  The resulting `Largest_economies.csv` file will be generated in the same directory as the notebook.

## Requirements

*   Python 3
*   pandas library
*   numpy library
*   xlml library

You can install the required libraries using pip:
