# Sales Data Processing with PySpark

## Overview
This script processes sales data from a CSV file, aggregates it by month, and saves the results into separate CSV files for each month. It utilizes PySpark to handle the data efficiently.

## Requirements
- Apache Spark
- PySpark

## Steps
1. **Initialize Spark Session**: Set up a Spark session to handle data processing tasks.
2. **Define Schema**: Define the schema for the CSV file to ensure correct data types.
3. **Load Data**: Load the CSV data into a DataFrame using the defined schema.
4. **Data Transformation**: Convert the `OrderDate` column to a timestamp and extract the year and month.
5. **Aggregation**: For each distinct year-month combination, filter the data, calculate total order quantity and total line total, and display the results.
6. **Save Results**: Save the aggregated data for each month into separate CSV files.

## Usage
1. **Run the Script**: Execute the script using Spark to process the data.
2. **Check Output**: Aggregated data will be displayed in the console, and monthly CSV files will be saved to `/FileStore/tables/`.

## Notes
- Ensure that the input file `Sales_SalesOrderDetail.csv` is correctly placed in the specified path.
- Adjust file paths as needed based on your environment.
- Optional final aggregation and saving of data can be adjusted according to requirements.

## Example Output
For each month, the script will print:

![image](https://github.com/user-attachments/assets/f9386dc4-d2aa-4b1a-9b57-342122b0d310)


The script also generates CSV files named `Sales_<year>_<month>.csv` containing the detailed data for each month.

## License
This project is licensed under the MIT License.

