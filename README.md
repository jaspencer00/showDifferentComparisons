# Full Mapping Comparison

This Python script compares accounts codes in two systems from a CSV file called "Full Mapping - Full Mapping (Ltd).csv". The CSV file has three columns:

- "Source Main Code": the main code in the source system.
- "Dest Main Code": the main code in the destination system.
- "Sub Code": the sub-code in the destination system.

The script loops through each unique value in column "Source Main Code" and checks if there are any repeats for that code. If there are repeats, the script checks if there are differences in column "Dest Main Code" or "Sub Code". If there are differences, the script saves the results to a new CSV file called "comparison.csv". The new CSV file has the following columns:

- "Col a": the source main code with a difference.
- "Col b": the number of differences.
- "Col c": the first instance of the dest main code + sub code with "/" as a divider.
- "Col d": the second instance of the dest main code + sub code with "/" as a divider, blank if same as "Col c".
- "Col e": the third instance of the dest main code + sub code with "/" as a divider, blank if same as "Col c" or "Col d".

## How to Use

1. Make sure you have Python and pandas library installed.
2. Download the "Full Mapping - Full Mapping (Ltd).csv" file and save it in your desired location.
3. Copy and paste the above Python code into a Python environment or a text editor and save it as a .py file.
4. Replace the file path "/content/sample_data/Full Mapping - Full Mapping (Ltd).csv" in the script with the actual file path of the "Full Mapping - Full Mapping (Ltd).csv" file.
5. Run the script.
6. Check the "comparison.csv" file in the same directory as the Python script for the results.
