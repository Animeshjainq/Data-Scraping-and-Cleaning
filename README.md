# Data-Scraping-and-Cleaning LinkedIn
# Data Preprocessing Tool

This Python script is a data preprocessing tool that helps you clean and modify a CSV dataset, specifically designed for data in a format similar to the provided 'JAIPUR DATA - SheetJS.csv'. It utilizes the pandas library for data manipulation and regular expressions for text extraction.

## Prerequisites

Before using this tool, make sure you have the following:

- Python installed (3.6 or higher)
- pandas library installed (`pip install pandas`)
- Basic knowledge of Python and data preprocessing

## Usage

1. Clone or download this repository to your local machine.

2. Place your CSV data file (e.g., `JAIPUR DATA - SheetJS.csv`) in the same directory as this script or provide the full file path in the code.

3. Open the script and adjust the file paths if necessary:

   ```python
   df = pd.read_csv(r"C:\Users\anime\OneDrive\Desktop\JAIPUR DATA - SheetJS.csv")
   ```

4. Customize the data preprocessing steps as needed. You can modify the script to match your specific dataset's structure and requirements.

5. Run the script using a Python environment.

   ```bash
   python preprocess_data.py
   ```

6. The modified dataset will be saved to a new CSV file, `modified_data.csv`, in the same directory as the script.

7. Check the console for information about the number of columns, a preview of the original data, and a message confirming the save operation.

## Data Preprocessing Steps

1. Load the CSV data into a pandas DataFrame.
2. Extract phone numbers from the 5th column using regular expressions and update the 'Phone No' column.
3. Split multiple email addresses in the 'Email' column and keep the first one.
4. Create a new 'NAME' column by concatenating 'First Name' and 'Last Name' columns.
5. Delete unnecessary columns ('First Name', 'Last Name', 'Summary').
6. Remove rows with missing data in the 'Email' column.
7. Save the modified DataFrame to a new CSV file.

Feel free to modify the code to suit your specific data preprocessing needs. Enjoy working with cleaner and more organized data!
